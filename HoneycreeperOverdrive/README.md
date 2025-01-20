# Honeycreeper Overdrive

<img src="https://github.com/RWLPedal/music-pcbs/blob/main/HoneycreeperOverdrive/images/honeycreeper_overdrive.png?raw=true" alt="Cover image with gutshot" height="500px">

The *Honeycreeper Overdrive* is a PCB based on the Mad Professor Sweet Honey OD, one of many variations of the same pedal that also includes the Honey Bee. This pedal is based on a 2010 schematic trace credited to Yitzhak Turner-Schnell. It's a relatively transparent low-gain overdrive that was more popular in the late 2010s. The components are relatively cheap and easily sourced - the only hard-to-find part is the OP275 opamp.

The Honeycreeper name was chosen due to the obvious honey reference. The bird on the design above is a [Green Honeycreeper](https://ebird.org/species/grehon1), relatively common bird found in Central and South America. Honeycreepeprs are a family of small songbirds in the tanager family. They eat a variety of fruits and insects.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/HoneycreeperOverdrive/gerber.zip) for fabrication.

## Bill of materials


| References | Value  | Description            |
| :--------- | :----- | :--------------------- |
| C3         | 4N7    | Film capacitor         |
| C9         | 4N7    | Film capacitor         |
| C15        | 4N7    | Film capacitor         |
| C8         | 22N    | Film capacitor         |
| C10        | 22N    | Film capacitor         |
| C11        | 22N    | Film capacitor         |
| C1         | 22U    | Electrolytic capacitor |
| C12        | 22U    | Electrolytic capacitor |
| C6         | 1U     | Film capacitor         |
| C14        | 1U     | Film capacitor         |
| C2         | 220N   | Film capacitor         |
| C4         | 22U    | Electrolytic capacitor |
| C5         | 100P   | MLCC capacitor         |
| C7         | 100U   | Electrolytic capacitor |
| C13        | 1N     | Film capacitor         |
| R9         | 47K    | 1/4W Resistor          |
| R10        | 47K    | 1/4W Resistor          |
| R18        | 47K    | 1/4W Resistor          |
| R1         | 5K6    | 1/4W Resistor          |
| R17        | 5K6    | 1/4W Resistor          |
| R2         | 1M     | 1/4W Resistor          |
| R15        | 1M     | 1/4W Resistor          |
| R3         | 4K7    | 1/4W Resistor          |
| R4         | 1K     | 1/4W Resistor          |
| R5         | 360K   | 1/4W Resistor          |
| R6         | 6K8    | 1/4W Resistor          |
| R7         | 51R    | 1/4W Resistor          |
| R8         | 3K     | 1/4W Resistor          |
| R11        | 2K     | 1/4W Resistor          |
| R12        | 13K7   | 1/4W Resistor          |
| R13        | 10K    | 1/4W Resistor          |
| R14        | 150K   | 1/4W Resistor          |
| R16        | 2K6    | 1/4W Resistor          |
| D2         | LED    | 3mm LED (display)      |
| D3         | LED    | 3mm Red LED            |
| D4         | LED    | 3mm Red LED            |
| D7         | LED    | 3mm Red LED            |
| D5         | 1N4007 | Diode                  |
| D6         | 1N4007 | Diode                  |
| D1         | 1N5817 | Diode                  |
| U1         | OP275  | IC                     |
| FOCUS      | B50K   | Potentiometer          |
| VOL        | B50K   | Potentiometer          |
| DRIVE      | A500K  | Potentiometer          |

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

![Screenshot of the front of the PCB](https://github.com/RWLPedal/music-pcbs/blob/main/HoneycreeperOverdrive/images/pcb_front.png?raw=true)

![Screenshot of the back of the PCB](https://github.com/RWLPedal/music-pcbs/blob/main/HoneycreeperOverdrive/images/pcb_back.png?raw=true)

Here is the front of the PCB with references rather than values:

![Screenshot of the front of the PCB with references](https://github.com/RWLPedal/music-pcbs/blob/main/HoneycreeperOverdrive/images/pcb_references.png?raw=true)

### Offboard wiring

Offboard wiring is standard for this pedal. See the [detailed offboard wiring instructions](https://github.com/RWLPedal/music-pcbs/instructions/WIRING.md) if you want more specifics.

## Schematic

Below is the KiCad schematic.

![Screenshot of the circuit's schematic](https://github.com/RWLPedal/music-pcbs/blob/main/HoneycreeperOverdrive/images/schematic.png?raw=true)

## Licensing

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

This PCB is released under a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.1 - Minor tweaks for symmetry, font, and legibility. Not built.
* V1.0 - First build. Verified to work.