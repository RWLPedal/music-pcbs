# Northern Harrier Distortion

The *Northern Harrier Distortion* is a PCB based on the famous ProCo RAT. There's little to be said about this distortion that hasn't alread been said.

This layout is named after the Northern Harrier. The Harrier is a unique raptor known primarily for its habit of flying low over fields while hunting. Unlike hawks or falcons, it rarely flies above the treeline. It has an unsual owl-like face and its behavior is similar to diurnal owls, such as short-eared owls. The name was chosen because the Northern Harrier hunts rodents... such as RATs.

If you'd like to just get started with the build, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/NorthernHarrierDistortion/gerber.zip) for fabrication.

## Bill of materials

| References | Value  | Description                             |
| :--------- | :----- | :-------------------------------------- |
| C1         | 22N    | Film capacitor                          |
| C2         | 1N     | Film capacitor                          |
| C3         | 30P    | MLCC Capacitor                          |
| C4         | 100P   | MLCC Capacitor                          |
| C5         | 2U2    | Electrolytic capacitor                  |
| C6         | 4U7    | Electrolytic capacitor                  |
| C7         | 4U7    | Electrolytic capacitor                  |
| C8         | 3N3    | Film capacitor                          |
| C9         | 22N    | Film capacitor                          |
| C10        | 1U     | Film capacitor                          |
| C100       | 100U   | Electrolytic capacitor                  |
| C101       | 100N   | Film capacitor                          |
| C102       | 1U     | Film capacitor                          |
| R1         | 1M     | 1/4W Resistor                           |
| R2         | 1M     | 1/4W Resistor                           |
| R3         | 1K     | 1/4W Resistor                           |
| R4         | 47R    | 1/4W Resistor                           |
| R5         | 560R   | 1/4W Resistor                           |
| R6         | 1K     | 1/4W Resistor                           |
| R7         | 1K5    | 1/4W Resistor                           |
| R8         | 1M     | 1/4W Resistor                           |
| R9         | 10K    | 1/4W Resistor                           |
| R100       | 4K7    | 1/4W Resistor                           |
| R101       | 47R    | 1/4W Resistor                           |
| R102       | 100K   | 1/4W Resistor                           |
| R103       | 100K   | 1/4W Resistor                           |
| D1         | 1N914  | Diode                                   |
| D2         | 1N914  | Diode                                   |
| D100       | 1N5817 | Diode                                   |
| D101       | LED    | Light emitting diode (bypass indicator) |
| Q1         | 2N5458 | JFET transistor                         |
| U1         | LM308  | OpAmp                                   |
| DISTORTION | A100K  | Potentiometer                           |
| FILTER     | A100K  | Potentiometer                           |
| VOLUME     | A100K  | Potentiometer                           |

Note that the bypass indicator LED and LEDR are on the PCB, and are listed here in the BOM.

The original RAT is well-known for using an LM308 OpAmp. This IC can be hard to find, or expensive, but the chip is said to be distinctive. Most recent RATs have used an OP07 instead. You can use either IC.

Likewise, several transistors will work - various schematics refer to a 2N5458, 2N5457, 2N5485, 2N3819, MPF102, BF245A. This layout includes pads to use an SMD transistor. You can use either the SMD or a through-hole component.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal will fit in a 125B enclosure
* Sockets (if you want to socket the transistor or IC, which is recommended).
* Wire
* Solder

## Layout

The layout follows the PedalPCB layout conventions and positions for a 3-knob pedal. You should be able to use it interchangeably with PedalPCB three-knob enclosures, or three-knob enclosures from my other layouts. The LED is positioned to go in line between the two knobs at the top of the pedal.

### Screenshots

Here are the front and back with traces and component values:

![Screenshot of the front of the PCB](https://github.com/RWLPedal/music-pcbs/blob/main/NorthernHarrierDistortion/images/pcb_front.png?raw=true)

![Screenshot of the back of the PCB](https://github.com/RWLPedal/music-pcbs/blob/main/NorthernHarrierDistortion/images/pcb_back.png?raw=true)

Here is the front of the PCB with references rather than values:

![Screenshot of the front of the PCB with references](https://github.com/RWLPedal/music-pcbs/blob/main/NorthernHarrierDistortion/images/pcb_references.png?raw=true)

### Offboard wiring

Offboard wiring is standard for this pedal. See the [detailed offboard wiring instructions](https://github.com/RWLPedal/music-pcbs/instructions/WIRING.md) if you want more specifics.

## Schematic

Below is the KiCad schematic.

![Screenshot of the circuit's schematic](https://github.com/RWLPedal/music-pcbs/blob/main/NorthernHarrierDistortion/images/schematic.png?raw=true)

## Licensing

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

This PCB is released under a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.1 - Fix error with transistor pin order in V1.0. Introduced SMD option for transistor. Also, make small text and layout tweaks.
* V1.0 - First build. Verified to work. 