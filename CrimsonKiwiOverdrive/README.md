# Crimson Kiwi Overdrive

The *Crimson Kiwi Overdrive* is a PCB based on the Way Huge Purple Platypus, a fairly rare pedal from the 90s. It's a very heavy "octave overdrive," perhaps closer to an octave fuzz. The octave effect is quite pronounced all the way down the neck, although as with most octave effects it's most prominent above the 12th fret. The circuit is similar to the Way Huge Red Llama.

The Crimson Kiwi name is based on the fact that platypus are very weird mammals... and Kiwis are very weird birds.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/CrimsonKiwiOverdrive/gerber.zip) for fabrication.

## Bill of materials

| References | Value  | Type                   | Note                |
| :--------- | :----- | :--------------------- | :------------------ |
| C1         | 68N    | Film Capacitor         |                     |
| C2         | 120P   | MLCC Capacitor         |                     |
| C3         | 33N    | Film Capacitor         |                     |
| C4         | 120P   | MLCC Capacitor         |                     |
| C5         | 10U    | Electrolytic capacitor |                     |
| C6         | 10U    | Electrolytic capacitor |                     |
| C7         | 10U    | Electrolytic capacitor |                     |
| C8         | 470U   | Electrolytic capacitor |                     |
| C9         | 22U    | Electrolytic capacitor |                     |
| C10        | 47U    | Electrolytic capacitor |                     |
| C100       | 100U   | Electrolytic capacitor |                     |
| D1         | GE     | Germanium Diode        |                     |
| D2         | GE     | Germanium Diode        |                     |
| D100       | LED    | LED                    | Bypass indicator    |
| D101       | 1N5817 | Diode                  | Polarity protection |
| Q1         | 2N3906 | Transistor             |                     |
| Q2         | 2N3904 | Transistor             |                     |
| R1         | 1M     | 1/4W Resistor          |                     |
| R2         | 220K   | 1/4W Resistor          |                     |
| R3         | 68K    | 1/4W Resistor          |                     |
| R4         | 1M     | 1/4W Resistor          |                     |
| R5         | 220K   | 1/4W Resistor          |                     |
| R6         | 4K7    | 1/4W Resistor          |                     |
| R7         | 4K7    | 1/4W Resistor          |                     |
| R8         | 100K   | 1/4W Resistor          |                     |
| R9         | 100K   | 1/4W Resistor          |                     |
| R10        | 100K   | 1/4W Resistor          |                     |
| R11        | 510K   | 1/4W Resistor          |                     |
| R12        | 100K   | 1/4W Resistor          |                     |
| R13        | 10K    | 1/4W Resistor          |                     |
| R14        | 1K5    | 1/4W Resistor          |                     |
| R15        | 100K   | 1/4W Resistor          |                     |
| R16        | 1M     | 1/4W Resistor          |                     |
| R17        | 1K     | 1/4W Resistor          |                     |
| R100       | 4K7    | 1/4W Resistor          | LEDR                |
| U1         | CD4049 | IC                     |                     |
| DRIVE      | B1M    | Potentiometer          |                     |
| VOLUME     | A10K   | Potentiometer          |                     |

All of the parts in this build should be easily sourced. You should be able to use any germanium diodes. Various vero layouts and schematics show different transistors. 2N3904/2N3906 are probably the easiest to source.

This is a mostly straightforward build, but if you want an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/CrimsonKiwiOverdrive/interactive_bom.html) is also available.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure.
* Sockets (for the IC and diodes).
* Wire
* Solder

## Layout

This pedal uses a standard [two-knob layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md).

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

* V1.1 - First public version.
* V1.0 - Unreleated. Verified and works well. Some small layout changes and updates after this build.