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
Este robot cuenta con 4 atriculaciones rotativas y ninguna de tipo longitudinal, ademas de la herramienta.
ESTE Permite realizar movimientos en el entorno virtual de como se comportaria el robot, y obsrvar la posicion en que quedaría ubicado segun la rotación dada al robot.

![DH](https://github.com/JuanPabloOrt/lab4_robotica_phantom/assets/144562439/07d9b675-9a88-4055-94bf-4df021bbdffe)

Esta es la matriz DH del robot

Se plotea esta posicion del robot desde Matlab

![ROBOT_SImulado](htt![ps1_matlab](https://github.com/JuanPabloOrt/lab4_robotica_phantom/assets/144562439/101f5dcd-011a-447d-828d-fe907e1cd02e)
ps://github.com/JuanPabloOrt/lab4_robotica_phantom/assets/144562439/ac61994b-f7f1-43fa-a8ce-c88b92db890b)

Ahora se empieza con el entorno DYNAMIXEL para corroborar  los punto cero de cada articulación en cada motor de cada eslabon y observar los valores maximos de torque.


INSERTAR IMAGENES DYMAMIXEL Y QUE SE HIZO


Luego de esto e procede a crear el codigo PYTHON/MATLAB con el cual se realiza la programacion de movimientos del robot y la creacion de este en el entorno ROS, luego se realizan los pasos de codigo en la consola de linux con el software ROS para crear el pquete de robot segun el github  https://github.com/felipeg17/px_robot. COn este se crea el entorno del robot, y luego se procede a 
