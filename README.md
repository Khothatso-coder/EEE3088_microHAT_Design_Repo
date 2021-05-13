# Motor driver with position feedback HAT
## Overview

This is a DC motor HAT for Raspberry Pi board that consist of three modules with an on-board motor controller that keeps track of the position, speed and direction of the motor.
The HAT consist of power supply unit, motor driver IC, motor position feedback sensor providing an input signal within 0-3.3V, and LEDs status circuitry displaying the motor power, motor direction, motor connected/not and high current draw warning.

## Runnign simulations files on LTSpice
Please see the appropriate guide for running the uploaded LTSpice simulation files for each sub-module and software installation:
-   [LTspice Information Flyer & Shortcuts](https://www.analog.com/en/license/spice-models?mediaPath=media/en/simulation-models/spice-models/LTspice_ShortcutFlyer.pdf&modelType=spice-models)
-   [Download for Windows 7, 8 and 10](https://ltspice.analog.com/software/LTspiceXVII.exe) and
-   [Download for Mac 10.9+ U](https://ltspice.analog.com/software/LTspice.pkg)

## Specific instructions on how the HAT could be used.
This microHAT is perfect for any motion applications as it can drive Stepper motors with full PWM speed control and position control. Use a PWM driver chip onboard to both control motor direction and speed. This chip handles all the motor and speed controls over I2C. Only two GPIO pins (SDA & SCL) are required to drive the multiple motors(if necessary), and since it's I2C you can also connect any other I2C devices or HATs to the same pins.
To achieve the required position accuracy, use stepper motors which include Hall effect sensor circuitry that keeps track of the rotor position. 

## Common applications relevant to this HAT.
This PiHAT is relevant in designing robots that keeps track of the position of their motors to keep track of their position or just to control the speed of it more precise and accurate. Clients could use this microHAT in the operations of automation and robotic equipment where a high accuracy requirement of the position feedback sensor in a high speed application is required. This microHAT could be useful in situations whereall components need to be infused into a limited PCB space to fit inside tiny enclosures, such as robotic arm.

## Contributing to this repository
We would appreciate your input! We want to make contributing to this project as easy and transparent as possible, whether it's:

- Uploading submodules simulations files.
- Reporting any issues related to simulations files uploaded
- Discussing the current state of the microHAT
- Submitting a fix
- Proposing new features

## Any contributions you make will be under the MIT Software License
In short, when you submit simulation changes, your submissions are understood to be under the same [MIT License](http://choosealicense.com/licenses/mit/) that covers the project. Feel free to contact the maintainers if that's a concern.