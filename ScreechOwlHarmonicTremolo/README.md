# Screech Owl Harmonic Tremolo

The *Screech Owl Harmonic Tremolo* is a PCB based on the Skidmark Pedals Equanimity. This is a very smooth-sounding harmonic tremolo. The effect can be quite intense but when dialed down to toned down to low rate and depth, it has a subtle, warm, lush tone. I like it much more than a regular tremolo.

Skidmark Pedals was the company founded by pedal designer Cees van Eijk, who passed away in spring 2024. Cees wrote a message to be shared posthumously: "*You are all free to use the schematics as posted in the files section, but I would appreciate if you at least would give me some credits. That my designs will live after I have passed, somehow gives me great comfort.*" It's in the spirit of that message that I share this PCB. Thankfully, build docs for the Equanimity were saved on some people's hard drives, and posted on the PedalPCB forums - thanks to forum member Blooze for sharing documentation.

The name from this pedal comes from the [Screech Owl](https://www.allaboutbirds.org/guide/Western_Screech-Owl/overview). This cute, angry-looking little owl is known for its call, which supposedly sounds like a ping-pong ball bouncing on a table (a series of quickly repeated calls that get closer over time). You can hear it at the link above. I figured this sounded a bit like a tremolo (just a bit)! Plus - the name is funny for a such a smooth-sounding pedal.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/ScreechOwlHarmonicTremolo/gerber.zip) for fabrication.

## Bill of materials


| References | Value    | Footprint              | Notes               |
| :--------- | :------- | :--------------------- | :------------------ |
| C1         | 47N      | Film Capacitor         |                     |
| C2         | 100N     | Film Capacitor         |                     |
| C3         | 4N7      | Film Capacitor         |                     |
| C4         | 4N7      | Film Capacitor         |                     |
| C5         | 100N     | Film Capacitor         |                     |
| C6         | 100N     | Film Capacitor         |                     |
| C7         | 10N      | Film Capacitor         |                     |
| C8         | 10N      | Film Capacitor         |                     |
| C9         | 100N     | Film Capacitor         |                     |
| C10        | 470P     | MLCC Capacitor         |                     |
| C11        | 22N      | Film Capacitor         |                     |
| C12        | 100N     | Film Capacitor         |                     |
| C13        | 1U       | Film Capacitor         |                     |
| C14        | 1U       | Film Capacitor         |                     |
| C15        | 1U       | Film Capacitor         |                     |
| C16        | 1U       | Film Capacitor         |                     |
| C17        | 470N     | Film Capacitor         |                     |
| C18        | 470N     | Film Capacitor         |                     |
| C100       | 100U     | Electrolytic Capacitor |                     |
| C101       | 100N     | Film Capacitor         |                     |
| C102       | 22U      | Electrolytic Capacitor |                     |
| C103       | 47U      | Electrolytic Capacitor |                     |
| D100       | LED      | 3MM LED                | Bypass indicator    |
| D101       | 1N5817   | Diode                  | Polarity Protection |
| D102       | 1N5817   | Diode                  |                     |
| Q1         | 2N3904   | Transistor             |                     |
| Q2         | 2N3904   | Transistor             |                     |
| Q3         | 2N3904   | Transistor             |                     |
| Q4         | 2N5088   | Transistor             |                     |
| Q5         | 2N5088   | Transistor             |                     |
| Q6         | 2N5088   | Transistor             |                     |
| Q7         | 2N5088   | Transistor             |                     |
| R1         | 1M       | 1/4W Resistor          |                     |
| R2         | 1M       | 1/4W Resistor          |                     |
| R3         | 47K      | 1/4W Resistor          |                     |
| R4         | 47K      | 1/4W Resistor          |                     |
| R5         | 680K     | 1/4W Resistor          |                     |
| R6         | 150K     | 1/4W Resistor          |                     |
| R7         | 2K7      | 1/4W Resistor          |                     |
| R8         | 150R     | 1/4W Resistor          |                     |
| R9         | 1K2      | 1/4W Resistor          |                     |
| R10        | 22K      | 1/4W Resistor          |                     |
| R11        | 27K      | 1/4W Resistor          |                     |
| R12        | 68K      | 1/4W Resistor          |                     |
| R13        | 680K     | 1/4W Resistor          |                     |
| R14        | 150K     | 1/4W Resistor          |                     |
| R15        | 150R     | 1/4W Resistor          |                     |
| R16        | 1K2      | 1/4W Resistor          |                     |
| R17        | 1K8      | 1/4W Resistor          |                     |
| R18        | 22K      | 1/4W Resistor          |                     |
| R19        | 10K      | 1/4W Resistor          |                     |
| R20        | 10K      | 1/4W Resistor          |                     |
| R21        | 4K7      | 1/4W Resistor          |                     |
| R22        | 100K     | 1/4W Resistor          |                     |
| R23        | 1M       | 1/4W Resistor          |                     |
| R25        | 10K      | 1/4W Resistor          |                     |
| R26        | 4K7      | 1/4W Resistor          |                     |
| R27        | 33K      | 1/4W Resistor          |                     |
| R28        | 6K2      | 1/4W Resistor          |                     |
| R29        | 2M4      | 1/4W Resistor          |                     |
| R30        | 18K      | 1/4W Resistor          |                     |
| R31        | 100K     | 1/4W Resistor          |                     |
| R32        | 100K     | 1/4W Resistor          |                     |
| R33        | 1M       | 1/4W Resistor          |                     |
| R34        | 10K      | 1/4W Resistor          |                     |
| R35        | 10K      | 1/4W Resistor          |                     |
| R36        | 12K      | 1/4W Resistor          |                     |
| R37        | 2K       | 1/4W Resistor          |                     |
| R100       | 4K7      | 1/4W Resistor          | LEDR                |
| R101       | 47K      | 1/4W Resistor          |                     |
| R102       | 47K      | 1/4W Resistor          |                     |
| R103       | 33R      | 1/4W Resistor          |                     |
| RANGE      | SW\_SPDT | SPDT ON/ON             |                     |
| DEPTH      | B1M      | 16mm Potentiometer     |                     |
| GAIN       | B100K    | 16mm Potentiometer     |                     |
| RATE       | B50K     | 16mm Potentiometer     |                     |
| U1         | TL072    | IC                     |                     |

All of the parts in this build should be easily sourced.

There are a number of components, so if you want, an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/ScreechOwlHarmonicTremolo/interactive_bom.html) is also available.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure.
* Sockets (for the IC and diodes).
* Wire
* Solder

## Layout

This pedal uses a [three-knob with switch layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md), but the switch is on the right side of the pedal rather than the left.

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

* V1.0 - First public version. Small tweaks to cap positioning for more breathing room, updated version number.
* V0.9 - First version. Verified, works well, but 1UF film caps are too tightly clustered.