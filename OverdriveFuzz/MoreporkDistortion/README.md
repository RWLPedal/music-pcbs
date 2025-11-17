# Morepork Distortion

The *Morepork Distortion* is a PCB based on the MXR Distortion+. The layout is true to the original pedal.

The name for this pedal, the [Morepork](https://ebird.org/species/morepo2), comes from a small owl from New Zealand. I thought that, for a pedal based on the "Distortion Plus," plus means more - and how can you not like a bird called the Morepork?! Ad where does that name come from? The Morepork's call sounds like "Morepork," although I'd say that's a bit of a stretch.

I suspect, like many non-New Zealanders, that my first encounter with the Morepork was through Discworld's Ankh-Morpork. Which is named for the owl! The city arms have an owl on them.

I had some fun with this layout. The PCB is set up like a "+" to mirror the original circuit's name.

If you'd like to just get started with the build, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/MoreporkDistortion/gerber.zip) for fabrication.

## Bill of materials

| References | Value  | Note             |
| :--------- | :----- | :--------------- |
| C1         | 1N     |                  |
| C2         | 10N    |                  |
| C3         | 47N    |                  |
| C4         | 1U     |                  |
| C5         | 1N     |                  |
| C100       | 1U     |                  |
| R1         | 10K    |                  |
| R2         | 1M     |                  |
| R3         | 4K7    |                  |
| R4         | 1M     |                  |
| R5         | 10K    |                  |
| R100       | 4K7    | LEDR             |
| R101       | 1M     |                  |
| R102       | 1M     |                  |
| D1         | GE     | 1N270 or 1N34A   |
| D2         | GE     | 1N270 or 1N34A   |
| D100       | LED    | Bypass Indicator |
| D101       | 1N5817 |                  |
| U1         | LM741  |                  |
| DISTORTION | C500K  | Originally B1M   |
| OUTPUT     | A10K   |                  |

There is one change in the label for this circuit compared to the original, which is the DISTORTION or gain knob. Originally this knob was a linear 1M potentiometer. However, this has almost no effect through most of its travel, with the distortion suddenly appearing in the last 10% or so of its sweep. Swapping it for a reverse logarithmic taper makes it more usable. Similarly, the distortion is most noticeable for the Morepork when the resistance is low, so the full 1M sweep is not necessary. You can use B1M, C1M, C500K, C100k, or similar pots.

As for diodes, the original Distortion+ uses germanium: 1N270s. It's common on many diagrams to show 1N34A instead. You can experiment with other diodes (1N4148 is common on other pedals with the same circuit layout).

This is a simple build, but you may want to take a look at the [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/OverdriveFuzz/MoreporkDistortion/interactive_bom.html).

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure
* Sockets (for the ICs and diodes).
* Wire
* Solder

## Layout

This pedal uses the [125B Two-Knob layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md).

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

This PCB is released under a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.0 - Fixed bad pot wiring. Minor layout and silkscreen tweaks. Not verified.
* V0.9 - First version, verified as working. However, middle pin of DISTORTION pot was wired wrong. Verified working as expected with bent pin.