# Ms Mallard Filter

The *Ms Mallard Filter* is a PCB based on the [Nurse Quacky](https://home-wrecker.com/nurse-quacky.html) from Homewrecker, an envelope filter. This in turn is based on the JD Sleep Dr. Q. A related pedal is the Dr. Quack. Lots of ducks here!

The pedal is named after the [mallard duck](https://www.allaboutbirds.org/guide/Mallard/id) - far and away the most ubiquitous duck in the US. I'd originally called this pedal Mr. Mallard - but male mallards don't quack, only the females do. In fact, quacking is fairly unusual for ducks. I thought this was a fun fact for the pedal.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/Filter/MsMallardFilter.zip) for fabrication.


## Bill of materials

You can find an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/Filter/MsMallardFilter/interactive_bom.html), which contains all reference numbers, component counts, and more. But it should not be necessary for populating the pedal.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure.
* Sockets (for the transistor and IC).
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

* V1.0 - Minor updates to clean up traces and update silkscreen.
* V0.9 - First version, validated and works well.