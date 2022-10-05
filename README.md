# Rheology-LabVIEW-Motor-Controller
 Desktop UI for Rheology experiment Nanotec PD4-C Motor Controller
 
## Description

This software is designed to interface Nanotec PD4-C Stepper Motors, with a user friendly LabVIEW Interface.

## Prerequisits

Proper function of the software relies on the correct NanoJ program to be installed on the PD4-C Stepper motor. This program can be found in the `PD4-C NanoJ Program` folder. 

Inside this folder is the C++ like NanoJ program `vmmcode.cpp` an a copy of the `nanotec.h` library. It also contains an additonal folder called `CURRENT MOTOR FIRMWARE` which contains the latest working copy of the contents of the PD4-C Motor Flash storage drive. 
This includes:

- CFG.TXT  _Config file for motor initialisation_
- INFO.BIN   _Hardware generated file_
- VMMCODE.USR  _Compiled NanoJ program using Plug & Drive Studio_

The NanoJ software can be updated and programmed into the PD4-C Motor using Nanotec's Plug & Drive Studio.

# Usage
## Hardware Controller

When the motor is first powered on, it will immediatly start running the internal NanoJ program. This allows the motor to be controlled via the supplied hardware controller. This has 3 controls:

- Enable Motor _(On/Off)_
- Speed
- Direction _(CW/CCW)_

# Warning! - Hardware controller has no automatic stop on power on! Motor will actuate if speed control is not at ZERO position and Enable Motor is switched to ON.
# - It is reccomended to 

