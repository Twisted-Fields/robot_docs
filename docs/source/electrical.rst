Electrical
=====

Acorn's electrical system can broadly be described as a motherboard
communicating with four corner assemblies using `CAN bus <https://en.wikipedia.org/wiki/CAN_bus>`_.

Chassis Wiring
------------

We use a custom data cable system with two CAN bus circuits and a special
emergency stop system, plus a second set of cables to carry power. One CAN bus
circuit is used specifically for our motor controllers, while the other circuit
is available for general use.

Power cables are generally 12 gauge silicone jacketed wire terminated with
Anderson PP45 crimp connectors. We use `this wire specifically <https://bntechgo.com/bntechgo-12-gauge-silicone-wire-spool-50-feet-25-ft-black-and-25-ft-red-ultra-flexible-high-temp-200-deg-c-600v/>`_.

Circuit Boards
----------

Acorn relies on an extensive set of custom circuit boards. The two most
important boards are the motherboard and the motor controller, with other boards
supporting these in a few ways.

#### Motherboard

Holds the main computer, a Raspberry Pi Compute Module 4, and communicates
with the four motor controllers using CAN bus. Also manages GPS, wifi, emergency
stop system, and several other functions.
For more information see :doc:`pcb/motherboard`
