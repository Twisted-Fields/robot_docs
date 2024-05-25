# Overview

## Background

Acorn is an organic farming automation research platform, designed to aid in
research and development of new automated organic farming systems. Acorn is a
mobile platform designed to support the future addition of farming tools
suitable for use in a solar powered system.

This development platform solves the problems of mobile autonomous operation
and power management, and serves as a tool for early adopters and developers
to research new farming automation tool development on a standardized open
source platform.

Long term, these tools will be integrated in to the main system design, creating
a complete open source farming automation system.

Our entire system source design files are available on our github:
[https://github.com/Twisted-Fields](https://github.com/Twisted-Fields)

## System Design

Acorn is a rectangular aluminum robot with a power system, main computer, and
four robotic corner assemblies which each contain a drive motor and steering
motor in an aluminum weldment with additional supporting electronics inside.

The main computer is a Raspberry Pi Compute Module 4, and our main software
stack is in python.

The power system is comprised of a solar panel system operating at 45 volts
nominal, an array of supercapacitors to temporarily store power, and simple
power electronics to protect the supercapacitors. There are no batteries -
Acorn operates directly off of solar power.

See also {doc}`materials`

## Corner Assembly

Most of the robotic complexity of Acorn is confined to the four identical
modular corner assemblies that handle drive and steering. These assemblies
bolt to the frame and attach to the chassis wiring to complete the robot.

For more details see {doc}`corner`

## Electronics

Acorn uses a custom motherboard to hold the main computer and interface to the
chassis wiring, a motor control board in each corner assembly, and quite a few
additional support PCBs.

For more details see {doc}`electrical`

## Software

Acorn's system software is primarily written in python. Embedded systems
code is written in C++.

For more details see {doc}`software`

## Mechanical

Acorn uses a MIG welded aluminum frame built from aluminum tubes and CNC plasma
cut aluminum plate.

For more details see {doc}`mechanical`
See also {doc}`frame`
