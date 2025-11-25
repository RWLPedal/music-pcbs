# Wood Owl Acoustic

The *Wood Owl Acoustic* is a PCB based on the Rockman Acoustic Guitar Pedal, which is a sort of compressor with bass and treble controls that gives an electric guitar a vaguely acoustic sound. While you may or may not find that the result sounds like an acoustic guitar, I think it *does* add a very nice resonance. This PCB was a collaboration with Cybercow (moo) on the PedalPCB forums. Cybercow traced and shared the circuit, and helped build and troubleshoot this board, including a few circuit revisions.

We chose to call this pedal the [Wood Owl](https://en.wikipedia.org/wiki/Spotted_wood_owl) - there are a few species of this owl in Southeast Asia and Africa. They're quite alien-looking birds with huge, all-black eyes. The name comes from the "wood" connection between acoustic guitars and the owls.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/Other/WoodOwlAcoustic/WoodOwlAcoustic.zip) for fabrication.

## Bill of materials

This is a very complicated pedal (about as dense a board as you can fit into a 125B enclosure), so the [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/WoodOwlAcoustic/interactive_bom.html) is recommended for viewing the list of components, sorting, or highlighting them on the board.

There are no hard-to-find components in this build, although you might find that a few of the resistor values are missing from your storage!

This build supports a few different component options. For the J201 transistor, you may use a surface-mount or through-hole design. There is a 1uF capacitor, which you can use either an electrolytic or film capacitor for (film is recommended, but a pad is labeled for the positive lead of an electrolytic capacitor - the two circular pads are interchangeable and both negative). Finally, there is a trimpot on the board and it supports both trimpot form factors, although note that it's oriented upside-down compared to a typical trimpot.

### Adjusting the trimpot

Set the gain control fully counter-clockwise, and the other controls at 50%. Adjust the trimmer while using the pedal until you can detect a slight bit of compression on the attack transient of each stroke of the strings.

For a factory adjustment, inject a 1KHz @ 1V peak-to-peak signal at the pedals input, with the controls set the same. Measure the PCB at the test point (top right of the board) for 1.25V DC (+/-.05V DC), while adjusting the trimmer. The test point is also the same as pin 7 of U1. If 1.25V can't be achieved at the test point, then the JFET's Vgs(Off) is out of spec. It should be -1.00V +/-.15V.

### Circuit details

This trace is of the Dunlop (blue button) version of the Acoustic Guitar pedal. With their JFET bias selection, the range of Vgs(Off) is extended by +/- .1V (from +/- .05V to +/- .15V), without needing to adjust bias resistor values.

The compression in the circuit is very subtle - it's not very squishy and not comparable to other the Rockman X100.

### Changes from stock circuit

Cybercow made the following revisions to this circuit after comparing with a stock pedal:

* R29 and R30 were reduced from 150K to 100K. When these were 150K, the body control became too "boomy" at high levels. 
* The volume pot was increased from A100K to A500K. This increased the overall available output of the pedal.

These adjustments are included on the gerber files, but you can use the original values if you prefer.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure.
* Sockets (for the transistors and IC).
* Wire
* Solder

## Layout

This pedal uses a standard [four-knob layout](https://github.com/RWLPedal/music-pcbs/blob/main/instructions/DRILLING.md), although note that the volume knob is at the top right of the pedal, and the bypass indicator LED is positioned at the bottom of the board, closer to the footswitch, rather than between the four potentiometers.

Cybercow has included a [template](images/AmplifyFun_template.psd) if you want to print the pedal with AmplifyFun.

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
* V1.1 - C101 had been positioned backwards (in schematic and silkscreen). Fixed this - the positive lead should be at the bottom. This version is unvalidated, but that was the only change. Without this the pedal still worked fine, but there could be some problems with the reference voltage.
* V1.0 - Tweaked a few positions and fixed silkscreen errors. This version has been confirmed working over a few builds.
* V0.9 - First version, this worked, but Cybercow confirmed a few silkscreen errors, and also made the resistor adjustments noted in the BOM.