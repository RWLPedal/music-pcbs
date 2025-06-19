# Horus Fuzz

![Horus logo](images/logo.png)

The *Horus Fuzz* is a PCB based on the Black Art Toneworks Pharoah, a type of silicon tonebender. This is one of my favorite fuzz pedals, with a ton of sounds, all of them good. There's a limited number of parts, all of which are easily sourced. 

The name from this pedal is based on ancient Egyptian god Horus, who has the head of a falcon (a peregrine falcon in this case). I thought this was a fitting name for a pedal based on a pharoah. Peregrine falcons are the fastest animals on the planet (measured at 242 mph) while diving towards prey.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/HorusFuzz/HorusFuzz.zip) for fabrication.

## Bill of materials


| References | Value  | Type                   | Notes            |
| :--------- | :----- | :--------------------- | :--------------- |
| C1         | 10N    | Film capacitor         |                  |
| C2         | 10U    | Electrolytic capacitor |                  |
| C3         | 100N   | Film capacitor         |                  |
| C5         | 100N   | Film capacitor         |                  |
| C7         | 100N   | Film capacitor         |                  |
| C4         | 4U7    | Electrolytic capacitor |                  |
| C6         | 8N2    | Film capacitor         |                  |
| C100       | 100N   | Film capacitor         |                  |
| C101       | 100U   | Electrolytic capacitor |                  |
| R1         | 150K   | 1/4W Resistor          |                  |
| R2         | 22K    | 1/4W Resistor          |                  |
| R3         | 10K    | 1/4W Resistor          |                  |
| R4         | 1K     | 1/4W Resistor          |                  |
| R5         | 10K    | 1/4W Resistor          |                  |
| R6         | 100R   | 1/4W Resistor          |                  |
| R7         | 47K    | 1/4W Resistor          |                  |
| R8         | 1K     | 1/4W Resistor          |                  |
| R9         | 750R   | 1/4W Resistor          |                  |
| R10        | 100R   | 1/4W Resistor          |                  |
| R11        | 10K    | 1/4W Resistor          |                  |
| R12        | 4K7    | 1/4W Resistor          |                  |
| R13        | 10K    | 1/4W Resistor          |                  |
| R14        | 2K2    | 1/4W Resistor          |                  |
| RPD1       | 2M2    | 1/4W Resistor          |                  |
| R100       | 4K7    | 1/4W Resistor          | LEDR             |
| R101       | 100R   | 1/4W Resistor          |                  |
| D100       | LED    | LED                    | Bypass indicator |
| D101       | 1N5817 | Schottky diode         |                  |
| Q1         | 2N5088 | Transistor             |                  |
| Q2         | 2N5088 | Transistor             |                  |
| Q3         | 2N5088 | Transistor             |                  |
| Q4         | 2N5088 | Transistor             |                  |
| BIAS       | B25K   | 16mm potentiometer     |                  |
| FAT        | A100K  | 16mm potentiometer     |                  |
| GAIN       | B1K    | 16mm potentiometer     |                  |
| TONE       | B50K   | 16mm potentiometer     |                  |
| VOLUME     | A100K  | 16mm potentiometer     |                  |


All of the parts in this build should be very easily sourced.

If you want, an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/HorusFuzz/interactive_bom.html) is also available if you want the option of sorting components or highlighting them on the board.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure.
* Sockets (for the transistors).
* Wire
* Solder

## Layout

This pedal follows the drill conventions for the 
[125B Five-Knob, LED Bottom layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md).

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

This layout is licensed with a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.2 - Substantial revisions to clean up layout, fix suboptimal traces, add logos.
* V1.0 - First version, worked fine.