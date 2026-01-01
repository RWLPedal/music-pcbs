# Shiny Cowbird (Dyl-ei Fuzz Apprentice)

<img src="images/front_guts.png?raw=true" alt="Cover image with gutshot">

The *Shiny Cowbird* is a PCB for [Dylan159's Dyl-ei Fuzz Apprentice](https://bentfishbowl.wixsite.com/electronics/post/dyl-ei-fuzz-apprentice-trev-ei-brazzmaster), which is in turn a modified *Shin-ei FY-2 Companion Fuzz*. This is a fuzz with a distinct harsh nasally tone - charming and quite unique. It only has a few components, and they're all easily obtained.

This Shiny Cowbird name was chosen for two reasons:

1. The original pedal is the *Shin-ei Companion Fuzz*, so I wanted to have *Shiny* in the name.
2. Cowbirds are obligate brood parasites. This means that they cannot construct nests or incubate eggs on their own. Instead, they lay eggs in the nests of other birds, and then the cowbird hatchlings will try to dominate the other hatchlings - by growing faster and often pushing the host hatchlings out of the nest! Quite nasty, but I felt this fit with the "Companion/Apprentice" naming in a dark way!

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/OverdriveFuzz/ShinyCowbirdFuzz/gerber.zip) for fabrication.

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

Dylan159 doesn't specify the transistors to use. I've used 2N3904, but you can experiment with others.

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

This pedal follows the drill conventions for the 
[125B Three-Knob layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md).

### Screenshots

Here are the front and back with traces and component values:

![Screenshot of the front of the PCB](images/pcb_front.png?raw=true)

![Screenshot of the back of the PCB](images/pcb_back.png?raw=true)

Here is the front of the PCB with references rather than values:

![Screenshot of the front of the PCB with references](images/pcb_references.png?raw=true)

### Offboard wiring

Offboard wiring is standard for this pedal. See the [detailed offboard wiring instructions](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/WIRING.md) if you want more specifics.

## Schematic

Below is the KiCad schematic.

![Screenshot of the circuit's schematic](images/schematic.png?raw=true)

## Licensing

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

As with the Dylan159's original schematic, this layout is licensed with a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.2 - Rotate transistors to face the same direction. Small polish to ensure labels look good and slightly increase electrolytic footprint size.
* V1.1 - Fixed transistor and electrolytic capacitor footprints. First public release. Confirmed to work.
* V1.0 - First build. Had bad footprints for transistors and electrolytic capacitor, but still confirmed to work. Never publically released.