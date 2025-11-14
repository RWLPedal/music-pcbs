# RWL Pedal PCBs

![RWL Pedals Mascot, an Osprey](images/osprey.png)

This is a repository for sharing PCB layouts, and pedal-building advice. Most PCBs here are for effects pedals.

 If you've never had PCBs fabricated before, check out the [fabrication instructions](instructions/FABRICATION.md) - it's easy and cheap to have PCBs manufactured.

## What can I expect?

These PCBs have the following properties:

All PCBs:
* Have top jacks for both power and audio. There are no side jack layouts.
* Have component values printed on the board. No need for a BOM - they're all self-documenting.
* Fit into a 125B enclosure (a few can fit into a smaller form factor).
* Use consistent [control layouts](instructions/DRILLING.md) and spacing to the extent possible.
* Follow consistent [conventions](instructions/CONVENTIONS.md).

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

|                          PCB Name                           |       Type       |        Circuit Name         | Circuit Author  | Fav?  |
| :---------------------------------------------------------: | :--------------: | :-------------------------: | :-------------: | :---: |
|    [Buffalo-Weaver Overdrive](/BuffaloWeaverOverdrive/)     |    Overdrive     | Guitar Magazine Tube Bender |   Dan Coggins   |
|             [Corn Crake Fuzz](/CornCrakeFuzz/)              |       Fuzz       |          NG-4 Fuzz          |    Dylan159     |
|           [Dipper Compressor](/DipperCompressor/)           |    Compressor    |      "That" Compressor      |    Dylan159     |
|             [Dirty Bird Fuzz](/DirtyBirdFuzz/)              |       Fuzz       |        BC108 Dirtbag        |  Cees van Eijk  |
|            [Fledgling Phaser](/FledglingPhaser/)            |      Phaser      |     PUP: Litter of Four     |    Dylan159     |
|    [Footswitch Daughterboard](/FootswitchDaughterboard/)    |     Utility      |             N/A             |       N/A       |
|          [Gray Hornbill Fuzz](/GrayHornbillFuzz/)           |    Sitar/Fuzz    |           Jawari            |  Tim Escobedo   |
|    [Li'l Black Cormorant Fuzz](/LilBlackCormorantFuzz/)     |       Fuzz       |       L'il Black Key        |      BYOC       |
|           [Li'l Echo Parakeet](/LilEchoParakeet/)           |      Delay       |          L'il Echo          |      BYOC       |
|           [Ms Mallard Filter](/MsMallardFilter/)            | Envelope Filter  |        Nurse Quacky         |   Homewrecker   |
|        [Pacific Loon Tremolo](/PacificLoonTremolo/)         |     Tremolo      |     Trembling Satellite     |    Dylan159     |
| [Screech Owl Harmonic Tremolo](/ScreechOwlHarmonicTremolo/) | Harmonic Tremolo |         Equanimity          |  Cees van Eijk  |   *   |
|          [Sharp-shinned Fuzz](/SharpShinnedFuzz/)           |       Fuzz       |     One-Knobber Project     | Effects Layouts |
|               [Shiny Cowbird](/ShinyCowbird/)               |       Fuzz       |   Dyl-Ei Fuzz Apprentice    |    Dylan159     |
|     [Shred-Masked Distortion](/ShredMaskedDistortion/)      |    Distortion    |          Shredder           |      BYOC       |
|             [Songifier Boost](/SongifierBoost/)             |  Boost & Buffer  |          Sonofier           |  Cees van Eijk  |
|               [Tui Overdrive](/TuiOverdrive/)               |    Overdrive     |        Supreaux Deux        |  RunOffGroove   |   *   |
|               [Tiny Tyrant](/TinyTyrantPll/)                |       PLL        |           PLLedal           |    Dylan159     |
|                [Weaver Boost](/WeaverBoost/)                |   Dirty Boost    |          Artiflex           |  Cees van Eijk  |
|    [White-Throated Overdrive](/WhiteThroatedOverdrive/)     |    Overdrive     |  Dudson Narrowest Castest   |    Dylan159     |   *   |

### Commercial

The following PCBs are based on commercial circuits:

|                          PCB Name                          |        Type        |                Compare to                | Fav?  |
| :--------------------------------------------------------: | :----------------: | :--------------------------------------: | :---: |
|           [CrimsonKiwi](/CrimsonKiwiOverdrive/)            |  Octave Overdrive  |         Way Huge Purple Platypus         |   *   |
|     [Honeycreeper Overdrive](/HoneycreeperOverdrive/)      |     Overdrive      |        Mad Professor Sweet Honey         |   *   |
|                 [Horus Fuzz](/HorusFuzz/)                  |        Fuzz        |       Black Art Toneworks Pharoah        |   *   |
|          [Kakapo Distortion](/KakapoDistortion/)           |     Distortion     |             Kokko Distortion             |       |
|             [King Eider Fuzz](/KingEiderFuzz/)             |        Fuzz        | Catalinbread Katzenkönig/AionFX Poseidon |   *   |
|      [Little Hawk Distortion](/LittleHawkDistortion/)      |     Distortion     |            Durham Crazy Horse            |
| [Northern Harrier Distortion](/NorthernHarrierDistortion/) |     Distortion     |                ProCo RAT                 |
|        [Morepork Distortion](/MoreporkDistortion/)         |     Distortion     |             MXR Distortion+              |
|               [Potoo Octave](/PotooOctave/)                |    Octave Fuzz     |      Fuzzhugger(fx) Phantom Octave       |
|        [Red-winged Overdrive](/RedwingedOverdrive/)        |     Overdrive      |              EHX Hot Tubes               |   *   |
|   [Saturnine Antshrike Boost](/SaturnineAntshrikeBoost/)   |       Boost        |            Spaceman Saturn V             |   *   |
|             [Shoebill Boost](/ShoebillBoost/)              |       Boost        |           Way Huge Angry Troll           |
| [Southern Screamer Overdrive](/SouthernScreamerOverdrive/) |     Overdrive      |           Ibanez Tube Screamer           |
|          [Whippoorwill Fuzz](/WhippoorwillFuzz/)           |        Fuzz        |    Dunwich Amplification Cthulhu Fuzz    |
|           [Wood Owl Acoustic](/WoodOwlAcoustic/)           | Acoustic Simulator |      Rockman Acoustic Guitar Pedal       |

