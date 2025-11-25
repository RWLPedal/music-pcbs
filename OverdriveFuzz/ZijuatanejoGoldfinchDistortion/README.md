# Zijuatanejeo Goldfinch Distortion

The *Zijuatanejo Goldfinch Distortion* is a PCB based on the Earthquaker Devices Acapulco Gold. This is an incredibly simple circuit, with just a few common components. It's an exceptionally loud distortion, moderately unruly, with a great tone.

The name for this pedal is based on the [American Goldfinch](https://en.wikipedia.org/wiki/American_goldfinch), a very common little thistle-eating bird with a range across the United States and part of Canada and Mexico. It's the state bird of New Jersey, Washington, and Iowa. In Mexico, the goldfinch has a different coloration than in the United States. Zijuatanejo is a little place in Mexico on the Pacific Ocean. It has no memory. A warm place with no memory. (Ok, that's a quote from the Shawshank Redemption). The range of the goldfinch is such that it would probably be a very rare find in Zijuatanejo, but maybe not impossible.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/OverdriveFuzz/gerber.zip) for fabrication.

## Bill of materials

All of the parts in this build should be easily sourced.

This is an exceptionally simple build, but if you want an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/OverdriveFuzz/ZijuatanejoGoldfinchDistortion/interactive_bom.html) is also available.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure. Unlike the original, it wasn't designed for a smaller enclosure.
* Sockets (for the ICs and diodes).
* Wire
* Solder

## Layout

This pedal uses the standard [125B five knob, LED bottom layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md).

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

* V1.2 - Pot moved to the top of the PCB. Verified and put in an enclosure.
* V1.1 - Worked well, but pot was positioned at the bottom of the PCB. As a result, the PCB would collide with the jacks when trying to put it in an enclosure.