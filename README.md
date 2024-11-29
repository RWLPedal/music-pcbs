# Music PCBs

This repository contains links to publically available PCBs, including Gerber files, which can be printed cheaply from any PCB fabricator.

## PCBs

Here's list of my own PCBs.

|            PCB Name             | PCB Author | Type  |     Schematic Name     | Schematic Author |
| :-----------------------------: | :--------: | :---: | :--------------------: | :--------------: |
| [Shiny Cowbird](/ShinyCowbird/) |    RWL     | Fuzz  | Dyl-Ei Fuzz Apprentice |     Dylan159     |
| [Footswitch Daughterboard](/FootswitchDaughterboard/) |    RWL     | Utility  | N/A |     N/A     |

## Conventions

For my layouts, I've attempted to apply the following conventions:

* **Layout:**
  * *Control spacing* - following PedalPCB standards for knobs and switches. This ensures enclosures can be reused for layouts that have the same number of controls.
  * *Control layout* - for standard 3-knob overdrive/fuzz/distortion, *Volume* is at the top left of the pedal (when the pedal is in its enclosure) and *Fuzz/Gain* or similar is at the top right, with the bottom reserved for *Tone* or other controls.
* Input/output pads: 2x audio jack grounding pads + DC positive/negative pads at top; IN/SW/GND/OUT on bottom. This is also the PedalPCB standard layout (without onboard input/output jack positive connections).
* **Components:**
  * *Indicator LED* - All boards include the LED and LEDR onboard. They can simply be omitted if you would prefer to populate these offboard.
  * *ICs* - Always positioned with pin 1 at the upper left (this means the IC notch will be facing the top of the PCB).
  * *Electrolyic capacitors* - leads are positioned consistently across the entire PCB (ie, all negative leads might be facing the bottom, right, etc - according to the board).
* **Labels:**
  * All input/output pads labeled with name on both front and back of the PCB. This is to prevent the most common source of errors when I am testing/populating a PCB (connecting wires to the wrong pads).
  * All controls (potentiometers/switches) are labeled with name and value on front and back of the PCB. This is to prevent the second most common source of errors when I am populating a PCB (getting the potentiometer values mixed up). Having the name populated on the back allows easy reference when using a test platform to audition the PCB outside of a box, without needing to refer to the documentation.
  * For clarity, LED leads are labeled with +/- on front and back, rather than with other annotations like A/K, or simply showing the flat part of the LED package.
  * Capacitor leads are labeled with + on the front and back.
* **References:**
  * Power and LED components are labeled with *?10?* references (such as *R100* for the first resistor in the power/LED section) to indicate that they are not part of the main circuit.
* **Gerbers:**
  * Gerber files provided with attribute values on the silkscreen, so no need to reference the BOM when populating the PCB. Attribute references are still available via screenshot in the build doc.