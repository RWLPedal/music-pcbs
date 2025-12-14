# Bonaparte's Gull Preamp

![Bonaparte's Gull logo](images/logo.png)

The *Bonaparte's Gull Preamp* is a PCB based on Dylan159's [Bonson Praemp](https://www.freestompboxes.org/viewtopic.php?t=31229) (not a typo), which is based on the Benson Preamp.

The pcb's name comes from Bonson name; there's a distinctive smaller black-headed gull called a [Bonaparte's Gull](https://www.allaboutbirds.org/guide/Bonapartes_Gull/id). I chose this for the pedal because of the name similarity, to give gulls some representation, and because it is a pretty cool gull.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/OverdriveFuzz/BonapartesGullPreamp/BonapartesGullPreamp.zip) for fabrication.

## Bill of materials

As with other Dylan159 pedals, the rule here is component simplicity. There are no components of this pedal that are hard to source. Well, almost - the J201 transistor is pretty hard to find in through-hole format these days. For this reason, the layout uses footprints that support either a through-hole or surface mount component.

*Do note that all three electrolytic capacitors rated for 35V or above.*

If you want, an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/OverdriveFuzz/BonapartesGullPreamp/interactive_bom.html) is also available if you want the option of sorting components or highlighting them on the board.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure
* Wire
* Solder

## Layout

This pedal uses a [four-knob layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md). The bypass indicator LED is at the bottom of the board.

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

* V1.0 - Add Bonaparte's Gull logo, tweak silkscreen.
* V0.9 - First version, works well.