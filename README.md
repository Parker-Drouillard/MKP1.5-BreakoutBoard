# MKP1.5-BreakoutBoard
A breakout board for supporting dual extrusion &amp; 6 pwm fan control for the Rambo 1.4 

This board supports a Teensy 2.0 slave device to the Rambo 1.4 over Serial. The purpose of this board is to expand the available IO of the Rambo 1.4 to be capable of supporting a dual extrusion system, as well as additional PWM fan controls.

## About this board
This board offers 6 5v fan headers for PWM switching via a darlington array. At this current time, it does not seem the max PWM speed of the Teensy 2.0 is sufficient to run the fans at less than 100% power, so for the time being it is simply a toggle of Off or On.
The board includes a 24V to 5V buck converter, capable of supporting 3A of power, of which only 2A is anticipated to be used. Additionally, 2 ports for PT1000 passthrough, and 2 ports for E3D PT100 Amplifier boards are provided. 
An onboard L298N allows for low voltage switching of 2 independant 24V systems, one of which is being used for the second extruder solenoid, and one will be used in the future fora dynamic extruder pressure motor. Both systems have 2 encontrol pins, 1 for forward, and 1 for reverse. 
