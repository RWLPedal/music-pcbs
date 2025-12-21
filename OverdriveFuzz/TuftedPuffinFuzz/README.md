# Tufted Puffin Fuzz

The *Magpie Overdrive* is a PCB based on Dylan159's [Bigger Muff](https://www.freestompboxes.org/viewtopic.php?t=31259), a simplified version of Big Muff that uses opamps but sounds more like the original Big Muff than an OpAmp Big Muff.

The pedal's name is an obvious play on the Big Muff; the [Tufted Puffin](https://en.wikipedia.org/wiki/Tufted_puffin) is largest of the puffin family.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/OverdriveFuzz/TuftedPuffinFuzz/TuftedPuffinFuzz.zip) for fabrication.

## Bill of materials

As with other Dylan159 pedals, the rule here is a limited number of components, and all of them easily obtainable. There are no components of this pedal that are hard to source.

If you want, an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/OverdriveFuzz/TuftedPuffinFuzz/interactive_bom.html) is also available if you want the option of sorting components or highlighting them on the board.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure.
* Sockets (for the IC and transistors).
* Wire
* Solder

## Layout

This pedal uses a [four-knob layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md). The bypass indicator LED is at the bottom of the board.

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

As with Dylan159's schematic, this layout is licensed with a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.0 - Increment version number, but no other changes.
* V0.9 - First version, works well.