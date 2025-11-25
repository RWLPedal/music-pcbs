# Red-winged Overdrive

The *Red-winged Overdrive* is a PCB based on the ElectroHarmonix Hot Tubes, an early CMOS-based overdrive. All components should be easy to source, though note there's a few capacitor and resistor values which are less common. The Red-winged Overdrive is a versatile, warm, tube-sounding overdrive.

The name for the pedal comes from the color scheme of the Hot Tubes: red and black. It's named for the [Red-winged Blackbird](https://ebird.org/species/rewbla), a medium-sized black bird with bright red and yellow epaulets, common across North America (typically in swamps and wetlands). Black-birds have a distinctive mechanical clockwork song.

If you'd like to just get started with the build, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/OverdriveFuzz/RedwingedOverdrive/gerber.zip) for fabrication.

## Bill of materials

| References    | Value    | Description | Note                |
| :------------ | :------- | :---------- | :------------------ |
| C1            | 100N     |             |                     |
| C2            | 180P     |             |                     |
| C3            | 4U7      |             |                     |
| C4            | 47P      |             |                     |
| C5            | 100N     |             |                     |
| C6            | 27P      |             |                     |
| C7            | 150N     |             |                     |
| C8            | 10U      |             |                     |
| C9            | 120N     |             |                     |
| C10           | 120N     |             |                     |
| C11           | 220N     |             |                     |
| C12           | 4U7      |             |                     |
| C13           | 220N     |             |                     |
| C14           | 4U7      |             |                     |
| C100          | 100N     |             |                     |
| C101          | 220U     |             |                     |
| C102          | 47U      |             |                     |
| C103          | 47U      |             |                     |
| D100          | LED      |             | Bypass Indicator    |
| D101          | 1N5817   |             | Polarity Protection |
| R1            | 120K     |             |                     |
| R2            | 20K      |             |                     |
| R3            | 20K      |             |                     |
| R4            | 75K      |             |                     |
| R5            | 8K2      |             |                     |
| R6            | 1M8      |             |                     |
| R7            | 150K     |             |                     |
| R8            | 2M2      |             |                     |
| R9            | 200K     |             |                     |
| R10           | 5K6      |             |                     |
| R11           | 1K2      |             |                     |
| R12           | 150K     |             |                     |
| R13           | 1M       |             |                     |
| R14           | 47K      |             |                     |
| R15           | 430K     |             |                     |
| R16           | 1M       |             |                     |
| R17           | 47K      |             |                     |
| R18           | 150R     |             |                     |
| R100          | 4K7      |             | LEDR                |
| R101          | 100R     |             |                     |
| R102          | 220K     |             |                     |
| R103          | 220K     |             |                     |
| RPD1          | 1M       |             |                     |
| U2            | CD4049   |             |                     |
| U3            | RC4558   |             |                     |
| TONE1         | B10K     |             |                     |
| DRIVE1        | C1M      |             |                     |
| VOL1          | A10K     |             |                     |
| TONE\_BYPASS1 | SW\_SPDT |             |                     |

You may want to take a look at the [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/OverdriveFuzz/RedwingedOverdrive/interactive_bom.html).

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure
* Sockets (for the ICs).
* Wire
* Solder

## Layout

This pedal follows the drill conventions for the 
[125B Three-Knob with Switch layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md).

### Screenshots

Here are the front and back with traces and component values:

![Screenshot of the front of the PCB](https://github.com/RWLPedal/music-pcbs/blob/main/RedwingedOverdrive/images/pcb_front.png?raw=true)

![Screenshot of the back of the PCB](https://github.com/RWLPedal/music-pcbs/blob/main/RedwingedOverdrive/images/pcb_back.png?raw=true)

Here is the front of the PCB with references rather than values:

![Screenshot of the front of the PCB with references](https://github.com/RWLPedal/music-pcbs/blob/main/RedwingedOverdrive/images/pcb_references.png?raw=true)

### Offboard wiring

Offboard wiring is standard for this pedal. See the [detailed offboard wiring instructions](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/WIRING.md) if you want more specifics.

## Schematic

Below is the KiCad schematic.

![Screenshot of the circuit's schematic](https://github.com/RWLPedal/music-pcbs/blob/main/RedwingedOverdrive/images/schematic.png?raw=true)

## Licensing

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

This PCB is released under a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.0 - Minor text changes and trace tweaks to tidy up the board.
* V0.9 - First build. Verified as working.