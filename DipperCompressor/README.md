# Dipper Compressor ("That" Compressor)

<img src="https://github.com/RWLPedal/music-pcbs/blob/main/DipperCompressor/images/dipper_compressor.png?raw=true" alt="Cover image with gutshot" height="500px">

The *Dipper Compressor* is a PCB for [Dylan159's "That" Compressor](https://bentfishbowl.wixsite.com/electronics/post/that-compressor), a unique compressor. As with most compressors, this one is relatively subtle, but features a limited number of easy-to-obtain components, and it has low ripple or other artifacts.

Dylan159 provides vero layouts for a 3-knob and 5-knob compressor. This layout is for 5 knobs.

The Dipper name was chosen because this pedal has "low ripple." Dippers are a type of songbird which dive into running water (ostensibly without leaving much of a ripple!). They are the only diving songbird - they look similar to thrushes such as robins, but can dive. In the US West, you can see American Dippers diving into icy spring snow runoff and emerging with aquatic prey.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/DipperCompressor/gerber.zip) for fabrication.

## Bill of materials

| **References** | **Value** | **Description**        | **Notes**                                           |
| :------------- | :-------- | :--------------------- | :-------------------------------------------------- |
| C1             | 47N       | Film capacitor         |                                                     |
| C2             | 1U        | Electrolytic capacitor |                                                     |
| C3             | 1U        | Electrolytic capacitor |                                                     |
| C4             | 1U        | Electrolytic capacitor |                                                     |
| C5             | 33P       | MLCC Ceramic Capacitor |                                                     |
| C6             | 47P       | MLCC Ceramic Capacitor |                                                     |
| C7             | 10U       | Electrolytic capacitor |                                                     |
| C100           | 100U      | Electrolytic capacitor |                                                     |
| C101           | 47U       | Electrolytic capacitor |                                                     |
| C102           | 100N      | Film Capacitor         |                                                     |
| R1             | 1K        | Resistor               |                                                     |
| R2             | 1M        | Resistor               |                                                     |
| R3             | 10K       | Resistor               |                                                     |
| R4             | 10K       | Resistor               |                                                     |
| R5             | 1K        | Resistor               |                                                     |
| R6             | 47K       | Resistor               |                                                     |
| R7             | 2K2       | Resistor               |                                                     |
| R8             | LDR       | LDR                    | Dylan159 suggests "400 ohms (light) to 20M (dark)." |
| R9             | 10K       | Resistor               |                                                     |
| R10            | 330K      | Resistor               |                                                     |
| R11            | 330K      | Resistor               |                                                     |
| R12            | 2K2       | Resistor               |                                                     |
| R13            | 47K       | Resistor               |                                                     |
| R15            | 220K      | Resistor               |                                                     |
| R14            | 220K      | Resistor               |                                                     |
| R16            | 100K      | Resistor               |                                                     |
| R17            | 1K        | Resistor               |                                                     |
| R18            | 10K       | Resistor               |                                                     |
| R19            | 10K       | Resistor               |                                                     |
| R100           | 4K7       | Resistor               |                                                     |
| D1             | LED       | 5mm Red LED            | Dylan159 suggests a "5mm high brightness red LED."  |
| D2             | BAT41     | Schottky diode         |                                                     |
| D3             | BAT41     | Schottky diode         |                                                     |
| D4             | 1N4148    | Diode                  |                                                     |
| D5             | 1N4148    | Diode                  |                                                     |
| D6             | 1N5817    | Schottky diode         |                                                     |
| D100           | LED       | 3mm LED (Indicator)    |                                                     |
| U1             | LM324     | IC                     |                                                     |
| U2             | TL072     | IC                     |                                                     |
| ATTACK         | B10K      | Potentiometer          |                                                     |
| THRESHOLD      | B10K      | Potentiometer          |                                                     |
| MAKEUP         | B100K     | Potentiometer          |                                                     |
| RATIO          | B100K     | Potentiometer          |                                                     |
| DECAY          | B1M       | Potentiometer          |                                                     |

Note that the bypass indicator LED and LEDR are on the PCB, and are listed here in the BOM.

The only unusual components here are the LDR and LED, which together act as a vactrol. These are listed seperately above. I used a regular 5mm red LED for the LED, and a GL5549 for the LDR (which has 45-100k (light) - 10M (dark)), wrapped in black electrical tape, with satisfactory results - but I could perhaps audition others components. Per the [doc](https://bentfishbowl.wixsite.com/electronics/post/that-compressor), "almost any should work fine, since the low part of the resistance range isn't usually reached in practice and it's the ratio with the 'Ratio' resistancee that matters for both: as long as the dark resistance isn't lower than that, nothing bad will happen, and if ti's not, it's just a matter of make-up gain."

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Sockets (I would recommend socketing the ICs on this PCB- you will need an 8-pin DIP socket and a 14-pin DIP socket)
* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal will fit in a 125B enclosure
* Wire
* Solder

## Layout

The layout follows the PedalPCB layout conventions and positions for a "5-knob (Type 1)" pedal - which has a top row with potentiometer/LED/potentiometer, and 3 potentiometers on the bottom row. It should any enclosures drilled to match.

### Screenshots

Here are the front and back with traces and component values:

![Screenshot of the front of the PCB](https://github.com/RWLPedal/music-pcbs/blob/main/DipperCompressor/images/pcb_front.png?raw=true)

![Screenshot of the back of the PCB](https://github.com/RWLPedal/music-pcbs/blob/main/DipperCompressor/images/pcb_back.png?raw=true)

Here is the front of the PCB with references rather than values:

![Screenshot of the front of the PCB with references](https://github.com/RWLPedal/music-pcbs/blob/main/DipperCompressor/images/pcb_references.png?raw=true)

### Offboard wiring

Offboard wiring is standard for this pedal. See the [detailed offboard wiring instructions](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/WIRING.md) if you want more specifics.

## Schematic

Below is the KiCad schematic.

![Screenshot of the circuit's schematic](https://github.com/RWLPedal/music-pcbs/blob/main/DipperCompressor/images/schematic.png?raw=true)

## Licensing

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

As with the Dylan159's original schematic, this layout is licensed with a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.1 - Small touchups to positioning of components and silkscreens. First public release.
* V1.0 - Confirmed working well. Made slight tweaks to positioning and silkscreen after building. Never released.