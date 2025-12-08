# Magpie Overdrive

![Magpie logo](images/logo.png)

The *Magpie Overdrive* is a PCB based on Dylan159's [1Q81](https://www.freestompboxes.org/viewtopic.php?t=31537), in turn a version of the DRV 1981 with simplified components, *in turn* itself a RAT derivative. Wow! This is a low-gain RAT that has a nice tone.

The pedal's name comes from the 1Q81 name that Dylan159 gave the pedal - named for a Haruki Murakami book. I chose the Magpie as reference to a different Murakami book, the Wind-up Bird Chronicles (Murakami doesn't name the bird, but people speculate that it's a [Magpie](https://en.wikipedia.org/wiki/Oriental_magpie) based on the sound of the call and the geographic location.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/OverdriveFuzz/MagpieOverdrive/MagpieOverdrive.zip) for fabrication.

## Bill of materials

As with other Dylan159 pedals, the rule here is component simplicity. There are no components of this pedal that are hard to source.

If you want, an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/OverdriveFuzz/MagpieOverdrive/interactive_bom.html) is also available if you want the option of sorting components or highlighting them on the board.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure.
* Sockets (for the IC and transistor).
* Wire
* Solder

## Layout

This pedal uses a [three-knob layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md), but the bottom left and bottom right knobs are actually toggle switches. The bypass indicator LED is at the bototm of the board.

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

* V1.0 - Add Magpie logo, tweaked silkscreen, rotated one capacitor that was misoriented.
* V0.9 - First version, works well.