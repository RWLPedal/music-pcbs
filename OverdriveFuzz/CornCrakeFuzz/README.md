# Corn Crake Fuzz

The *Corn Crake Fuzz* is a PCB based on the [Dylan159 NG-4 Fuzz](https://bentfishbowl.wixsite.com/electronics/post/ng-4-fuzz). This is an intense fuzz pedal with a huge amount of range. I'll say that some of the settings seem hard to use with some sputtery noise or a little static, so in that ways it's similar to a Fuzz Factory - a pedal with a lot of options that requires a little finesse. The circuit is based on the Cornish NG-3, but simplified. All the parts are easily sourced. 

The name from this pedal is based on the [Corn Crake](https://en.wikipedia.org/wiki/Corn_crake), a relatively common Eurasian bird. Just because it has "Corn" in the name. Thee corn crake is a type of rail, which tend to be shy birds that live around the edges of swamps. I have not seen a corn crake in the wild, but I believe that unlike other rails it lives in fields (particularly cornfields, giving it its name). Unfortunately, the corn crake is in decline because it lives in fields and modern farming techniques tend to destroy its nest.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/CornCrakeFuzz/CornCrakeFuzz.zip) for fabrication.

## Bill of materials

| References | Value  | Type                   | Notes               |
| :--------- | :----- | :--------------------- | :------------------ |
| C1         | 100N   | Film Capacitor         |                     |
| C2         | 100P   | MLCC Capacitor         |                     |
| C3         | 4U7    | Electrolytic Capacitor |                     |
| C4         | 220N   | Film Capacitor         |                     |
| C5         | 22U    | Electrolytic Capacitor |                     |
| C6         | 100N   | Film Capacitor         |                     |
| C7         | 4U7    | Electrolytic Capacitor |                     |
| C8         | 1N     | Film Capacitor         |                     |
| C9         | 220N   | Film Capacitor         |                     |
| C10        | 10N    | Electrolytic Capacitor |                     |
| C11        | 10N    | Electrolytic Capacitor |                     |
| C12        | 100N   | Film Capacitor         |                     |
| C13        | 4U7    | Electrolytic Capacitor |                     |
| C100       | 47U    | Electrolytic Capacitor |                     |
| C101       | 100U   | Electrolytic Capacitor |                     |
| C102       | 100U   | Electrolytic Capacitor |                     |
| D1         | 1N4148 | Diode                  |                     |
| D100       | LED    | 3mm LED                | Indicator LED       |
| D101       | 1N5817 | Diode                  | Polarity protection |
| Q1         | 2N3904 | Transistor             |                     |
| Q2         | 2N3904 | Transistor             |                     |
| R1         | 1K     | 1/4" Resistor          |                     |
| R2         | 2M2    | 1/4" Resistor          |                     |
| R3         | 3K3    | 1/4" Resistor          |                     |
| R4         | 2K2    | 1/4" Resistor          |                     |
| R5         | 150K   | 1/4" Resistor          |                     |
| R6         | 4K7    | 1/4" Resistor          |                     |
| R7         | 33K    | 1/4" Resistor          |                     |
| R8         | 1K     | 1/4" Resistor          |                     |
| R9         | 47K    | 1/4" Resistor          |                     |
| R10        | 220K   | 1/4" Resistor          |                     |
| R11        | 100K   | 1/4" Resistor          |                     |
| R12        | 33K    | 1/4" Resistor          |                     |
| R13        | 10K    | 1/4" Resistor          |                     |
| R14        | 27K    | 1/4" Resistor          |                     |
| R15        | 27K    | 1/4" Resistor          |                     |
| R16        | 100K   | 1/4" Resistor          |                     |
| R17        | 220K   | 1/4" Resistor          |                     |
| R18        | 1M     | 1/4" Resistor          |                     |
| R19        | 1K     | 1/4" Resistor          |                     |
| R100       | 4K7    | 1/4" Resistor          | LEDR                |
| R101       | 10K    | 1/4" Resistor          |                     |
| R102       | 10K    | 1/4" Resistor          |                     |
| R103       | 220R   | 1/4" Resistor          |                     |
| U1         | TL072  | IC                     |                     |
| BIAS       | B100K  | 16mm Potentiometer     |                     |
| EQ         | B100K  | 16mm Potentiometer     |                     |
| GAIN1      | A100K  | 16mm Potentiometer     |                     |
| GAIN2      | A100K  | 16mm Potentiometer     |                     |
| VOLUME     | A100K  | 16mm Potentiometer     |                     |

All of the parts in this build should be very easily sourced.

If you want, an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/OverdriveFuzz/CornCrakeFuzz/interactive_bom.html) is also available if you want the option of sorting components or highlighting them on the board.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure.
* Sockets (for the IC and transistors).
* Wire
* Solder

## Layout

This pedal follows the drill conventions for the 
[125B Five-Knob, LED Bottom layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md).

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

* V1.0 - Tweaked to rearrange a few caps.
* V0.9 - First version. Verified, worked well. One pot was a little inaccessible for soldering due to cap placement.