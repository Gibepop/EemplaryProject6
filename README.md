# Moving robot navigated by LIDAR camera
# Authors 
- Piotr Słowik
# Description of the project 
A robot that moves in the direction where the distance to the nearest obstacle is greatest. Based on a previous project https://github.com/ComplexityGarage/Lidar

The principle of this project is simple. LIDAR camera is placed on a servo. When it rotates, the distanes between camera and nearest object are measured depending on the angle. After a full rotation the measurements are compared, and the angle for which the distanse was greatest is saved. Then the motor is turning in that direction. After some time this procedure repeats.
# Science and tech used 
## Metal chaissis 2WD
A metal platform with two DC motors. In configuration with raspberry pie it allows to make a fully controlled 2-wheel robot.
(Red Metal Chassis 2WD 2-Wheel with DC Motor Drive)
## Raspberry Pi (4, model B, 2018)
https://www.raspberrypi.com/products/raspberry-pi-4-model-b/
## Lidar distance sensor (TF Luna 8m UARTI2C)
https://botland.store/time-of-flight-sensor/16638-lidar-tf-luna-laser-distance-sensor-8m-uarti2c-5903351249041.html
The full specifications can be found in `TFLuna-specs.pdf` or at https://www.mouser.pl/datasheet/2/1099/Benewake_10152020_TF_Luna-1954056.pdf.
## Servo (FEETECH Standard Servo FS5103B)
https://www.pololu.com/product/3424 
Servo has a running angle of approximately 180°, its angular velocity can be easily modified in a wide range. Full specifications can be found in `FS5103B-specs.pdf`.
## L298N - two-channel motor controller
A module which allows to controll directrion and speed of two DC motors
https://components101.com/modules/l293n-motor-driver-module
## Other:
-a breadboard,
-KORAD DC power supply,
-a lot of wires,
-seld-made wooden "floors" which allowes to fit all parts on the chaissis
# State of the art 
A circuit and the code and are going to be based on the tutorials 
(https://maker.pro/raspberry-pi/projects/make-obstacle-avoiding-robot-raspberry-pi)
and
(https://diyprojectslab.com/raspberry-pi-with-l298n-driver/)

