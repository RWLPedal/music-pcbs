# L'il Black Cormorant Fuzz

The *L'il Black Cormorant Fuzz* is a PCB based on the Build Your Own Clone (BYOC) "L'il Black Key," which itself is a modified verson of the MFZ-1 Fuzz. The original name is because there are references to the band The Black Keys using the Maestro. BYOC announced they were shutting down in 2024 and the original circuit is no longer commercially available. This pedal has all commodity components, there are no mojo parts.

The name for this pedal, the [L'il Black Cormorant](https://ebird.org/species/libcor1), is an obvious reference to the BYOC pedal name. Cormorants are a family of diving birds which are not waterproof, commonly found worldwide. The Little Black Cormorant is located primarily around Australia and the South Pacific.

If you'd like to just get started with the build, you can [find the PCB on PCBWay](https://www.pcbway.com/project/shareproject/L_il_Black_Cormorant_PCB_a7334241.html) (I will receive a small commission if you order from them). Alternately, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/LilBlackCormorantFuzz/gerber.zip) for fabrication.

## Bill of materials

| References | Value   | Type                  | Notes               |
| :--------- | :------ | :-------------------- | :------------------ |
| C1         | 47N     | Film Capacitor        |                     |
| C2         | 33N     | Film Capacitor        |                     |
| C3         | 47P     | MLCC Capacitor        |                     |
| C4         | 47N     | Film Capacitor        |                     |
| C5         | 6N8     | Film Capacitor        |                     |
| C6         | 22N     | Film Capacitor        |                     |
| C7         | 220N    | Film Capacitor        |                     |
| C8         | 1U      | Film Capacitor        |                     |
| C100       | 100U    | Electrolyic Capacitor |                     |
| D1         | GE      | Germanium Diode       |                     |
| D2         | GE      | Germanium Diode       |                     |
| D3         | 1N4148  | Diode                 |                     |
| D100       | LED     | LED                   | Bypass Indicator    |
| D101       | 1N5817  | Schottky Diode        | Polarity protection |
| Q1         | PN2222A | Transistor            |                     |
| Q2         | 2N3906  | Transistor            |                     |
| Q3         | BC109C  | Transistor            |                     |
| R1         | 10K     | 1/4W Resistor         |                     |
| R2         | 560K    | 1/4W Resistor         |                     |
| R3         | 560K    | 1/4W Resistor         |                     |
| R4         | 150K    | 1/4W Resistor         |                     |
| R5         | 22K     | 1/4W Resistor         |                     |
| R6         | 15K     | 1/4W Resistor         |                     |
| R7         | 100R    | 1/4W Resistor         |                     |
| R8         | 47K     | 1/4W Resistor         |                     |
| R9         | 15K     | 1/4W Resistor         |                     |
| R10        | 82K     | 1/4W Resistor         |                     |
| R11        | 1K      | 1/4W Resistor         |                     |
| R100       | 4K7     | 1/4W Resistor         | LEDR                |
| DEATH      | B500K   | Potentiometer         |                     |
| INPUT      | A100K   | Potentiometer         |                     |
| LIFE       | B100K   | Potentiometer         |                     |
| STARVE     | B100K   | Potentiometer         |                     |
| VOODOO     | A100K   | Potentiometer         |                     |

There are a feew unusual components to this build. The original schematic used a 2N2222A. This is somewhat expensive ($2-$3), depending on your source. The PCB shows PN2222A, which is very cheap. Likewise, the original calls out a BC109C. I used a BC109 with no apparent adverse effects.

I believe that any germanium diodes should work. I think I used D9Gs.

This is a mostly straightforward build, but if you want an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/LilBlackCormorantFuzz/interactive_bom.html) is also available.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure.
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

* V0.9 - First version, worked perfectly. Very minor subsequent silkscreen changes. Thanks to [PCBWay](https://www.pcbway.com/) for sponsoring the fabrication of the test build. You can get the exact board I fabricated [here](https://www.pcbway.com/project/shareproject/L_il_Black_Cormorant_PCB_a7334241.html).