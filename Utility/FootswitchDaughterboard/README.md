# Footswitch Daughterboard
This is a very simple daughterboard, which can be used for most true bypass pedals. Of course, you can simply wire footswitches directly, but I find this a bit tidier and more convenient.

If printed on JLC PCB, with a 5x5 tiled layout and the minimum 5 panels, you can currently get 125 daughterboards for $7.15, or 17 cents each. This is somewhat cheaper than any you could buy a handful anywhere else... although you'll have 125! When printing on JLC, select the `Panel by JLC` Delivery Format, then on the dialog which appears, select `Column=5; Row=5; Edge Rails = No Rails`.

For my layout, I wanted the following affordances, which were not on other daughterboards:

* All pads labeled on front and back of the daughterboard.
* All traces explicitly printed on the silkscreen (for easy reference).
* My own name on the daughterboard.

If you'd like to just get started, you can go ahead and download the [gerber](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/FootswitchDaughterboard/gerber.zip) for fabrication.

## Bill of materials

No BOM - this is simply a daughterboard compatible with a standard 3PDT footswitch or toggle switch.

## Layout

The layout is for a standard PedalPCB-style daughterboard.

### Screenshots

Here are the front and back with traces and component values:

![Screenshot of the front of the PCB](https://github.com/RWLPedal/music-pcbs/blob/main/FootswitchDaughterboard/images/pcb_front.png?raw=true)

![Screenshot of the back of the PCB](https://github.com/RWLPedal/music-pcbs/blob/main/FootswitchDaughterboard/images/pcb_back.png?raw=true)

## Schematic

For reference, below is the (messy) KiCad schematic:

![Screenshot of the circuit's schematic](https://github.com/RWLPedal/music-pcbs/blob/main/FootswitchDaughterboard/images/schematic.png?raw=true)

## Licensing

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

This layout is provided with a Creative Commons BY-NC-SA 4.0 license (Attribution, Non-commercial, Share-alike).

## Versions

* V1.0 - First version, works fine.