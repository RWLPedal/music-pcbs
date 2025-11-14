# Anhinga Distortion

The *Anhinga Distortion* is a PCB based on the Animal Factory Baron Samedi, itself a variation of the Jordan Bosstone. The circuit was released by the creator with an informal open license in 2014 (see details in licensing below). The original pedal was built with four knobs, but this version adds a fifth knob for additional control. The pedal has a heavy distortion/fuzz sound, but with voltage controls that allow it take on a spitty, suffocated sound. Note that it's fairly noisy.

The name for this pedal, the [Anhinga Distortion](https://www.allaboutbirds.org/guide/Anhinga/id), is based on the Anhinga, a cormorant relative that typically lives in swamps. The Baron Samedi is named after an [Iwa of Haitian Voodoo](https://en.wikipedia.org/wiki/Baron_Samedi) and I felt the swamp/bayou theme was relevant. Plus it's just a really cool bird, like a more extreme, *longer-necked* cormorant.

If you'd like to just get started with the build, you can [find the PCB on PCBWay](https://www.pcbway.com/project/shareproject/Anhinga_Distortion_1784f5dd.html) (I will receive a small commission if you order from them). Alternately, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/AnhingaDistortion/gerber.zip) for fabrication.

## Bill of materials


| References | Value  | Type                   | Notes               |
| :--------- | :----- | :--------------------- | :------------------ |
| C1         | 100N   | Film Capacitor         |                     |
| C2         | 2U2    | Electrolytic Capacitor |                     |
| C3         | 2U2    | Electrolytic Capacitor |                     |
| C4         | 220P   | MLCC Capacitor         |                     |
| C5         | 220N   | Film Capacitor         |                     |
| C100       | 2U2    | Electrolytic Capacitor |                     |
| R1         | 470K   | 1/4W Resistor          |                     |
| R2         | 1M     | 1/4W Resistor          |                     |
| R3         | 1M     | 1/4W Resistor          |                     |
| R4         | 2K2    | 1/4W Resistor          |                     |
| R5         | 1M     | 1/4W Resistor          |                     |
| R6         | 10K    | 1/4W Resistor          |                     |
| R100       | 4K7    | 1/4W Resistor          | LEDR                |
| R101       | 2M2    | 1/4W Resistor          |                     |
| R102       | 2M2    | 1/4W Resistor          |                     |
| D1         | 1N4148 | Diode                  |                     |
| D2         | 1N4148 | Diode                  |                     |
| D3         | 1N4148 | Diode                  |                     |
| D4         | 1N4148 | Diode                  |                     |
| D100       | LED    | LED                    | Bypass Indicator    |
| D101       | 1N5817 | Schottky Diode         | Polarity Protection |
| U1         | RC4558 | IC                     |                     |
| DRIVE      | A100K  | Potentiometer          |                     |
| VOLUME     | A100K  | Potentiometer          |                     |

All of the parts in this build should be easily sourced.

This is a mostly straightforward build, but if you want an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/AnhingaDistortion/interactive_bom.html) is also available.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure. Unlike the original, it wasn't designed for a smaller enclosure.
* Sockets (for the ICs and diodes).
* Wire
* Solder

## Layout

This pedal uses the standard [125B five knob, LED bottom layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md).

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

The original circuit schematic was shared with an attribution request, reproduced here:

* "Circuit free to use, modify, and distribute in any way if the information in the bottom row, website and logo are retained. If you use this for personal gain, do credit us :)"
* Schematic (c) Adity Nandwana
* Animal Factory Amplification
* Baron Samedi
* www.fuzzlov.in
* www.fbl.me/afa
* @animal_factor
* instagram.com/animalfactoryamps
* Bombay, 31/12/2014

## Versions

* V0.9 - First version, worked perfectly. Thanks to [PCBWay](https://www.pcbway.com/) for sponsoring the fabrication of the test build. You can get the exact board I fabricated [here](https://www.pcbway.com/project/shareproject/Anhinga_Distortion_1784f5dd.html).