# Yellow-Rumped Fuzz

The *Yellow-Rumped Fuzz* is a PCB based on the Spaceman Rumblefuzz II. It's a rich fuzz with a moderately unique tone.

The pedal's name is a play on the "Rumblefuzz". While funny, "rump" is common in bird names, describing the area just above the tail. There are a number of "Yellow-Rumped" birds - I had in mind the [Yellow-Rumped Warbler](https://ebird.org/species/yerwar) when naming this pedal.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/OverdriveFuzz/YellowRumpedFuzz/YellowRumpedFuzz.zip) for fabrication.

## Bill of materials

There are a few slightly unusual components for this pedal. The ferrite beads are typical of Spaceman pedals, and you can jumper them if you don't want to follow the exact circuit. Theoretically they reduce noise; in practice few people notice a difference.

The 1N4002 diode is not typically used, but you can use other 1N400X diodes in its place (for example 1N4001 and 1N4007 are both more common).

Likewise, you can use 2N222A or PN222A interchangeably.

If you want, an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/OverdriveFuzz/YellowRumpedFuzz/interactive_bom.html) is also available if you want the option of sorting components or highlighting them on the board.

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

This pedal uses a [three-knob with switch on right layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md).

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

* V1.0 - Silkscreen adjustments.
* V0.9 - First version, works well.