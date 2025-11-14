# Tiny Tyrant PLL

The *Tiny Tyrant PLL* is a PCB based on [Dylan159's PLLedal](https://bentfishbowl.wixsite.com/electronics/post/cd4046-fun-the-plledal-and-the-hacksaw). It's a PLL pedal with a small number of component types with a limited number of values.

The name for this pedal, the [Tiny Tyrant](https://ebird.org/species/titman1), comes from the Tiny Tyrant-Manakin, a small jungle bird from South America. I've selected Manakins as a general theme for PLL-related pedals. This pedal, as with many Dylan159 designs, is relatively simple. Manakins in general are colorful birds with elaborate mating dances, although the Tiny Manakin is notably small (and a little drab) - I thought it was a good reflection of the relatively limited parts count for this pedal.

If you'd like to just get started with the build, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/TinyTyrantPll/gerber.zip) for fabrication.

## Bill of materials

| References | Value       | Notes               |
| :--------- | :---------- | :------------------ |
| C1         | 100N        |                     |
| C2         | 1U          |                     |
| C3         | 100P        |                     |
| C4         | 100N        |                     |
| C5         | 10N         |                     |
| C6         | 10N         |                     |
| C7         | 100N        |                     |
| C8         | 100N        |                     |
| C9         | 100N        |                     |
| C10        | 10U         |                     |
| C100       | 100U        |                     |
| C101       | 100U        |                     |
| R1         | 10K         |                     |
| R2         | 1M          |                     |
| R3         | 1M          |                     |
| R4         | 2K2         |                     |
| R5         | 1K          |                     |
| R6         | 22K         |                     |
| R7         | 10K         |                     |
| R8         | 10K         |                     |
| R9         | 10K         |                     |
| R10        | 10K         |                     |
| R11        | 47K         |                     |
| R12        | 1M          |                     |
| R13        | 100K        |                     |
| R14        | 10K         |                     |
| R15        | 33K         |                     |
| R16        | 100K        |                     |
| R17        | 100K        |                     |
| R18        | 220K        |                     |
| R19        | 220K        |                     |
| R20        | 100K        |                     |
| R100       | 4K7         | LEDR                |
| R101       | 10K         |                     |
| R102       | 10K         |                     |
| D1         | LED         |                     |
| D2         | LED         |                     |
| D100       | LED         | Indicator LED       |
| D101       | 1N5817      | Polarity Protection |
| LEAD\_BASS | DPDT ON/ON  |                     |
| OCTAVE     | DPDT ON/ON  |                     |
| SW4        | 1P8T Rotary |                     |
| U2         | TL072       |                     |
| U3         | LM358       |                     |
| U4         | CD4024      |                     |
| U5         | CD4046      |                     |
| U6         | CD4017      |                     |
| MIX        | B100K       |                     |
| VOLUME     | A10K        |                     |

All of the parts in this build should be easily sourced. The rotary switch is slightly unusual, see "Rotary switch" section below

This is a relatively complicated build, so you may prefer to look at the [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/TinyTyrantPll/interactive_bom.html).

### Rotary switch

The only slightly unusal component is the 1P8T rotary switch. It's designed for a 1 Pole 8 Position mini-rotary. [Here the page](https://www.taydaelectronics.com/mini-rotary-switch-1-pole-8-position-alpha-rs16211-20mm.html) on Tayda.

The rotary switch is laid out to use positions 1 through 5; positions 6, 7, and 8 will have no effect. See below for how the poles will work, per documentatoin from Dylan159.

| 1P8T Pin | CD4047 Pin | Effect                                 |
| -------- | ---------- | :------------------------------------- |
| 1        | 11         | \+maj9th with \-2 oct                  |
| 2        | 1          | maj 3rd with \-2 oct                   |
| 3        | 7          | \+p5th with \-1 oct; \-p4 with \-2 oct |
| 4        | 4          | One octave above (+oct, uni, \-oct)    |
| 5        | 2          | Input                                  |


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

This pedal uses the [125B Five-Knob, LED top layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md). The rotary switch tends to have a thicker base than a regular potentiometer (I measure mine as 8.5mm, meaning a 9mm hole is probably appropriate for drilling; typical pot holes are 7.4mm for a 7mm post).

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

As with the Dylan159's original schematic, this layout is licensed with a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.2 - Cosmetic changes and fixes to incorrect component values. Unverified, but expected to be 100% correct.
* V1.1 - Fix bad wiring and labels. Three component values wrong (R13, R101, R102). Verified as working. 
* V1.0 - First version, several problems including a few bad connections. Worked with some jumpers.