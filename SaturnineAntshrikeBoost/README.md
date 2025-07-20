# Saturnine Antshrike Boost

The *Saturnine Antshrike Boost* is a PCB based on the Spaceman Saturn V, a "harmonic booster" pedal. This is a pretty standard boost pedal, with a light overdrive control. It can crank out a lot of volume. The additional control, while still offering the ability to have a clean boost, makes this my favorite boost right now. This is a build with very few components (there are probably fewer components than letters in its name!), but as with many Spaceman layouts it has a few unique components.

The name of this layout comes from the [Saturnine Antshrike](https://ebird.org/species/satant1). While the original pedal is the Saturn V, why not go with the Saturn IX for the name?! Antshrikes are bug-eating birds that can attack army ant swarms.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/SaturnineAntshrikeBoost/SaturnineAntshrikeBoost.zip) for fabrication.

## Bill of materials

You can find an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/SaturnineAntshrikeBoost/interactive_bom.html), which contains all reference numbers, component counts, and more. But it should not be neccessary for populating the pedal.

There are a few unique components for this pedal:

* There are ferrite beads. These are ostensibly noise-cancelling. I used these [76 Ohm](https://www.taydaelectronics.com/axial-ferrite-bead-76-ohm.html) beads, which are cheap. However, many people have reported omitting the beads from with no ill-effect. If you want to ignore them, just lay a jumper form one end of each bead footprint to the other.
* The transistors are LND150N3-G. These can currently be found for cheap on Mouser, but other sites may not carry them.

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

This layout is licensed with a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.0 - First version, validated and works well.