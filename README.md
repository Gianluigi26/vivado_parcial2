### Maquina de estados vivado 
1.	RTL Code (Registre-Transfer Level)
En este paso describimos el comportamiento de un circuito digital a nivel abstracción que incluye registros, utilizando leguaje de descripción de hardware (HDL), al igual que se describe los términos de los registros que almacenaran los datos, y la trasferencia de datos entre los tipos de registros, también definimos las entras y salidas,  como también creamos señales internas .
![Imagen1](https://github.com/Gianluigi26/vivado_parcial2/assets/54091081/8d5e3bd4-4513-4770-9c8e-45f9c8daf38d)
![image](https://github.com/Gianluigi26/vivado_parcial2/assets/54091081/167c7aad-dcec-4823-beff-d9a269841032)

-2.	Simulation
En este paso se emplea la herramienta de simulación para verificar el comportamiento del diseño antes de sintetizarlo en un dispositivo FPGA real. Se crean tesbenches, que verifican la sintaxis, para el funcionamiento del código. Esto para que se cumpla la funcionalidad y en tiempos. Acá podemos ver que nuestro código comienza en estado S0, donde vemos que TA es positivo y por ende se verifica que nuestras funciones de verde en TA y rojo en TB se esta cumpliendo, si arrastramos la barra amarilla podemos ver que sigue el código, hasta el estado TB, en la parte superior podemos ver nuestra entra del clck. 
![image](https://github.com/Gianluigi26/vivado_parcial2/assets/54091081/4343e83e-84cc-4e41-a7fd-eea3eb5053ba)
![image](https://github.com/Gianluigi26/vivado_parcial2/assets/54091081/069b1872-e7a0-4300-99e2-d5b689a386c5)
![image](https://github.com/Gianluigi26/vivado_parcial2/assets/54091081/09f1201b-82fd-4893-98e3-6d933da4a52b)

-3.	Synthesis
El proceso de síntesis se convierte la descripción del comportamiento del circuito digital en una representación más detallada que se puede implementar en el hardware real. Esto quiere decir que va a transformar el código a nivel de compuertas y flip flop. En otras palabras, Este proceso implica mapear las estructuras lógicas y las interconexiones especificadas en el código HDL a los recursos físicos disponibles en la FPGA. En este proceso se verifica que el código HDL este correctamente estructurado y sin errores, como también optimiza la lógica para tener un mejor rendimiento ya que reduce el espacio que ocupara en la FPGA.

Acá podemos ver como se asignan las funciones lógicas y las conexiones entre ellas a los bloques lógicos, como también vemos como estables las mejores rutas para las interconexiones de nuestro Código. 
![image](https://github.com/Gianluigi26/vivado_parcial2/assets/54091081/63c2a910-4165-4e31-bca0-58d544314b28)
![image](https://github.com/Gianluigi26/vivado_parcial2/assets/54091081/20891c3d-3e89-4629-b96b-e1d1f012bb09)

-4.	Implementation
En este paso es donde se lleva a cabo la asignación física de recursos y el enrutamiento de conexiones para nuestro diseño en la FPGA específica seleccionada. 

Acá se nos crea la netlis que nos permite rutear, cerrar los circuitos necesarios a  implementar, que ejecutaran las funciones lógicas.  Acá podemos verificar varios buffers ya que nos garantizan la señal.

Una vez completado el paso de implementación con éxito, estamos listo para cargar el bitstream generado en la FPGA para probar y ejecutar nuestro diseño en hardware real.

![image](https://github.com/Gianluigi26/vivado_parcial2/assets/54091081/70413e0b-9a25-4784-bf96-616e1a025f15)
![image](https://github.com/Gianluigi26/vivado_parcial2/assets/54091081/4923d90f-e06e-45bc-8321-8ea263e23d3f)

-5	Device programming (programación del Dispositivo) 
implica cargar el bitstream generado durante la implementación en el dispositivo FPGA real o en la tarje de programación. Acá ya procedemos a cargas nuestro código a la placa para ya visualizar físicamente nuestro circuito. 

![image](https://github.com/Gianluigi26/vivado_parcial2/assets/54091081/3cf85aa2-3658-4cf2-b409-873cd0982a4f)
![image](https://github.com/Gianluigi26/vivado_parcial2/assets/54091081/c4c43b35-7586-45bb-96eb-5564b7390036)


video de del circuito en funcionamineto  
https://youtu.be/0PnA4kRwHDA

