# Fledgling Phaser

The *Fledgling Phaser* is a PCB based on Dylan159's [Perfectly Usable Phaser (PUP) Litter of Four](https://bentfishbowl.wixsite.com/electronics/post/pup-a-host-of-perfectly-usable-phasers). This circuit was an attempt to build a workable phaser that didn't require maching JFETs. The result is a phaser that... sounds like a phaser, with all cheap commodity parts. Dylan159 created a number of variations (at the linked page), including a single-FET phaser, a 2-stage, 4-stage, trimless 4-stage and 6-stage. This is the regular 4-stage phaser.

The name is unfortunately fairly dull. Since the original is called a "PUP," this is named for the bird equivalent. What can I say, I thought it was clever at the time.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/FledglingPhaser/gerber.zip) for fabrication.

## Bill of materials

| References | Value    | Type                   | Notes               |
| :--------- | :------- | :--------------------- | :------------------ |
| C1         | 100N     | Film Capacitor         |                     |
| C2         | 47N      | Film Capacitor         |                     |
| C3         | 47N      | Film Capacitor         |                     |
| C4         | 1U       | Film Capacitor         |                     |
| C5         | 47N      | Film Capacitor         |                     |
| C6         | 47N      | Film Capacitor         |                     |
| C7         | 100U     | Electrolytic Capacitor |                     |
| C8         | 47N      | Film Capacitor         |                     |
| C9         | 100U     | Electrolytic Capacitor |                     |
| C10        | 10U      | Electrolytic Capacitor |                     |
| D1         | 1N5817   | Diode                  | Polarity protection |
| D3         | LED      | LED                    | Bypass indicator    |
| R1         | 33K      | 1/4W Resistor          |                     |
| R2         | 47K      | 1/4W Resistor          |                     |
| R3         | 1M       | 1/4W Resistor          |                     |
| R4         | 10K      | 1/4W Resistor          |                     |
| R5         | 10K      | 1/4W Resistor          |                     |
| R6         | 1M       | 1/4W Resistor          |                     |
| R7         | 10K      | 1/4W Resistor          |                     |
| R8         | 10K      | 1/4W Resistor          |                     |
| R9         | 1M       | 1/4W Resistor          |                     |
| R10        | 1M       | 1/4W Resistor          |                     |
| R11        | 100K     | 1/4W Resistor          |                     |
| R12        | 10K      | 1/4W Resistor          |                     |
| R13        | 10K      | 1/4W Resistor          |                     |
| R14        | 47K      | 1/4W Resistor          |                     |
| R15        | 22K      | 1/4W Resistor          |                     |
| R16        | 1M       | 1/4W Resistor          |                     |
| R17        | 10K      | 1/4W Resistor          |                     |
| R18        | 10K      | 1/4W Resistor          |                     |
| R19        | 1M       | 1/4W Resistor          |                     |
| R20        | 10K      | 1/4W Resistor          |                     |
| R21        | 10K      | 1/4W Resistor          |                     |
| R22        | 10K      | 1/4W Resistor          |                     |
| R23        | 1M       | 1/4W Resistor          |                     |
| R24        | 1M       | 1/4W Resistor          |                     |
| R25        | 10K      | 1/4W Resistor          |                     |
| R26        | 10K      | 1/4W Resistor          |                     |
| R27        | 1M       | 1/4W Resistor          |                     |
| R28        | 10K      | 1/4W Resistor          |                     |
| R29        | 10K      | 1/4W Resistor          |                     |
| R30        | 10K      | 1/4W Resistor          |                     |
| R31        | 1M       | 1/4W Resistor          |                     |
| R32        | 10K      | 1/4W Resistor          |                     |
| R33        | 10K      | 1/4W Resistor          |                     |
| R34        | 10K      | 1/4W Resistor          |                     |
| R35        | 10K      | 1/4W Resistor          |                     |
| R36        | 100K     | 1/4W Resistor          |                     |
| R100       | 4K7      | 1/4W Resistor          | LEDR                |
| RV1        | BIAS     | Trimpot                |                     |
| RV2        | RATE     | Potentiometer          |                     |
| SW1        | FEEDBACK | SPDT ON/ON Switch      |                     |
| U1         | TL074    | IC                     |                     |
| U2         | CD4069   | IC                     |                     |
| U3         | TL074    | IC                     |                     |


All of the parts in this build should be easily sourced.

This is a mostly straightforward build, but if you want an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/Phaser/FledglingPhaser/interactive_bom.html) is also available.

### Layout note

The control layout for this pedal was awkward (a single knob and switch), and I opted to use the same layout as you'd find for two potentiometers. But with a switch in place a potentiometer, the layout is slightly higher and may interfere with audio jacks. I built this with a [bulkier enclosed jack](https://stompboxparts.com/audio-jacks/1-4-ts-enclosed-jack-panel-mount-skinny-lug/) and it just barely fit over the lugs of the switch. You may opt instead for a [less enclosed](https://lovemyswitches.com/1-4-mono-jack-lumberg-klbm-3/) or [completely exposed](https://lovemyswitches.com/1-4-mono-jack-neutrik-rean-nys229/) jack, which I expect would be less likely to touch the board.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure.
* Sockets (for the ICs and diodes).
* Wire
* Solder

## Layout

This pedal uses a slightly unusual [two-knob layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md), but the right knob is a toggle switch.

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

As with the original circuit, this layout is licensed with a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.1 - First public version. Verified and works well. Minor silkscreen changes after build.