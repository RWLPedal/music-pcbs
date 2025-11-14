# Shred-Masked Distortion

![Example front of the enclosure and gutshot](images/front_guts.png?raw=true)

The *Shred-Masked Distortion* is a PCB based on the BYOC Shredder, which is based on the Marshall Shredmaster. This isn't a metal pedal, but it does have a heavily distorted sound. It's also not high gain - it barely reaches unity gain. So all said, it's an odd beast, but a unique sound.

This layout is named after the [Red-masked Parakeet](https://ebird.org/species/rempar) purely to indulge in the fun name. This parakeet is sometimes a pet, and has been introduced in Hawaii and California, but is native to Ecuador.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/ShredMaskedDistortion/ShredMaskedDistortion.zip) for fabrication.

## Bill of materials

You can find an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/ShredMaskedDistortion/interactive_bom.html), which contains all reference numbers, component counts, and more. But it should not be neccessary for populating the pedal.

All the components for this pedal are easily sourced.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure.
* Sockets (for the ICs).
* Wire
* Solder

## Layout

This pedal uses the standard [five-knob, LED bottom](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md) layout.

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

* V1.0 - Updated, validated as working well.
* V0.9 - First version, worked ok but had some problems with the control placement and traces.