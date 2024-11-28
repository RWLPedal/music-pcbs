# Shiny Cowbird

The *Shiny Cowbird* is a PCB layout of [Dylan159's Dyl-Ei Fuzz Apprentice](https://bentfishbowl.wixsite.com/electronics/post/dyl-ei-fuzz-apprentice-trev-ei-brazzmaster), which is in turn a version of the Shin-ei FY-2 Companion Fuzz. This is a fuzz with a harsh nasally tone, quite distinct from other fuzzes. It only has a few components, and they're all easily obtained.

## Layout

The layout follows the PedalPCB layout conventions and positions for a 3-knob pedal, and will fit in any drilled 3-knob enclosure drilled for PedalPCB that has the LED at the top of the pedal.

## Bill of materials

| **References** | **Value** | **Description**        | **Notes**                               |
| :------------- | :-------- | :--------------------- | :-------------------------------------- |
| C1             | 47N       | Film capacitor         |                                         |
| C3             | 47N       | Film capacitor         |                                         |
| C2             | 1N        | Film capacitor         |                                         |
| C6             | 1N        | Film capacitor         |                                         |
| C4             | 22N       | Film capacitor         |                                         |
| C5             | 100N      | Film capacitor         |                                         |
| C101           | 100U      | Electrolytic capacitor |                                         |
| R1             | 2M2       | Resistor               |                                         |
| R2             | 22K       | Resistor               |                                         |
| R3             | 470K      | Resistor               |                                         |
| R4             | 47K       | Resistor               |                                         |
| R5             | 10K       | Resistor               |                                         |
| R6             | 1K        | Resistor               |                                         |
| R100           | 4K7       | Resistor               | LEDR                                    |
| R101           | 220R      | Resistor               |                                         |
| D100           | LED       | 3mm LED (display)      | Bypass LED                                        |
| D101           | 1N5817    | Schottky Diode         |                                         |
| Q1             | 2N3904    | NPN Transistor         | Dylan159 doesn't specify the transistor |
| Q2             | 2N3904    | NPN Transistor         | Dylan159 doesn't specify the transistor |
| FUZZ           | B100K     | Potentiometer          |                                         |
| NOTCH          | A100K     | Potentiometer          |                                         |
| VOLUME         | A100K     | Potentiometer          |                                         |

The BOM contains both the bypass LED and LEDR.

## Layout & schematic

Below are the KiCad schematic, front and back traces for the V1.1 layout.

![Screenshot of the circuit's schematic](https://github.com/RWLPedal/music-pcbs/blob/main/ShinyCowbird/images/schematic.png?raw=true)

![Screenshot of the front of the PCB](https://github.com/RWLPedal/music-pcbs/blob/main/ShinyCowbird/images/pcb_front.png?raw=true)

![Screenshot of the back of the PCB](https://github.com/RWLPedal/music-pcbs/blob/main/ShinyCowbird/images/pcb_back.png?raw=true)

### Not listed

As with most BOMs, the following components are not listed:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure (size 125B)
* Wire
* Solder

## Licensing

As with the Dylan159's original schematic, this layout is licensed with a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, share-alike).