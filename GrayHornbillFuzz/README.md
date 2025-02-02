# Gray Hornbill Fuzz

<img src="images/grayhornbill_fuzz.png?raw=true" alt="Cover image with gutshot" height="500px">

The *Gray Hornbill Fuzz* is a PCB based on a Tim Escobedo circuit fragment, the Jawari. The circuit fragment does not include a power section, but all necessary components are included on this PCB.

The Jawari is reputed to sound like a sitar, and it does - particularly on the D and G strings, between frets 0 and 12. Elsewhere on the neck, it's a solid-sounding, slightly nasally, fuzz. You'll want to play around with the tone, volume, and pickups on your guitar and the pedal. Note that this circuit is relatively quiet and barely has unity gain with the volume maxed out.

If you look at the gutshot above, you'll see that there's a separate boost board in the pedal, the [Szukalski Uggsy](https://github.com/szukalski/pedal-dylan159/tree/main/uggsy), based on the Dylan159 Boot Boost, but with a trimpot instead of a regular potentiometer. This is to give the pedal a reasonable amount of volume.

The name for this pedal, the [Gray Hornbill](https://ebird.org/species/inghor2) Fuzz, was selected because the Indian Gray Hornbill is a distinctive bird from India. This bird looks like a cross between a small dinosaur and a toucan, and is one of a number of hornbill birds.

If you'd like to just get started with the build, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/GrayHornbillFuzz/gerber.zip) for fabrication.

## Bill of materials

| References | Value   | Description            | Note             |
| :--------- | :------ | :--------------------- | :--------------- |
| C1         | 1U      | Electrolytic Capacitor |                  |
| C2         | 100N    | Film Capacitor         |                  |
| C100       | 22U     | Electrolytic Capacitor |                  |
| D1         | 1N34A   | GE Diode               |                  |
| D2         | 1N34A   | GE Diode               |                  |
| D3         | 1N4148  | Diode                  |                  |
| D100       | LED     | LED                    | Bypass indicator |
| D101       | 1N5817  | Polarity protection    |                  |
| Q1         | J201    | Transistor             |                  |
| R1         | 1M      | 1/4W Resistor          |                  |
| R2         | 1K      | 1/4W Resistor          |                  |
| R3         | 100K    | 1/4W Resistor          |                  |
| R100       | 4K7     | 1/4W Resistor          | LEDR             |
| R101       | 47R     | 1/4W Resistor          |                  |
| TR1        | 42TM018 | Transformer            |                  |
| GAIN1      | B10K    |                        |                  |
| VOLUME1    | A100K   |                        |                  |


You may want to take a look at the [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/GrayHornbillFuzz/interactive_bom.html).

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

This pedal uses the [125B Two-Knob layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md).

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

* V1.1 - Ergonomic changes: tweaked pot location, moved resistors further from transformer, silkscreen text changes.
* V1.0 - First version, verified as working.