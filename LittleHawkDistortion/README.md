# Little Hawk Distortion

The *Little Hawk Distortion* is a PCB based on the Durham Crazy Horse. This is a Neil Young-inspired fuzz which can have a wild sound due to voltage starve. Without voltage starved, it's still a quite nice-sounding fuzz.

This pedal's name is inspired by Crazy Horse, the famous Lakota warrior - whose younger half brother was named Little Hawk. I pictured the species that inspires this pedal to be the [Cooper's Hawk](https://www.allaboutbirds.org/guide/Coopers_Hawk/id), a little hawk that his widespread across the United States.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/LittleHawkDistortion/LittleHawkDistortion.zip) for fabrication.

## Bill of materials

There are no components of this pedal that are particularly hard to source.

There is a clipping LED (next to the volt pot), for which I suggest using a 3mm green LED.

If you want, an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/LittleHawkDistortion/interactive_bom.html) is also available if you want the option of sorting components or highlighting them on the board.

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

This pedal uses a standard [five-knob, LED bottom layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md), although the bypass indicator LED is positioned at the bottom of the board.

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

* V1.1 - Removed the SPST and went with the original pedal's schematic. This version, which is not changed too much from V1.0, is not yet validated.
* V1.0 - Tweak to add the trace and a SPST switch, because in some settings the disconnected trace was self-muting. Validated, but found in most settings the SPST being disconnected is useless. Validated working otherwise.
* V0.9 - First version, missing a trace. Validated working with an extra wire.