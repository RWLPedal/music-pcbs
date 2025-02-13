# Fabrication

If you're unsure how to get a PCB fabricated, this page should help you figure it out. As an up-front disclosure, I am not an expert on fabrication, but I've had a number of boards fabricated without problems. When I first started the fabrication process I was nervous (but shouldn't have been). I've tried to answer the questions here that I had when I began.

## Background

You can skip this section if you just want to see instructions, but it contains useful context.

There's a number of programs for laying out PCBs. These all have different conventions and save the files in different formats. I have only used KiCad, an open source option. KiCad will typically save three files for each PCB:

* A project file (.kicad_pro) with pointers to other files.
* A schema file (.kicad_sch) which contains the circuit's schematic.
* A layout file (.kicad_pcb) with the actual component layout.

With these files you can change the circuit or adjust the PCB's layout. But, you might wonder, isn't it annoying to have many different files that describe the PCB? Yes.

The good news is that there's a single format which is typically used to share the PCB, called Gerber. A Gerber file is a "compiled" version of the layout. The bad news is that this means it can't really be edited, since it removes a lot of the requisite information to understand the layout in any given program. But it contains all the information necessary for someone to fabricate the PCB.

A Gerber file is simply a zip file containing 10+ other files. There are basically three types of files:

* The PCB has a number of layers. These include traces, silkscreens, paste, edge cuts, etc.
* The PCB has drilling instructions. Any through-hole components require drilling. I believe technically the drill files are not gerber files, but they get added to the whole gerber zip.
* There's an overall set of instructions. I believe this is mostly ignored in favor of options selected on PCB fabricator websites.

## Fabrication

Fabrication looks scary at first, but it's actual simple. I've only used some PCB fabricators; I'll include instructions for them here.

I think these sites regularly update their interface, so I won't include screenshots because they'll go out of date.

### PCBWay

[PCBWay](https://www.pcbway.com/) is a Chinese PCB fabricator. They offer both an option to fabricate from Gerbers, as well as an option to share projects for quick ordering ([example](https://www.pcbway.com/project/shareproject/L_il_Black_Cormorant_PCB_a7334241.html)). Ordering from a previously shared project is simple enough. If you want to fabricate an order with PCBWay using a gerber file, you can follow these instructions:

1. Go to the [quick order](https://www.pcbway.com/QuickOrderOnline.aspx) page. Note that this page is not linked from the PCBWay homepage, which featurse a process that requires selection of PCB board size (which nobody shares for pedals). This page is intimidating but you'll leave most things unchanged so don't worry about it.
2.  There's a link to "Add Gerber File" and select the file you want fabricated. This will auto-load the file. You'll see the layout in miniature.
3.  Note that the minimum order is 5 PCBs. Don't worry, they're cheap. Give away the extras, make variations, or use for birthday presents.
4. You'll leave most fields unchanged. All RWL PCBs are very standard. You can change a few fields if you want:
   * You can change the **thickness**. 1.6mm is a typical thickness, and it's the default - sturdy and feels good to handle, so there's not much reason to change it. But if you want you could likely order down to 1mm without adverse impact. If you're ordering faceplates, you probably want to go thinner.
   * You can change the **color**. Half the colors are will not change the price at all, but note that currently purple/matte black/matte green are much more expensive for a small order. Just check you price. Pick whatever you think best fits the pedal or your aesthetic. Colors other than green may take a few days longer to fabricate.
   * A typical **surface finish** is "HASL with lead," but I've seen people recommend lead-free HASL and immersion gold (ENIG). The HASL with and without lead are the same price. Other options are much more expensive. I've only ordered HASL with lead - it's your call.
   * PCBWay will print a product number (it's a text string). You can alternately select **remove product number** for a small fee. If the internal aesthetics of your build are important to you, you can select this option.
5. Double check the price. A set of 5-10 PCBs should cost $5-$10.
6. Save the order to your cart.

I've made a mistake or two in uploading gerbers (for example, accidentally zipping two PCB layouts into a single file). PCBWay manually reviews all uploads and will promptly send a message if they see anything unexpected.

After your upload is reviewed, you can check the layouts you want fabricated and go through the ordering process as you would with any store.

### JLC

[JLCPCB](https://jlcpcb.com) is another Chinese PCB fabricator. After creating an account, select "order now" to begin the process. This is the process as of January 2025.

1. After clicking "Order Now" you'll get a very intimidating-looking page, but you're going to leave almost everything set to the defaults.
2. There's a link to "Add gerber file." Click it, and select the gerber file for the PCB you've downloaded. This will upload the file and JLC will process it. Just wait 20 seconds or so before proceeding.
3. If everything went well, you'll see the layout appear in miniature on the page. You can select "Gerber viewer" to get a better sense what the layout looks like. This is what will be manufactured, so if it looks weird, don't order it.
4. Note that the minimum order is 5 PCBs. Don't worry, they're cheap. Give away the extras, make variations, or use for birthday presents.
5. You'll leave most fields unchanged. All RWL PCBs are very standard. You can change a few fields if you want:
   * You can change the **thickness**. 1.6mm is a typical thickness - sturdy and feels good to handle, so there's not much reason to change it (saving weight on shipping is the only time I've adjusted this). But if you want you could likely order down to 1mm without adverse impact. If you're ordering faceplates, you probably want to go thinner.
   * You can change the **color**. JLC offers a number of colors. Pick whatever you think best fits the pedal or your aesthetic. Colors other than green will take a few days longer to fabricate, but cost the same.
   * A typical **surface finish** is "HASL (with lead)," but I've seen people recommend lead-free HASL and ENIG. They cost more, but are slightly safer and/or more durable. I've only ordered HASL (with lead) - it's your call.
   * JLC will put a **mark on PCB,** typically the order number. I believe JLC has someone manually check each uploaded PCB before it's fabricated, and they'll drop the number in a corner where it doesn't interfere with anything. You can select "remove mark" but I think the option might be broken. I feel like I usually check that but still end up with a PCB with an order number. In any case, this is not a big deal, just a cosmetic concern.
6. Check your price. A set of 5 PCBs should total $2-$10, depending on the PCB size and how deluxe you go with the options. But some option combinations are very expensive or slow to fabricate.
7. Save the order to your cart.

That's all. You can add more orders if you want multiple PCBs. JLC's cart system is a little weird (you need to manually select items things from within your cart to add them to your total), but that's separate from fabrication options.