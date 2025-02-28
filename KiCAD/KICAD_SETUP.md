# KiCAD files

I use KiCAD for all my layouts. It's open source and free. I'm not a professional but it works fine for me.

If you want to lay out PCBs, you'll rely on a library of symbols and footprints. KiCAD comes with a number of these, but many common symbols and footprints used in guitar pedals are missing. I'm sharing mine here.

First - credit to MadBeanPedals for sharing their footprints. My footprints are mostly based on theirs, with some heavy tweaks for consistency of some pad sizes, my preferences for display (changed font and silkscreen). That said, I can't guarantee that the symbol names and documentation is particularly clean right now. But they've served me well enough for 30+ layouts.

## Symbols

Symbols are what appear in circuit schematics. They're used in the Schematic Editor.

1. Download the [RwlLib.kicad_sym](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/KiCAD/RwlLib.kicad_sym) file and put it in your symbols directory (on Windows this is `C:\Users\[Username]\Documents\KiCad\[version]\symbols`).
2. Open KiCAD, and then open the `Symbol Editor` function.
3. Select `Preferences -> Manage Symbol Library`.
4. I would recommend adding this library globally so you don't need to follow this process every time. Click the `+` button to add a new library. This will create a new row.
5. Put 'RwlLib' as the Nickname, and .kicad_sym file path as the path. The nickname is case-sensitive.

You should now have access to symbols I've created that were missing from the main KiCAD library (or were present but had supoptimal pin arrangements/etc).

## Footprints

Footprints are what appear in PCB layouts. They're used in the PCB Editor.

1. Download the [RwlLib.pretty.zip](https://github.com/RWLPedal/music-pcbs/raw/refs/heads/main/KiCAD/RwlLib.pretty.zip) file.
2. Unzip it in your footprints directory (on Windows this is `C:\Users\[Username]\Documents\KiCad\[version]\footprints`).
3. Make sure it's not nested after the unzip (you should see `...\footprints\RwlLib.pretty\[a bunch of files]`), not `...\footprints\RwlLib.pretty\RwlLib.pretty\[a bunch of files]`).
4. Open KiCAD, and then open the `Footprint Editor`.
5. Select `Preferences -> Manage Symbol Library`.
6. I would recommend adding this library globally so you don't need to follow this process every time.  Click the `+` button to add a new library. This will create a new row.
7. Put 'RwlLib' as the Nickname, and put the .pretty directory as the path in the row. The nickname is case-sensitive.

You hsoul dnow have access to footprints I've derived from MadBeanPedals, or created myself.
