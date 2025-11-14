# Songifier Boost

![Example enclosure front and gutshot](images/front_guts.png?raw=true)

The *Songifier Boost* is a PCB based on the Skidmark Pedals Sonofier. It's an (inverting) boost plus an always-on (non-inverting) buffer, based on the amp section of the Sonomatic Delux Delay. It's a subtle always-on kind of effect.

Skidmark Pedals was the company founded by pedal designer Cees van Eijk, who passed away in spring 2024. Cees wrote a message to be shared posthumously: "*You are all free to use the schematics as posted in the files section, but I would appreciate if you at least would give me some credits. That my designs will live after I have passed, somehow gives me great comfort.*" It's in the spirit of that message that I share this PCB. Thankfully, build docs for the Sonofier were saved on some people's hard drives, and posted on the PedalPCB forums - thanks to forum member coltonius for sharing documentation.

The name from this pedal is a simple play on the Sonofier name. There are a few literal "song" birds (that is, birds with "song" in their names). I had in mind the [Song Sparrow](https://ebird.org/species/sonspa). It's one of the most common birds in the Pacific Northwest, and can be found in a variety of habitats. It's known for its cheery song and funny "chimp" call. Such a ubiquitous bird seems like a good fit for an always-on pedal.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/SongifierBoost/Songifier.zip) for fabrication.

## Bill of materials

| References | Value  | Footprint              | Notes               |
| :--------- | :----- | :--------------------- | :------------------ |
| C1         | 220N   | Film Capacitor         |                     |
| C2         | 220P   | MLCC Capacitor         |                     |
| C3         | 100N   | Film Capacitor         |                     |
| C4         | 10N    | Film Capacitor         |                     |
| C5         | 47N    | Film Capacitor         |                     |
| C6         | 100P   | MLCC Capacitor         |                     |
| C7         | 2U2    | Electrolytic capacitor |                     |
| C8         | 4N7    | Film Capacitor         |                     |
| C9         | 10N    | Film Capacitor         |                     |
| C10        | 100N   | Film Capacitor         |                     |
| C11        | 100N   | Film Capacitor         |                     |
| C12        | 1N     | Film Capacitor         |                     |
| C13        | 220N   | Film Capacitor         |                     |
| C14        | 4N7    | Film Capacitor         |                     |
| C15        | 100N   | Film Capacitor         |                     |
| C100       | 100U   | Film Capacitor         |                     |
| C101       | 100N   | Film Capacitor         |                     |
| C102       | 10U    | Electrolytic capacitor |                     |
| C103       | 100U   | Electrolytic capacitor |                     |
| C104       | 10U    | Electrolytic capacitor |                     |
| C105       | 100U   | Electrolytic capacitor |                     |
| C106       | 10U    | Electrolytic capacitor |                     |
| D1         | LED    | 3mm LED                |                     |
| D2         | LED    | 3mm LED                |                     |
| D100       | LED    | 3mm LED                | Bypass Indicator    |
| D101       | 1N5817 | Schottky Diode         | Polarity protection |
| D102       | 1N5817 | Schottky Diode         |                     |
| D103       | 1N5817 | Schottky Diode         |                     |
| R1         | 4K7    | 1/4W Resistor          |                     |
| R2         | 100K   | 1/4W Resistor          |                     |
| R3         | 10K    | 1/4W Resistor          |                     |
| R4         | 5K6    | 1/4W Resistor          |                     |
| R5         | 1M     | 1/4W Resistor          |                     |
| R6         | 1M     | 1/4W Resistor          |                     |
| R7         | 100K   | 1/4W Resistor          |                     |
| R8         | 2K2    | 1/4W Resistor          |                     |
| R9         | 150K   | 1/4W Resistor          |                     |
| R10        | 2K2    | 1/4W Resistor          |                     |
| R11        | 4K7    | 1/4W Resistor          |                     |
| R12        | 4K7    | 1/4W Resistor          |                     |
| R13        | 10K    | 1/4W Resistor          |                     |
| R14        | 47K    | 1/4W Resistor          |                     |
| R15        | 47K    | 1/4W Resistor          |                     |
| R16        | 4K7    | 1/4W Resistor          |                     |
| R17        | 47K    | 1/4W Resistor          |                     |
| R18        | 47K    | 1/4W Resistor          |                     |
| R19        | 4K7    | 1/4W Resistor          |                     |
| R20        | 10K    | 1/4W Resistor          |                     |
| R21        | 47K    | 1/4W Resistor          |                     |
| R22        | 100K   | 1/4W Resistor          |                     |
| R23        | 1K     | 1/4W Resistor          |                     |
| R100       | 4K7    | 1/4W Resistor          | LEDR                |
| R101       | 100R   | 1/4W Resistor          |                     |
| U1         | TL072  | IC                     |                     |
| U2         | TL072  | IC                     |                     |
| U3         | LT1054 | IC                     |                     |
| GAIN       | B1M    | 16mm Potentiometer     |                     |
| LEVEL      | A100K  | 16mm Potentiometer     |                     |
| TONE       | B25K   | 16mm Potentiometer     |                     |
| TYPE       | DPDT   | DPDT On/On Switch      |                     |

All of the parts in this build should be easily sourced.

"Now the use of the 'posh' OPA2134 might be debatable when comparing datasheets, but I'm not going down that rabbit hole. When I kick it in, it inspires me to play, when I switch it off, I'm suddnly just missing 'something'..."

You should be able to substitute in any dual op-amp (TL072, RC4558, etc).

This is a basic build, but an [interactive BOM](https://html-preview.github.io/?url=https://github.com/RWLPedal/music-pcbs/blob/main/SongifierBoost/interactive_bom.html) is available.

### Not listed

As with most guitar pedal BOMs, the following components are not listed above:

* Footswitch
* DC Jack
* 2x 1/4" audio jack
* Enclosure: this pedal fits into a 125B enclosure.
* Socket (for the IC).
* Wire
* Solder

## Layout

This pedal only has a single knob, so you can use whatever layout you like. The board is modestly larger than the potentiometer footprint.

### Screenshots

Here are the front and back with traces and component values:

![Screenshot of the front of the PCB](images/pcb_front.png?raw=true)

![Screenshot of the back of the PCB](images/pcb_back.png?raw=true)

Here is the front of the PCB with references rather than values:

![Screenshot of the front of the PCB with references](images/pcb_references.png?raw=true)

### Offboard wiring

Offboard wiring is unusual for this pedal. There are pads for input and output jacks, as well as power, at the top. These should be labeled.

There are also 9 direct connections to a footswitch. You can wire them directly to the footswitch, so BPIN/BPOUT/INPGND will connect to the first row of the footswitch, SWIN/SWOUT/GNDIN will connect to the second, and AMPIN/AMPOUT/LEDIN will connect to the third row.

The wiring is set up this way because this is not a true bypass pedal.

## Schematic

Below is the KiCad schematic.

![Screenshot of the circuit's schematic](images/schematic.png?raw=true)

## Licensing

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

This layout is licensed with a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.1 - Updated to position the knob to the top of the layout and verified. In the previous layout, caps and board collided with jacks, forcing knob to be positioned too low in the enclosure.
* V1.0 - First public version. Small tweaks a few traces and a tiny silkscreen adjustment.
* V0.9 - First version. Verified, works well.