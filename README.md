# lab4_robotica_phantom

En el laboratorio de hoy se trabaja el robot pahntom x 'Pincher', para lograr trabajar con este es necesario contar con lo siguientes recursos de Software.

1. Ubuntu 20.4
2. ROS
3. Dynamixel de Robotis
4. Python 3.9.x
5. Robot Phantom XA
6. Matlab

Con estos recursos es posible llevar acabo este laboratorio.

## Conexión y programación del robot 

El robot se energiza, y pormedio del controlador se conexta via USB al ordenador con el cual será programado.
Luego de esto con Dynamixel se corrobora el funcionamiento correcto de cada servomotor, todo esto con el fin de caracterizr los movimientos maximos y minimos del robot, e cada grado de libertad, y tner la capacidad de ubicar el cero de este, ademas de ver velocidades macimas, y torques maximos.

## Programación de movimientos del robot
 Inicialmente se establece la longitud de cada eslabón del robot, todo esto para realizar la tabla DH y el tipo de movimiento de cada eslabon y asi poder creal el modelo simulado del robot

![ROBOT_SImulado](https://github.com/JuanPabloOrt/lab4_robotica_phantom/assets/144562439/3c7c519e-4470-4170-85cc-fd47d45e9990)
Este robot cuenta con 4 atriculaciones rotativas y ninguna de tipo longitudinal, ademas de la herramienta.
ESTE Permite realizar movimientos en el entorno virtual de como se comportaria el robot, y obsrvar la posicion en que quedaría ubicado segun la rotación dada al robot.

![DH](https://github.com/JuanPabloOrt/lab4_robotica_phantom/assets/144562439/07d9b675-9a88-4055-94bf-4df021bbdffe)

Esta es la matriz DH del robot

![ps1_matlab](https://github.com/JuanPabloOrt/lab4_robotica_phantom/assets/144562439/137fdb85-a347-4321-9b49-fa5a96db3841)
Se plotea esta posicion del robot desde Matlab, dando

![pos1_robot](https://github.com/JuanPabloOrt/lab4_robotica_phantom/assets/144562439/4c87f4ad-4a09-42ef-a5e9-57ffc0614028)


Ahora se empieza con el entorno DYNAMIXEL para corroborar  los punto cero de cada articulación en cada motor de cada eslabon y observar los valores maximos de torque.





Luego de esto e procede a crear el codigo PYTHON/MATLAB con el cual se realiza la programacion de movimientos del robot y la creacion de este en el entorno ROS, luego se realizan los pasos de codigo en la consola de linux con el software ROS para crear el pquete de robot segun el github  https://github.com/felipeg17/px_robot. COn este se crea el entorno del robot, y luego se procede a dar un movimiento a partir de un codigo Python, luego se ejecuta creando el entorno catwin_ws en ROS dando asi lugar al siguiente movimiento de prueba




https://github.com/JuanPabloOrt/lab4_robotica_phantom/assets/144562439/1ef7a2ec-f235-41c1-bd25-2331b9a46013


Este movimiento nos demuestra que el software ROS pemite programar rutinas para robots, ya que se le podria la orden de bucle para este movimiento, observamos el movimiento en todos los eslabones, ademas de que es un software libre, por lo cual permite realizar desarrollos academicos e industriales de bajo coste.

Ahora se procede implementando las 5 posiciones del robot deseadas, esto con el fin de demostrar que se podría implementar una rutina en bucle para realizar tareas desde ROS implementado y Python. Dando asi el siguiente video



##  Conclusiones

ROS es una herramienta computacional muy util par ahacer desarrollos en el area de robotica, por lo que nos da la posibilidad de interactuar en tiempo real con robots, por otra parte Linux siempre presenta pequeños bus al momento de empezar a utilizar un nuevo software, lo cual dificultó el acople de ROS con Python y el robot Phantom. Esta parte siempre es la mas demandante de trabajr en este enetorno. El robot Pahntom se deja mover en los 5 grados de libertad que tiene a una velocidad baja, estos servomotores manejan un elevado torque por lo cual es imperativo dar un aterrizaje al robot correctamente para lograr hacer movimientos a una mayor velocidad.

