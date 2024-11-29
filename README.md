# Music PCBs

This repository contains links to publically available PCBs, including Gerber files, which can be printed cheaply from any PCB fabricator (such as JLC or OSHPark).

## PCBs

Here's list of my own PCBs.

|            PCB Name             | PCB Author |     Schematic Name     | Schematic Author |
| :-----------------------------: | :--------: | :--------------------: | :--------------: |
| [Shiny Cowbird](/ShinyCowbird/) |    RWL     | Dyl-Ei Fuzz Apprentice |     Dylan159     |

## Conventions

For my layouts, I've attempted to apply the following conventions:

* Control spacing: following PedalPCB standards for knobs and switches.
  * Control layout: for overdrive/fuzz/distortion, *Volume* is at the top left and *Fuzz/Gain* is at the top right, with the bottom for *Tone* or other controls.
* Input/output pads: 2x audio jack grounding pads + DC positive/negative pads at top; IN/SW/GND/OUT on bottom. This is also the PedalPCB standard layout (without onboard input/output jack positive connections).
* Components: all boards include the LED and LEDR onboard. They can simply be omitted if you would prefer to populate these offboard.
* ICs: Always positioned with pin 1 at the upper left (notch to PCB top).
* Electrolyic capacitors: leads consistently positioned across the entire PCB (ie, all negative leads at bottom/right/etc according to the board).
* Labels:
  * All input/output labeled with name on both front and back of the PCB. This is to prevent the most common source of errors when I am testing/populating a PCB.
  * All controls labeled with name and value on front and back of the PCB. This is to prevent the second most common source of errors when I am populating a PCB. The name on the back allows easy reference when testing the PCB out of the box, without needing to look at the documentation.
  * For clarity, LED leads are labeled with +/- on front and back, rather than with other annotations like A/K, or simply showing the flat part of the LED package.
  * Capacitor leads are labeled with + on the front and back.
* References:
  * Power and LED components are labeled with *10?* references (such as *D100*) to indicate that they are not part of the main circuit.
* Gerbers:
  * Gerber files provided with attribute values on the silkscreen, so no need to reference the BOM. Attribute references provided via screenshot on github.