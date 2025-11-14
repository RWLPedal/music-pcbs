# King Eider Fuzz

<img src="images/front_guts.png?raw=true" alt="Cover image with gutshot">

The *King Eider Fuzz* is a PCB based on the Catalinbread Katzenkönig. It also has a clipping switch, as with the AionFX Poseidon. The Katzenkönig is a combination of a Tone Bender and a RAT, and it absolutely rips. The original Katzenkönig was published with a schematic licensed under Creative Commons, which this layout also uses as a license.

The name for this pedal, the [King Eider](https://ebird.org/species/kineid), is based on the Katzenkönig name - literally Cat King. So another king is approporiate. The King Eider is an arctic duck with a girthy, magnificent bill.

If you'd like to just get started with the build, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/KingEiderFuzz/gerber.zip) for fabrication.

## Bill of materials


| References | Value  | Description            | Note             |
| :--------- | :----- | :--------------------- | :--------------- |
| C1         | 68N    | Film Capacitor         |                  |
| C2         | 1N     | Film Capacitor         |                  |
| C3         | 47P    | MLCC Capacitor         |                  |
| C4         | 150N   | Film Capacitor         |                  |
| C5         | 22U    | Electrolytic Capacitor |                  |
| C6         | 10U    | Electrolytic Capacitor |                  |
| C7         | 22U    | Electrolytic Capacitor |                  |
| C8         | 4U7    | Electrolytic Capacitor |                  |
| C9         | 3N3    | Film Capacitor         |                  |
| C10        | 220N   | Film Capacitor         |                  |
| C11        | 1U     | Film Capacitor         |                  |
| C100       | 100N   | Film Capacitor         |                  |
| C101       | 100U   | Electrolytic Capacitor |                  |
| D2         | 1N914  | Diode                  |                  |
| D3         | 1N914  | Diode                  |                  |
| D4         | 1N914  | Diode                  |                  |
| D5         | 1N914  | Diode                  |                  |
| D6         | 1N914  | Diode                  |                  |
| D7         | 1N914  | Diode                  |                  |
| D8         | LED    | 3MM Red Diffused       |                  |
| D9         | LED    | 3MM Red Diffused       |                  |
| D100       | LED    | LED                    | Bypass Indicator |
| D101       | 1N5817 | Schottky Diode         |                  |
| Q1         | 2N5088 | Transistor             |                  |
| Q2         | 2N5088 | Transistor             |                  |
| Q3         | 2N5088 | Transistor             |                  |
| Q4         | 2N5088 | Transistor             |                  |
| R1         | 470K   | 1/4W Resistor          |                  |
| R2         | 100K   | 1/4W Resistor          |                  |
| R3         | 10K    | 1/4W Resistor          |                  |
| R4         | 1K     | 1/4W Resistor          |                  |
| R5         | 22K    | 1/4W Resistor          |                  |
| R6         | 1K     | 1/4W Resistor          |                  |
| R7         | 1K     | 1/4W Resistor          |                  |
| R8         | 150R   | 1/4W Resistor          |                  |
| R9         | 3K9    | 1/4W Resistor          |                  |
| R10        | 2K2    | 1/4W Resistor          |                  |
| R11        | 3K9    | 1/4W Resistor          |                  |
| R12        | 1K     | 1/4W Resistor          |                  |
| R13        | 1M     | 1/4W Resistor          |                  |
| R14        | 1M     | 1/4W Resistor          |                  |
| R15        | 3K3    | 1/4W Resistor          |                  |
| R100       | 4K7    | 1/4W Resistor          | LEDR             |
| R101       | 100R   | 1/4W Resistor          |                  |
| R102       | 1M     | 1/4W Resistor          |                  |
| CLIP1      |        | SPDT ON/OFF/ON         |                  |
| VOL1       | A100K  | Potentiometer          |                  |
| FILTER1    | A100K  | Potentiometer          |                  |
| GAIN1      | A50K   | Potentiometer          |                  |
| INPUT1     | B250K  | Potentiometer          |                  |


You may want to take a look at the [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/KingEiderFuzz/interactive_bom.html).

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

This pedal has a unique layout. Drill holes are in the same position as the [125B Five-Knob, LED Top layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md), but the bottom center potentiometer is replaced with the SPDT switch. You can use the same layout but the diameter of that hole will be 6.6mm.

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

This pedal went through a few iterations as I corrected mistakes, but it's been working from the start.

* V1.3 - Minor tweaks for ergonomics after building (moving capacitors away from pot pads, text tweaks).
* V1.2 - Moved pots, other cleanup. Verified as working. Very close to V1.3 layout.
* V1.1 - Pots in wrong location. Never built.
* V1.0 - First version, verified as working, but layout felt untidy.