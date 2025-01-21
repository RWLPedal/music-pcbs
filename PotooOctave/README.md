# Potoo Octave

The *Potoo Octave* is a PCB based on Fuzzhugger(fx)'s Phantom Octave, which appears to be out of production. The Potoo is a physically small octave pedal, consisting of just 15 easy-to-source components (including LEDR and bypass indicator LED). The original name refers to the fact that the octave effect changes shape and intensity according to volume, tone, picking intensity and pickups. You can get a lot of interesting tones out of this thing, from straight octave fuzz to a crunchy fuzz or relatively clean boost. It's loud and you can hear an octave effect further down the neck than many other octaves.

The name for the pedal comes from one of the most [freakish birds](https://www.youtube.com/watch?v=LkIlrNAGXQM) (and a personal favorite bird), the [Common Potoo](https://ebird.org/species/compot1), which has the nickname "Ghost Bird". Potoos are part of the frogmouth family, which also includes nightjars, but they're way weirder. Pootoos have enormous black eyes, an exceptionally wide mouth, and they're very scruffy. With eyes closed, they raise their head and are well-camouflaged as branches. With eyes open, they look more like a muppet than a bird.

If you'd like to just get started with the build, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/PotooOctave/gerber.zip) for fabrication.

## Bill of materials


| References | Value  | Description            | Note                |
| :--------- | :----- | :--------------------- | :------------------ |
| C1         | 100U   | Electrolytic capacitor |                     |
| C2         | 100N   | Film capacitor         |                     |
| C3         | 100U   | Electrolytic capacitor |                     |
| C100       | 100U   | Electrolytic capacitor |                     |
| C101       | 100N   | Film capacitor         |                     |
| R1         | 2M2    | 1/4W Resistor          |                     |
| R2         | 47K    | 1/4W Resistor          |                     |
| R100       | 4K7    | 1/4W Resistor          | LEDR                |
| D1         | 1N4148 | Diode                  |                     |
| D2         | 1N4148 | Diode                  |                     |
| D3         | LED    | LED                    | Blue 5MM            |
| D100       | LED    | Bypass indicator       |                     |
| D101       | 1N5817 | Schottky Diode         | Polarity Protection |
| U1         | LM386  | IC                     |                     |
| VOL1       | A100K  | Potentiometer          |                     |

D3 is recommended to be a 5mm blue high bright LED. Socket it and try some different options.

Note that the bypass indicator LED and LEDR are on the PCB, and are listed here in the BOM.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal will probably fit into a 1590A enclosure
* Sockets (if you want to socket the transistors).
* Wire
* Solder

## Layout

This is a single-knob pedal, so there's really no control layout. The PCB is barely larger than the footprint of a potentimeter -slightly wider, and just enough long to also fit offboard wiring and bypass LED.

### Screenshots

Here are the front and back with traces and component values:

![Screenshot of the front of the PCB](https://github.com/RWLPedal/music-pcbs/blob/main/PotooOctave/images/pcb_front.png?raw=true)

![Screenshot of the back of the PCB](https://github.com/RWLPedal/music-pcbs/blob/main/PotooOctave/images/pcb_back.png?raw=true)

Here is the front of the PCB with references rather than values:

![Screenshot of the front of the PCB with references](https://github.com/RWLPedal/music-pcbs/blob/main/PotooOctave/images/pcb_references.png?raw=true)

### Offboard wiring

Offboard wiring is standard for this pedal. See the [detailed offboard wiring instructions](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/WIRING.md) if you want more specifics.

## Schematic

Below is the KiCad schematic.

![Screenshot of the circuit's schematic](https://github.com/RWLPedal/music-pcbs/blob/main/PotooOctave/images/schematic.png?raw=true)

## Licensing

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

This PCB is released under a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.0 - First build. Verified to work. There were minor text changes after the verification.