# Dirty Bird Fuzz

The *Dirty Bird Fuzz* is a PCB based on the Skidmark Pedals Dirtbag BC108 (MK2). This in turn is a variation of the Skreddy Lunar Module with a different voicing and some bonus features. While the Dirtbag was laid out for 1590BB, this version fits into a 125B. There are no boutique parts for this pedal.

The name of this layout doesn't come from a particular bird, but I named it for the "dirty bird," a nickname for the 98 Atlanta Falcons touchdown celebration dance. So I suppose the dirty bird is a falcon. It seemed like a good fit for the "Dirtbag" pedal.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/DirtyBirdFuzz/DirtyBirdFuzz.zip) for fabrication.

## Controls

Cees van Eijk from Skidmark pedals had the following notes for the controls:

* *Unity* - Sets the gain of the first (pre drive) gain stage.
* *Gate* - Decreases the voltage for Q2 & Q3 creating a 'gating' effect.
* *Fuzz* - Sets the amount of fuzz.
* *Gain* - Sets the output level.
* *Filter* - Sets the cut-off of the low-pass filter (internal trimmer for the range).
* *Bottom* - Sets the bass response (pre-drive).
* *L-Cut* - Cuts some additional low-end (interactive with the 'Bottom' controller).
* *Boost* - Boosts the gain of the first gains tage, resulting in more drive/fuzz.

## Bill of materials

You can find an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/DirtyBirdFuzz/interactive_bom.html), which contains all reference numbers, component counts, and more. But it should not be necessary for populating the pedal.

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

This pedal does not use a standard layout. The knobs are the [6-knob layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md), but there are an additional two switches below the bottom knobs.

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

* V1.0 - V0.9 was used to test superficial changes to logos and aesthetics, which were cleaned up in this version.
* V0.9 - First version, validated and works well.