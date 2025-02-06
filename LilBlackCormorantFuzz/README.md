# L'il Black Cormorant Fuzz

The *L'il Black Cormorant Fuzz* is a PCB based on the Build Your Own Clone (BYOC) "L'il Black Key," which itself is a modified verson of the MFZ-1 Fuzz. The original name is because there are references to the band The Black Keys using the Maestro. BYOC announced they were shutting down in 2024 and the original circuit is no longer commercially available. This pedal has all commodity components, there are no mojo parts.

The name for this pedal, the [L'il Black Cormorant](https://ebird.org/species/libcor1), is an obvious reference to the BYOC pedal name. Cormorants are a family of diving birds which are not waterproof, commonly found worldwide. The Little Black Cormorant is located primarily around Australia and the South Pacific.

If you'd like to just get started with the build, you can [find the PCB on PCBWay](https://www.pcbway.com/project/shareproject/L_il_Black_Cormorant_PCB_a7334241.html) (I will receive a small commission if you order from them). Alternately, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/LilBlackCormorantFuzz/gerber.zip) for fabrication.

## Bill of materials


| References | Value  | Type                   | Notes               |
| :--------- | :----- | :--------------------- | :------------------ |
| C1         | 100N   | Film Capacitor         |                     |
| C2         | 2U2    | Electrolytic Capacitor |                     |
| C3         | 2U2    | Electrolytic Capacitor |                     |
| C4         | 220P   | MLCC Capacitor         |                     |
| C5         | 220N   | Film Capacitor         |                     |
| C100       | 2U2    | Electrolytic Capacitor |                     |
| R1         | 470K   | 1/4W Resistor          |                     |
| R2         | 1M     | 1/4W Resistor          |                     |
| R3         | 1M     | 1/4W Resistor          |                     |
| R4         | 2K2    | 1/4W Resistor          |                     |
| R5         | 1M     | 1/4W Resistor          |                     |
| R6         | 10K    | 1/4W Resistor          |                     |
| R100       | 4K7    | 1/4W Resistor          | LEDR                |
| R101       | 2M2    | 1/4W Resistor          |                     |
| R102       | 2M2    | 1/4W Resistor          |                     |
| D1         | 1N4148 | Diode                  |                     |
| D2         | 1N4148 | Diode                  |                     |
| D3         | 1N4148 | Diode                  |                     |
| D4         | 1N4148 | Diode                  |                     |
| D100       | LED    | LED                    | Bypass Indicator    |
| D101       | 1N5817 | Schottky Diode         | Polarity Protection |
| U1         | RC4558 | IC                     |                     |
| DRIVE      | A100K  | Potentiometer          |                     |
| VOLUME     | A100K  | Potentiometer          |                     |

All of the parts in this build should be easily sourced.

This is a mostly straightforward build, but if you want an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/LilBlackCormorantFuzz/interactive_bom.html) is also available.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure. Unlike the original, it wasn't designed for a smaller enclosure.
* Sockets (for the ICs and diodes).
* Wire
* Solder

## Layout

This pedal uses the standard [125B two knob layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md).

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

* V0.9 - First version, worked perfectly. There were no subsequent changes to the fabricated pcb. Thanks to [PCBWay](https://www.pcbway.com/), [project link](https://www.pcbway.com/project/shareproject/L_il_Black_Cormorant_PCB_a7334241.html) for sponsoring the fabrication of the test build.