# lab4_robotica_phantom

En el laboratorio de hoy se trabaja el robot pahntom x 'Pincher', para lograr trabajar con este es necesario contar con lo siguientes recursos de Software.

1. Ubuntu 20.4
2. ROS
3. Dynamixel de Robotis
4. Python 3.9.x
5. Robot Phantom XA
6. Matlab

Con estos recursos es posible llevar acabo este laboratorio.

## Conexión del robot 

El robot se energiza, y pormedio del controlador se conexta via USB al ordenador con el cual será programado.
Luego de esto con Dynamixel se corrobora el funcionamiento correcto de cada servomotor, todo esto con el fin de caracterizr los movimientos maximos y minimos del robot, e cada grado de libertad, y tner la capacidad de ubicar el cero de este, ademas de ver velocidades macimas, y torques maximos.

## Programación de movimientos del robot
 Inicialmente se establece la longitud de cada eslabón del robot, todo esto para realizar la tabla DH y el tipo de movimiento de cada eslabon y asi poder creal el modelo simulado del robot

![ROBOT_SImulado](https://github.com/JuanPabloOrt/lab4_robotica_phantom/assets/144562439/3c7c519e-4470-4170-85cc-fd47d45e9990)
Este robot cuenta con 4 atriculaciones rotativas y ninguna de tipo longitudinal, ademas de la herramienta
