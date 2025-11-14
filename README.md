# RWL Pedal PCBs

![RWL Pedals Mascot, an Osprey](images/osprey.png)

This is a repository for sharing PCB layouts, and pedal-building advice. Most PCBs here are for effects pedals.

 If you've never had PCBs fabricated before, check out the [fabrication instructions](instructions/FABRICATION.md) - it's easy and cheap to have PCBs manufactured.

## What can I expect?

These PCBs have the following properties:

All PCBs:
* Have top jacks for both power and audio. There are no side jack layouts.
* Have component values printed on the board. No need for a printed bill of materials (BOM) - they're all self-documenting.
* Fit into a 125B enclosure (a few can fit into a smaller form factor).
* Use consistent [control layouts](instructions/DRILLING.md) and spacing to the extent possible.
* Follow consistent [layout conventions](instructions/CONVENTIONS.md).

If you do want a BOM, most boards include an interactive BOM as a single downloadable HTML file, allowing easy inspection of the layout and identification of components.

### Guides

The following are guides for my layouts, or for pedal-building in general:

* [Conventions](instructions/CONVENTIONS.md) - Layout and placement conventions I attempt to follow.
* [Drilling](instructions/DRILLING.md) - Drill templates for RWL pedals.
* [Fabrication](instructions/FABRICATION.md) - How exactly do you turn Gerber files into physical PCBs? Learn more here.
* [KiCAD Files](KiCAD/KICAD_SETUP.md) - Files I use in KiCAD for my layouts (footprints and symbols) and how to install them.
* [Wiring](instructions/WIRING.md) - Shows how to wire all pedals I've shared.

## PCBs

### DIY-related PCBs

The following PCBs are DIY-related, meaning they are based on kits or from circuits shared on pedal-building forums. However, many are based on classic pedals (or are the basis for them).

