# Reedhaunter Delay

The *Reedhaunter Delay* is a PCB based on the Mid-Fi Clarinot, a curious delay/envelope/wah/chorus/fuzz pedal. This is a PT2399 delay with a sort of wah effect and a fuzz. It's a very unique pedal that can get quite wild and uncontrollable on certain settings. The Mid-Fi name seems to be based on the rather pleasant "woody" tone of the pedal, which does sound like a clarinet.

This layout is named after the [Reedhaunter Parakeet](https://en.wikipedia.org/wiki/Curve-billed_reedhaunter), based on the reference to a clarinet, a reed-based instrument. The pedal does also have a slightly ghostly, fractured sound. The reedhaunter is a small wren-like marshbird that's in the ovenbird family.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/Delay/ReedhaunterDelay/ReedhaunterDelay.zip) for fabrication.

## Bill of materials

You can find an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/Delay/ReedhaunterDelay/interactive_bom.html), which contains all reference numbers, component counts, and more. But it should not be neccessary for populating the pedal.

All the components for this pedal are easily sourced.

This pedal uses a homemade vactrol. You can experiment with components, but for the LED, I used a 5MM yellow LED, and for the LDR, I used a GL2258, with 10-20k light resistance. Tilt the LDR's face to touch the LED, then wrap them in electrical tape or heatshrink tape.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure.
* Sockets (for the IC).
* Wire
* Solder

## Layout

This pedal uses the [five-knob, LED bottom layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md), but the LED pad for the bypass indicator is by the other offboard wiring, making it more convenient to place at the bottom of the enclosure, not in-line with the pots (though you could place it there with some wiring).

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

* V1.0 - Updated silkscreen.
* V0.9 - First version, validated and works well.