# Shiny Cowbird (Dyl-ei Fuzz Apprentice)

The *Shiny Cowbird* is a PCB layout of [Dylan159's Dyl-Ei Fuzz Apprentice](https://bentfishbowl.wixsite.com/electronics/post/dyl-ei-fuzz-apprentice-trev-ei-brazzmaster), which is in turn a version of the Shin-ei FY-2 Companion Fuzz. This is a fuzz with a harsh nasally tone, quite distinct from other fuzzes. It only has a few components, and they're all easily obtained.

The name has two meanings. First, the original pedal is the *Shin-ei fuzz apprentice*, so I wanted to have *Shiny* in the name. Second, cowbirds are obligate brood parasites. This means that they cannot construct nests or incubate eggs on their own. Instead, they lay eggs in the nests of other birds, and then the cowbird hatchlings will try to dominate the food consumption - often pushing the host hatchlings out of the nest! Quite nasty, but I felt this somewhat fit with the "Companion/Apprentice" naming.

## Bill of materials

| **References** | **Value** | **Description**        | **Notes**                                        |
| :------------- | :-------- | :--------------------- | :----------------------------------------------- |
| C1             | 47N       | Film capacitor         |                                                  |
| C3             | 47N       | Film capacitor         |                                                  |
| C2             | 1N        | Film capacitor         |                                                  |
| C6             | 1N        | Film capacitor         |                                                  |
| C4             | 22N       | Film capacitor         |                                                  |
| C5             | 100N      | Film capacitor         |                                                  |
| C101           | 100U      | Electrolytic capacitor |                                                  |
| R1             | 2M2       | 1/4W Resistor          |                                                  |
| R2             | 22K       | 1/4W Resistor          |                                                  |
| R3             | 470K      | 1/4W Resistor          |                                                  |
| R4             | 47K       | 1/4W Resistor          |                                                  |
| R5             | 10K       | 1/4W Resistor          |                                                  |
| R6             | 1K        | 1/4W Resistor          |                                                  |
| R100           | 4K7       | 1/4W Resistor          | LEDR                                             |
| R101           | 220R      | 1/4W Resistor          |                                                  |
| D100           | LED       | 3mm LED (display)      | Bypass LED                                       |
| D101           | 1N5817    | Schottky Diode         |                                                  |
| Q1             | 2N3904    | NPN Transistor         | Dylan159 doesn't specify the specific transistor |
| Q2             | 2N3904    | NPN Transistor         | Dylan159 doesn't specify the specific transistor |
| FUZZ           | B100K     | Potentiometer          |                                                  |
| NOTCH          | A100K     | Potentiometer          |                                                  |
| VOLUME         | A100K     | Potentiometer          |                                                  |

Note that the bypass indicator LED and LEDR are on the PCB, and are listed here in the BOM.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal will fit in a 125B enclosure
* Sockets (if you want to socket the transistors).
* Wire
* Solder

## Layout

The layout follows the PedalPCB layout conventions and positions for a 3-knob pedal, and will fit in any drilled 3-knob enclosure drilled for PedalPCB that has the LED at the top of the pedal.

### Screenshots

Here are the front and back with traces and component values:

![Screenshot of the front of the PCB](https://github.com/RWLPedal/music-pcbs/blob/main/ShinyCowbird/images/pcb_front.png?raw=true)

![Screenshot of the back of the PCB](https://github.com/RWLPedal/music-pcbs/blob/main/ShinyCowbird/images/pcb_back.png?raw=true)

Here is the front of the PCB with references rather than values:

![Screenshot of the front of the PCB with references](https://github.com/RWLPedal/music-pcbs/blob/main/ShinyCowbird/images/pcb_references.png?raw=true)

### Schematic

Below are the KiCad schematic, front and back traces for the V1.1 layout.

![Screenshot of the circuit's schematic](https://github.com/RWLPedal/music-pcbs/blob/main/ShinyCowbird/images/schematic.png?raw=true)

## Licensing

As with the Dylan159's original schematic, this layout is licensed with a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).