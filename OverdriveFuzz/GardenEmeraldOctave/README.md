# Garden Emerald Octave

The *Garden Emerald Octave* is an octave fuzz PCB based on a few pedals: the famous Green Ringer, the Earthquaker Devices Tentacle, and one section of the Earthquaker Devices Sunn O))).  (You can build any of these by simply adjusting components). It's probably the most famous octave fuzz circuit.

The name for this pedal comes from the [Garden Emerald](https://ebird.org/species/gareme1), a type of hummingbird from Costa Rica, paying homage to the Green Ringer name.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/OverdriveFuzz/GardenEmeraldOctave/GardenEmeraldOctave.zip) for fabrication - with Green Ringer values printed on it. I've also provided a [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/OverdriveFuzz/GardenEmeraldOctave/GardenEmeraldOctaveReferences.zip) that contains component references printed on the board (rather than component values), to make it easier if you would like to build a variation (see the variations section below).

## Bill of materials

All of the parts in this build are easily sourced.

This is a simple build, but if you want an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/OverdriveFuzz/GardenEmeraldOctave/interactive_bom.html) is also available.

### Variations

| Component number | Green ringer value | Tentacle value |    Sunn O))) value    |
| :--------------: | :----------------: | :------------: | :-------------------: |
|        R1        |        1M5         |      2M2       |          1M           |
|        R2        |        560K        |      560K      |         470K          |
|        R3        |        160K        |      160K      |          47K          |
|        R4        |        18K         |      18K       |          22K          |
|        R5        |        6K2         |      6K2       |          2K2          |
|        R8        |        68K         |      68K       |         100K          |
|        R9        |        68K         |      68K       |         100K          |
|       R10        |        22K         |      22K       |          47K          |
|       R11        |        22K         |      22K       |          47K          |
|       R13        |        47K         |      47K       |         Omit          |
|        C1        |        47N         |      47N       |         100N          |
|        C2        |        47N         |      47N       |         100N          |
|        C3        |        47N         |      47N       |         100N          |
|        C4        |        100N        |      100N      |          1U           |
|        C5        |        Omit        |      100P      |         100P          |
|        Q1        |       2N5088       |     2N5089     |        2N5089         |
|        Q2        |       2N3906       |     2N3906     |        2N5087         |
|        Q3        |       2N5088       |     2N5089     |        2N5089         |
|        D1        |         GE         |     1N4148     | GE (wired in reverse) |
|        Q3        |         GE         |     1N4148     | GE (wired in reverse) |

The Tentacle variation has the exact same values as the Earthquaker Devices Hoof Reaper pedal. I have not personally verified the Sunn O))) values.

The green ringer has a volume control, with value A100K, which you could wire from the PCB output to pin 3 of the potentiometer, with pin 1 going to ground and pin 2 continuing on to the output on the footswitch.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure. Unlike the original, it wasn't designed for a smaller enclosure.
* Sockets (for the transistors).
* Wire
* Solder

## Layout

This pedal doesn't have any external controls at all, unless you choose to wire them in yourself.

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

* V1.0 - Silkscreen changes and some slight tweaks to get better copper fill coverage.
* V1.0 - Worked well, verified.
* V0.9 - Worked ok, wanted to make some changes.