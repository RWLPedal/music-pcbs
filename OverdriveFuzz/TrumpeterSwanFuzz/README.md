# Trumpeter Swan Fuzz

![Trumpeter logo](images/logo.png)

The *Trumpeter Swan Fuzz* is a PCB based on the Paul Trombetta Mini-Bone. It's a great-sounding fuzz, with a peculiar property: with certain settings, it sounds quite "brassy" - almost like a trombone or trumpet. In particular, to my ears, it sounds like trumpet with a raspy growl. It's quite a nice pedal with a lot of variety, and it packs that all into a limited number of components.

The pedal's name comes from the brass reference. There are a few 'trumpeting' birds, of which the [Trumpeter Swan](https://en.wikipedia.org/wiki/Trumpeter_swan) is the most well-known.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/OverdriveFuzz/TrumpeterSwanFuzz/TrumpeterSwanFuzz.zip) for fabrication.

## Bill of materials

There are no components of this pedal that are particularly hard to source.

If you want, an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/OverdriveFuzz/TrumpeterSwanFuzz/interactive_bom.html) is also available if you want the option of sorting components or highlighting them on the board.

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

This pedal uses a [six-knob layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md), but the bottom left and bottom right knobs are actually toggle switches. The bypass indicator LED is at the bototm of the board.

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

* V1.0 - Silkscreen to implement version number.
* V0.9 - First version, works well and boxed up.