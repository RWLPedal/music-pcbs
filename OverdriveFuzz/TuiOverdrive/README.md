# Tui Overdrive

![A Tui logo](images/logo.png)

The *Tui Overdrive* is a PCB based on the [Runoff Groove Supreaux Deux](https://www.runoffgroove.com/sd.html). This is a really wonderful tube-style JFET overdrive based on the Supro brand of tube amps. The circuit is the basis for popular pedals like the JHS Superbolt.

The name from this pedal comes from the [Tui](https://ebird.org/species/tui1), a ubiquitous nectar-eating bird from New Zealand. This bird makes a huge range of sounds and has a distinctive white neck tuft. They're cool birds that seem to fit the "smart, noisy black mid-sized bird" niche in NZ (like grackles or crows in parts of the US). I selected this bird for the pedal because the Supreaux Deux has "two" in the name... and so does the "Tui"!

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/TuiOverdrive/TuiOverdrive.zip) for fabrication.

## Bill of materials

| References | Value   | Type                   | Notes         |
| :--------- | :------ | :--------------------- | :------------ |
| C1         | 270P    | MLCC Capacitor         |               |
| C2         | 470P    | MLCC Capacitor         |               |
| C3         | 2N2     | Film Capacitor         |               |
| C4         | 1N5     | Film Capacitor         |               |
| C5         | 4N7     | Film Capacitor         |               |
| C6         | 1N5     | Film Capacitor         |               |
| C7         | 68N     | Film Capacitor         |               |
| C8         | 2N2     | Film Capacitor         |               |
| C9         | 470P    | MLCC Capacitor         |               |
| C100       | 100U    | Electrolytic Capacitor |               |
| C102       | 10U     | Electrolytic Capacitor |               |
| C103       | 10U     | Electrolytic Capacitor |               |
| C104       | 100N    | Film Capacitor         |               |
| D100       | LED     | 3mm LED                | Indicator LED |
| D101       | 1N5817  | Schottky Diode         |               |
| D102       | 1N5817  | Schottky Diode         |               |
| D103       | 1N5817  | Schottky Diode         |               |
| Q1         | 2N5457  | Transistor             |               |
| Q2         | J201    | Transistor             |               |
| Q3         | 2N5457  | Transistor             |               |
| R1         | 1M      | 1/4" Resistor          |               |
| R2         | 100K    | 1/4" Resistor          |               |
| R3         | 390R    | 1/4" Resistor          |               |
| R4         | 56K     | 1/4" Resistor          |               |
| R5         | 1K      | 1/4" Resistor          |               |
| R6         | 100K    | 1/4" Resistor          |               |
| R7         | 1M      | 1/4" Resistor          |               |
| R8         | 390R    | 1/4" Resistor          |               |
| R9         | 22K     | 1/4" Resistor          |               |
| R10        | 1M      | 1/4" Resistor          |               |
| R100       | 4K7     | 1/4" Resistor          | LEDR          |
| R101       | 10R     | 1/4" Resistor          |               |
| RV1        | 10K     | Trim Pot               |               |
| RV2        | 50K     | Trim Pot               |               |
| RV3        | 10K     | Trim Pot               |               |
| BOTTOM     | SPST    | Switch                 |               |
| U1         | LTC1044 | IC                     |               |
| GAIN       | A500K   | 16mm Potentiometer     |               |
| TONE       | A500K   | 16mm Potentiometer     |               |
| VOLUME     | A100K   | 16mm Potentiometer     |               |


All of the parts in this build should be easily sourced. It can be hard or expensive to source through-hole J201s or 2N5457, so there are SMD pads, which you can use instead of the through-hole option.

If you want, an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/TuiOverdrive/interactive_bom.html) is also available if you want the option of sorting components or highlighting them on the board.

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
[125B Three-Knob, with Switch layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md) - but in this case, the switch is on the right side of the pedal.

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

* V1.0 - Minor tweaks to rearrange a few traces for better spacing. Added Tui logo and moved some silkscreen elements. Not verified.
* V0.9 - First version. Verified, sounds great.