|                              PCB Name                              |       Type       |        Circuit Name         | Circuit Author  | Fav?  |
| :----------------------------------------------------------------: | :--------------: | :-------------------------: | :-------------: | :---: |
| [Buffalo-Weaver Overdrive](OverdriveFuzz/BuffaloWeaverOverdrive/)  |    Overdrive     | Guitar Magazine Tube Bender |   Dan Coggins   |
|          [Corn Crake Fuzz](OverdriveFuzz/CornCrakeFuzz/)           |       Fuzz       |          NG-4 Fuzz          |    Dylan159     |
|         [Dipper Compressor](Compressor/DipperCompressor/)          |    Compressor    |      "That" Compressor      |    Dylan159     |
|          [Dirty Bird Fuzz](OverdriveFuzz/DirtyBirdFuzz/)           |       Fuzz       |        BC108 Dirtbag        |  Cees van Eijk  |
|            [Fledgling Phaser](Phaser/FledglingPhaser/)             |      Phaser      |     PUP: Litter of Four     |    Dylan159     |
|    [Footswitch Daughterboard](Utility/FootswitchDaughterboard/)    |     Utility      |             N/A             |       N/A       |
|       [Gray Hornbill Fuzz](OverdriveFuzz/GrayHornbillFuzz/)        |    Sitar/Fuzz    |           Jawari            |  Tim Escobedo   |
| [Li'l Black Cormorant Fuzz](OverdriveFuzz/LilBlackCormorantFuzz/)  |       Fuzz       |       L'il Black Key        |      BYOC       |
|            [Li'l Echo Parakeet](Delay/LilEchoParakeet/)            |      Delay       |          L'il Echo          |      BYOC       |
|            [Ms Mallard Filter](Filter/MsMallardFilter/)            | Envelope Filter  |        Nurse Quacky         |   Homewrecker   |
|        [Pacific Loon Tremolo](Tremolo/PacificLoonTremolo/)         |     Tremolo      |     Trembling Satellite     |    Dylan159     |
| [Screech Owl Harmonic Tremolo](Tremolo/ScreechOwlHarmonicTremolo/) | Harmonic Tremolo |         Equanimity          |  Cees van Eijk  |   *   |
|       [Sharp-shinned Fuzz](OverdriveFuzz/SharpShinnedFuzz/)        |       Fuzz       |     One-Knobber Project     | Effects Layouts |
|          [Shiny Cowbird](OverdriveFuzz/ShinyCowbirdFuzz/)          |       Fuzz       |   Dyl-Ei Fuzz Apprentice    |    Dylan159     |
|  [Shred-Masked Distortion](OverdriveFuzz/ShredMaskedDistortion/)   |    Distortion    |          Shredder           |      BYOC       |
|              [Songifier Boost](Boost/SongifierBoost/)              |  Boost & Buffer  |          Sonofier           |  Cees van Eijk  |
|            [Tui Overdrive](OverdriveFuzz/TuiOverdrive/)            |    Overdrive     |        Supreaux Deux        |  RunOffGroove   |   *   |
|                 [Tiny Tyrant](Pll/TinyTyrantPll/)                  |       PLL        |           PLLedal           |    Dylan159     |
|                 [Weaver Boost](Boost/WeaverBoost/)                 |   Dirty Boost    |          Artiflex           |  Cees van Eijk  |
| [White-Throated Overdrive](OverdriveFuzz/WhiteThroatedOverdrive/)  |    Overdrive     |  Dudson Narrowest Castest   |    Dylan159     |   *   |

### Commercial

The following PCBs are based on commercial circuits:

|                                PCB Name                                 |        Type        |                Compare to                | Fav?  |
| :---------------------------------------------------------------------: | :----------------: | :--------------------------------------: | :---: |
|           [CrimsonKiwi](OverdriveFuzz/CrimsonKiwiOverdrive/)            |  Octave Overdrive  |         Way Huge Purple Platypus         |   *   |
|     [Honeycreeper Overdrive](OverdriveFuzz/HoneycreeperOverdrive/)      |     Overdrive      |        Mad Professor Sweet Honey         |   *   |
|                 [Horus Fuzz](OverdriveFuzz/HorusFuzz/)                  |        Fuzz        |       Black Art Toneworks Pharoah        |   *   |
|          [Kakapo Distortion](OverdriveFuzz/KakapoDistortion/)           |     Distortion     |             Kokko Distortion             |       |
|             [King Eider Fuzz](OverdriveFuzz/KingEiderFuzz/)             |        Fuzz        | Catalinbread Katzenkönig/AionFX Poseidon |   *   |
|      [Little Hawk Distortion](OverdriveFuzz/LittleHawkDistortion/)      |     Distortion     |            Durham Crazy Horse            |
| [Northern Harrier Distortion](OverdriveFuzz/NorthernHarrierDistortion/) |     Distortion     |                ProCo RAT                 |
|        [Morepork Distortion](OverdriveFuzz/MoreporkDistortion/)         |     Distortion     |             MXR Distortion+              |
|               [Potoo Octave](OverdriveFuzz/PotooOctave/)                |    Octave Fuzz     |      Fuzzhugger(fx) Phantom Octave       |
|        [Red-winged Overdrive](OverdriveFuzz/RedwingedOverdrive/)        |     Overdrive      |              EHX Hot Tubes               |   *   |
|       [Saturnine Antshrike Boost](Boost/SaturnineAntshrikeBoost/)       |       Boost        |            Spaceman Saturn V             |   *   |
|                 [Shoebill Boost](Boost/ShoebillBoost/)                  |       Boost        |           Way Huge Angry Troll           |
| [Southern Screamer Overdrive](OverdriveFuzz/SouthernScreamerOverdrive/) |     Overdrive      |           Ibanez Tube Screamer           |
|          [Whippoorwill Fuzz](OverdriveFuzz/WhippoorwillFuzz/)           |        Fuzz        |    Dunwich Amplification Cthulhu Fuzz    |
|               [Wood Owl Acoustic](Other/WoodOwlAcoustic/)               | Acoustic Simulator |      Rockman Acoustic Guitar Pedal       |

