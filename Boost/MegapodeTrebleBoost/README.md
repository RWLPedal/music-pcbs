# Megapode Treble Boost

The *Megapode Treble Boost* is a PCB based on the [RunOffGroove Omega](https://www.runoffgroove.com/omega.html). It's a treble booster, intended to be an improved version of the Dallas Rangemaster.

The name from this pedal is should be obvious - the [Megapode](https://en.wikipedia.org/wiki/Megapode) are a family of birds similar to woodfowl or swamp hens, with lage feet and legs. So why not an OMegapode pedal?

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/Boost/MegapodeTrebleBoost/Songifier.zip) for fabrication.

## Bill of materials

All of the parts in this build should be easily sourced, although it can be hard to find 2N5457 through-hole transistors, so a surface mount option is provided.

This is a very simple build, but an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/Boost/MegapodeTrebleBoost/interactive_bom.html) is available.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure.
* Socket (for the transistors).
* Wire
* Solder

## Layout

This pedal uses the standard [two knob](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md) layout.

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

As with the RunOffGroove layout, this layout is licensed with a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.0 - First public version. Tweaked edges, moved potentiometers, adjusted a few traces and silkscreen.
* V0.9 - First version. Verified, works well, but potentiometers were mispositioned by 4mm.