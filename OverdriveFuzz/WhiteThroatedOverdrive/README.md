# White-Throated Overdrive

The *White-Throated Overdrive* is a PCB based on [Dylan159's "Dudson Narrowcast,"](https://bentfishbowl.wixsite.com/electronics/post/dudson-narrowcast-v2) a redesign of the Hudson Broadcast. Notably, the redesign does not include a transformer, and uses only easy-to-obtain components and values (no OC71 transistor or 330U electrolytic capacitor). Dylan159 provides two schematics, a PNP and NPN version. This PCB is for the PNP version, and it sounds great, with a crunchy tube-like tone.

The White-Throated name for the PCB was chosen somewhat haphazardly. For those of us living in the Pacific Northwest, we are excited to see the [White-Throated Sparrow](https://ebird.org/species/whtspa), but it's very common in New York's Hudson Valley. It's a charming sparrow with a splash of yellow.

If you'd like to just get started with the build, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/OverdriveFuzz/WhiteThroatedOverdrive/gerber.zip) for fabrication.

## Bill of materials

| References | Value   | Description                            |
| :--------- | :------ | :------------------------------------- |
| C1         | 10U     | Polarized capacitor                    |
| C2         | 10U     | Polarized capacitor                    |
| C3         | 330P    | MLCC capacitor                         |
| C4         | 330P    | MLCC capacitor                         |
| C5         | 100U    | Polarized capacitor                    |
| C6         | 470N    | Film capacitor                         |
| C7         | 100U    | Polarized capacitor                    |
| C8         | 10U     | Polarized capacitor                    |
| C9         | 10U     | Polarized capacitor                    |
| C10        | 1N      | Film capacitor                         |
| C100       | 100U    | Polarized capacitor                    |
| R2         | 220K    | 1/4W Resistor                          |
| R3         | 33K     | 1/4W Resistor                          |
| R4         | 4K7     | 1/4W Resistor                          |
| R5         | 1K      | 1/4W Resistor                          |
| R6         | 470R    | 1/4W Resistor                          |
| R7         | 4K7     | 1/4W Resistor                          |
| R8         | 4K7     | 1/4W Resistor                          |
| R9         | 47R     | 1/4W Resistor                          |
| R10        | 4K7     | 1/4W Resistor                          |
| R100       | 4K7     | 1/4W Resistor                          |
| R101       | 47R     | 1/4W Resistor                          |
| D100       | LED     | Light emitting diode, bypass indicator |
| D101       | 1N5817  | Diode, polarity protection             |
| Q1         | 2N3904  | NPN Transistor                         |
| Q2         | 2N3904  | NPN Transistor                         |
| SWITCH     | SW_SPDT | Switch, SPDT ON/ON                     |
| BASS_CUT   | A10K    | Potentiometer                          |
| GAIN       | A250K   | Potentiometer                          |
| VOLUME     | A25K    | Potentiometer                          |

Note that the bypass indicator LED and LEDR are on the PCB, and are listed here in the BOM.

Dylan159 advises that:
* The BASS_CUT pot be replaced with a C10K if the pedal is set up for bass.
* The 2N3904 transistors are stand-ins, but to experiment with other NPN transistors if you'd like.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal will fit in a 125B enclosure
* Sockets (if you want to socket the transistors).
* Wire
* Solder

## Layout

This pedal follows the drill conventions for the 
[125B Three-Knob with Switch layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md).

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

This PCB is released under a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike), the same as the original Dylan159 schematic.

## Versions

* V1.0 - First build. Verified to work. There were minor font and text changes after the verification.