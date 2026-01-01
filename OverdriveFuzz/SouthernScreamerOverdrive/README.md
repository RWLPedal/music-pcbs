# Southern Screamer Overdrive

The *Southern Screamer Overdrive* is a PCB based on the iconic Ibanez Tube Screamer, probably one of the most popular pedals and the parent of an enormous family of boutique overdrives.

The pedal is named after the [southern screamer](https://en.wikipedia.org/wiki/Southern_screamer), a goofy-looking bird with a distinctive screaming call. I think the selection of this bird as the inspiration for this board is obvious!

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/OverdriveFuzz/SouthernScreamerOverdrive/SouthernScreamerOverdrive.zip) for fabrication.

## Bill of materials

You can find an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/OverdriveFuzz/SouthernScreamerOverdrive/interactive_bom.html), which contains all reference numbers, component counts, and more. But it should not be necessary for populating the pedal.

### Circuit notes

I haven't traced this circuit myself, and there are a variety of traces available online, all of them subtly different. My impression is that few of the differences is significant enough to overall change the tone of the pedal, and I went with a "consensus" circuit.

Note that there are two components that are somewhat uncommon: the tone potentiometer is an unusual taper, W20K. And the transistors, 2SC1815, are not widely used in other pedals. The transistor pins are labeled on this pedal, and you could experiment and substitute other NPN transistors, checking the pinout. I've successfully tried using a 2N5088.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure.
* Sockets (for the transistors and IC).
* Wire
* Solder

## Layout

This pedal uses the standard layout [3-knob layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md).

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

* V1.1 - Validated and works well.