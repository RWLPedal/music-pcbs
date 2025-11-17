# Buffalo-Weaver Overdrive

The *Buffalo-Weaver Overdrive* is a PCB based on the Guitar Magazine Tube Bender. This was a DIY circuit published by Guitar Magazine in the UK in 2003. Later, a commercial pedal was released under the Dinosaural name, with tweaked values. This PCB is printed with the original DIY values. It's a bold, crunchy-sounding overdrive.

The name from this pedal comes from the [Buffalo-Weaver](https://ebird.org/species/rbbwea1) (there are a few species). These African birds weave huge, elaborate nests with multiple compartments in baobab trees. In other words, they bend tubes!

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/BuffaloWeaverOverdrive/gerber.zip) for fabrication.

## Bill of materials

| References  | Value  | Type                   | Note                |
| :---------- | :----- | :--------------------- | :------------------ |
| C1          | 10N    | Film Capacitor         |                     |
| C5          | 10N    | Film Capacitor         |                     |
| C8          | 10N    | Film Capacitor         |                     |
| C4          | 100N   | Film Capacitor         |                     |
| C100        | 100N   | Film Capacitor         |                     |
| C2          | 47N    | Film Capacitor         |                     |
| C3          | 47U    | Electrolytic capacitor |                     |
| C6          | 4N7    | Film Capacitor         |                     |
| C7          | 33N    | Film Capacitor         |                     |
| C101        | 100U   | Electrolytic capacitor |                     |
| R8          | 22K    | 1/4W Resistor          |                     |
| R10         | 22K    | 1/4W Resistor          |                     |
| R12         | 22K    | 1/4W Resistor          |                     |
| R13         | 22K    | 1/4W Resistor          |                     |
| R1          | 1K2    | 1/4W Resistor          |                     |
| R5          | 1K2    | 1/4W Resistor          |                     |
| R7          | 1K2    | 1/4W Resistor          |                     |
| R4          | 2K2    | 1/4W Resistor          |                     |
| R9          | 2K2    | 1/4W Resistor          |                     |
| R2          | 1M     | 1/4W Resistor          |                     |
| R3          | 100K   | 1/4W Resistor          |                     |
| R6          | 150R   | 1/4W Resistor          |                     |
| R11         | 10K    | 1/4W Resistor          |                     |
| R14         | 68K    | 1/4W Resistor          |                     |
| R100        | 4K7    | 1/4W Resistor          | LEDR                |
| R101        | 100R   | 1/4W Resistor          |                     |
| RPD1        | 2M2    | 1/4W Resistor          |                     |
| D100        | LED    | 3MM                    | Bypass indicator    |
| D101        | 1N5817 | Diode\_DO41-3          | Polarity Protection |
| DRIVE       | A50K   | 16MM potentiometer     |                     |
| TONE        | A50K   | 16MM potentiometer     |                     |
| VOLUME      | A50K   | 16MM potentiometer     |                     |
| Q1          | BC549C | Transistor             |                     |
| Q3          | BC549C | Transistor             |                     |
| Q4          | BC549C | Transistor             |                     |
| Q2          | BC307B | Transistor             | See below           |
| TONE\_SHIFT | SPDT   | On/Off/On              |                     |

I was unable to source a BC307B, but you can us a 2N3906. The pins are reversed, so simply flip the transistor.

If you want, an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/OverdriveFuzz/BuffaloWeaverOverdrive/interactive_bom.html) is also available.

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

This pedal uses a [three-knob with switch layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md).

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

* V1.1 - First public version. Verified to work. Slight changes to traces after verifcation to make populating the board easier. 
* V1.0 - First version. Some mistakes in traces and transistor orientation on the print. Worked with adaptations.