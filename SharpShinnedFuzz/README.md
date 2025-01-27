# Sharp-Shinned Fuzz

The *King Eider Fuzz* is a PCB based on the [Effects Layouts One-Knobber](https://effectslayouts.blogspot.com/2016/06/one-knobber-project.html). This is a unique and clever circuit which can be built as 5 different pedals, depending on the components selected. This PCB supports all five layouts. You can build:

* Colorsound One Knob Fuzz
* Black Arts Toneworks Ritual Fuzz
* D.A.M. Meathead
* D.A.M. Meathead Dark
* One-knob adaptation of '66 Vox ToneBender

This layout is named after the [Sharp-Shinned Hawk](https://ebird.org/species/shshaw), a small hawk common across North America, known for its adaptability.

If you'd like to just get started with the build, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/SharpShinnedFuzz/gerber.zip) for fabrication. Note that this gerber, unlike other RWL layouts, prints with component numbers rather than values, since the values can change depending on the build you choose.

## Bill of materials

| Component Number     | 1966   | ColorSound | Dark Meathead | Meathead | Ritual  | Note                |
| :------------------- | ------ | :--------- | :------------ | :------- | :------ | :------------------ |
| R1                   | 2M     | 2M         | 2M            | 2M       | 2M      |                     |
| R2                   | 10K    | 10K        | 18K           | 18K      | 10K     |                     |
| R3                   | 1K     | 820R       | 820R          | 820R     | 820R    |                     |
| R4                   | 47K    | 150K       | 120K          | 120K     | 150K    |                     |
| R5                   | 8K2    | 2K2        | 4K7           | 4K7      | 2K      |                     |
| R6                   | 1K     | 1K         | 1K            | 1K       | 1K      |                     |
| C1                   | 220N   | 100N       | 470N          | 47N      | 680N    |                     |
| C2                   | 220P   | 220P       | 470P          | 470P     | 150P    |                     |
| C3                   | omit   | omit       | 47P           | 47P      | omit    |                     |
| C4                   | 22U    | 10U        | 10U           | 10U      | 10U     |                     |
| C5                   | 6N8    | 220N       | 100N          | 22N      | 220N    |                     |
| C6                   | 47U    | 47U        | 47U           | 47U      | 100U    |                     |
| Q1                   | BC107  | BC109      | BC107         | 2N3904   | 2N2222A | Mind pinouts        |
| Q2                   | BC108  | BC108      | BC108         | BC182    | 2N2222A | Mind pinouts        |
| Volume Potentiometer | A500K  | A500K      | A500K         | B500K    | B500K   |                     |
| R100                 | 4K7    | 4K7        | 4K7           | 4K7      | 4K7     | LEDR                |
| D100                 | LED    | LED        | LED           | LED      | LED     | Bypass Indicator    |
| D101                 | 1N5817 | 1N5817     | 1N5817        | 1N5817   | 1N5817  | Polarity Protection |

The transistors may be hard to source or expensive. You could consider replacements, just check the pinouts (which are labeled on the board):

* BC107 -> BC547, BC549, 2N3904
* 2N2222A -> PN2222A

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal can likely fit into a 1590A enclosure, since the board is barely larger than a single knob.
* Sockets (for the ICs).
* Wire
* Solder

## Layout

There's no recommended layout for this pedal, since it has a single knob. You're on your own here :).

### Screenshots

Here are the front and back with reference numbers:

![Screenshot of the front of the PCB with references](images/pcb_references.png?raw=true)

![Screenshot of the back of the PCB](images/pcb_back.png?raw=true)

### Offboard wiring

Offboard wiring is standard for this pedal, even though it's smaller than usual. See the [detailed offboard wiring instructions](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/WIRING.md) if you want more specifics.

## Schematic

Below is the KiCad schematic.

![Screenshot of the circuit's schematic](images/schematic.png?raw=true)

## Licensing

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

This PCB is released under a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.2 - Tweaked text and reordered capacitors/resistors for cleanliness.
* V1.1 - Fixed pot, updated layout, verified as working.
* V1.0 - First version, verified as working, but pot pinout inverted (turning CCW increases fuzz).