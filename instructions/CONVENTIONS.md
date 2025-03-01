# Layout Conventions

For my layouts, I try to apply the same set of conventions for the sake of consistency.

Having a consistent policy for PCBs means that you can know what to expect when you populate them. Not to mention that debugging in the event of problems is easier.

## Hardware Layout
* *Top-mounted* - Audio and power jacks should be at the top of the pedal, unless there are too many jacks to fit (e.g. a switcher).
* *Control spacing* - following [PedalPCB standard layouts](DRILLIING.md) for knobs and switches. This ensures enclosures can be reused across pedals that have the same number of controls.
* *Control layout* - for standard 3-knob overdrive/fuzz/distortion, *Volume* is at the top left of the pedal (when the pedal is in its enclosure) and *Fuzz/Gain* or similar is at the top right, with the bottom reserved for *Tone* or other controls.
* Input/output pads: 2x audio jack grounding pads + DC positive/negative pads at top; IN/SW/GND/OUT on bottom. This is also the PedalPCB standard layout (some larger PedalPCB pedals do have on-PCB input/output positive connections).

## Component placement
* *Indicator LED* - All boards include the LED and LEDR onboard. They can simply be omitted if you would prefer to populate these offboard.
* *ICs* - Always positioned with pin 1 at the upper left (this means the IC notch will be facing the top of the PCB).
* *Electrolytic capacitors* - leads are positioned consistently across the entire PCB (ie, all negative leads might be facing the bottom, right, etc - according to the board). Ideally the negative lead is at the bottom, but this is much harder in most layouts.

## Label/Silkscreen
* All input/output pads labeled with name on both front and back of the PCB. This is to prevent the most common source of errors I've encountered when I am testing/populating a PCB (connecting wires to the wrong pads).
* All controls (potentiometers/switches) are labeled with name and value on front and back of the PCB. This is to prevent the second most common source of errors when I am populating a PCB (getting the potentiometer values mixed up). Having the name populated on the back allows easy reference when using a test platform to audition the PCB outside of a box, without needing to refer to the documentation.
* For clarity, LED leads are labeled with +/- on front and back, rather than with other annotations like A/K, or simply showing the flat part of the LED package.
* Capacitor leads are labeled with + on the front and back.

## References
* Power and LED components are labeled with references in the hundred range (such as *R100* for the first resistor in the power/LED section or *D101* for the second diode) to indicate that they are not part of the main circuit, which is numbered sequentially starting from 1.

## Gerbers
* Gerber files provided with attribute values on the silkscreen, so no need to reference the BOM when populating the PCB. Attribute references are still available via screenshot in the build doc.