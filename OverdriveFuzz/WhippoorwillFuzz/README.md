# Whippoorwill Fuzz

![Example enclosure front and gutshot](images/front_guts.png?raw=true)

The *Whippoorwill Fuzz* is a PCB based on the Dunwich Amplification Cthulhu ([circuit here](https://dirtboxlayouts.blogspot.com/2021/02/dunwich-cthulhu-fuzz-1-knob-silicon.html)). This is a cool one-knob fuzz, and its tone doesn't even out as much above the 12th fret, instead retaining fuzz characteristics.

The name from this pedal is based on [whippoorwill](https://en.wikipedia.org/wiki/Eastern_whip-poor-will), a bird with an eerie nighttime call that features in many HP Lovecraft stories (as does Cthulhu). Per wikipedia, New England suggests that whippoorwills can sense a soul departing and capture it. Whippoorwills are in the nightjar family, one of my favorite familites of birds because they're just so weird looking.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/OverdriveFuzz/WhippoorwillFuzz/WhippoorwillFuzz.zip) for fabrication.

Note that there are substantial differences in the layout between V1.0 and V1.1, although the circuit is the same.

## Bill of materials

| References | Value  | Type                   | Notes            |
| :--------- | :----- | :--------------------- | :--------------- |
| C1         | 15N    | Film Capacitor         |                  |
| C2         | 15N    | Film Capacitor         |                  |
| C3         | 820P   | MLCC Capacitor         |                  |
| C4         | 10U    | Electrolytic Capacitor |                  |
| C5         | 100N   | Film Capacitor         |                  |
| C6         | 100N   | Film Capacitor         |                  |
| C7         | 470P   | MLCC Capacitor         |                  |
| C8         | 1U     | Film Capacitor         |                  |
| C100       | 100U   | Electrolytic Capacitor |                  |
| R1         | 1M     | 1/4W Resistor          |                  |
| R2         | 27K    | 1/4W Resistor          |                  |
| R3         | 100K   | 1/4W Resistor          |                  |
| R4         | 1K     | 1/4W Resistor          |                  |
| R5         | 845R   | 1/4W Resistor          |                  |
| R6         | 5K1    | 1/4W Resistor          |                  |
| R7         | 33K    | 1/4W Resistor          |                  |
| R8         | 100K   | 1/4W Resistor          |                  |
| R9         | 470K   | 1/4W Resistor          |                  |
| R10        | 15K    | 1/4W Resistor          |                  |
| R11        | 100R   | 1/4W Resistor          |                  |
| R100       | 4K7    | 1/4W Resistor          | LEDR             |
| D1         | LED    | Red LED                |                  |
| D2         | 1N4148 | Diode                  |                  |
| D100       | 1N5817 | Schottky Diode         | LEDR             |
| D101       | LED    | LED                    | Bypass Indicator |
| Q1         | PN2222 | NPN Transistor         |                  |
| Q2         | PN2222 | NPN Transistor         |                  |
| Q3         | BS170  | Mosfet Transistor      |                  |
| Q4         | 2N5008 | NPN Transistor         | Or 2N3904        |
| VOLUME     | A100K  | 16mm potentiometer     |                  |

There is one hard-to-source part in this build, the 2N5008. I couldn't find it anywhere and saw a recommendation to instead try a 2N4123, which works OK. The ubiquitous 2N5088 and 2N3904 also work. My personal preference among these three was the 2N3904, but they all sound similar. I can't compare with the 2N5008, which I couldn't source.

If you want, an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/OverdriveFuzz/WhippoorwillFuzz/interactive_bom.html) is also available if you want the option of sorting components or highlighting them on the board.

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

This pedal only has one knob, so there's no established drilling layout.

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

* V1.1 - Completely changed the layout, but kept the circuit. Pushed the potentiometer to the top of the board, to allow space for the power jack to fit with the potentiometer high in the enclosure.
* V1.0 - Tweak one trace and increment silkscreen version number for initial release.
* V0.9 - First version, works fine.