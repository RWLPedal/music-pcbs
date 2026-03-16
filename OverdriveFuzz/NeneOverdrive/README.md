# Nene Overdrive

The *Nene Overdrive* is a PCB based on the RunOffGroove [Ube Screamer](https://www.runoffgroove.com/ubescreamer.html). It's a variation of the Tube Screamer, but rather than clipping diodes it uses a CD4049 UBE. It's a fun, relatively straightforward circuit with few parts.

The name for this pedal is based on the [Nene](https://en.wikipedia.org/wiki/Nene_(bird)), the state bird of Hawai'i. This is a very rare goose - it was critically endangered and the population was as low as *30 birds* before rehabilitation efforts increased their number 100x - there are now about 3k of them. This name for the layout was selected as a reference to the Ube in the original name - a type of yam common on Pacific islands where the Nene live.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/OverdriveFuzz/NeneOverdrive/NeneOverdrive.zip) for fabrication.

## Bill of materials

All of the parts in this build should be easily sourced. An [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/OverdriveFuzz/NeneOverdrive/interactive_bom.html) is also available.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure. Unlike the original, it wasn't designed for a smaller enclosure.
* Sockets (for the IC).
* Wire
* Solder

## Layout

This pedal uses the standard [125B four knob layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md).

### Screenshots

Here are the front and back with traces and component values:

![Screenshot of the front of the PCB](images/pcb_front.png?raw=true)

![Screenshot of the back of the PCB](images/pcb_back.png?raw=true)

Here is the front of the PCB with references rather than values:

![Screenshot of the front of the PCB with references](images/pcb_references.png?raw=true)

### Offboard wiring

Offboard wiring is standard for this pedal. See the [detailed offboard wiring instructions](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/WIRING.md) if you want more specifics.

## Schematic

Below is the schematic for this pedal.

![Screenshot of the circuit's schematic](images/schematic.png?raw=true)

## Licensing

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

This layout is licensed with a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.0 - Fixed pot positions and added missing silkscreens. Tweaked component positions to match new pot positions.
* V0.9 - Validated, but pot locations were positioned for 6-knob layout. Also silkscreen was missing for power connections.