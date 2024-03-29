The XO106r5 is a logical progression from its predecessors - although it no longer contains any 40106 ICs, it's still a good source of square-wave glitchiness along with a filter should you want to round off some of the rough edges.

It's also a lot bigger - 22HP.

The salient features are:

*    4 AVR-based square-wave oscillators with V/oct response good for around 5 octaves. There are fine-tune pots on the back side of the PCB.
*    Voltage-controlled pulse width for each oscillator
*    Oscillator firmware is available under a permissive license.
*    Patchable Sallen-Key low-pass filter - use it, or don't; it's something of a nod to the previous incarnations of the module.
*   Patchable logic matrix - this is the big step from the previous versions. 

The oscillators are no longer hardwired to the logic IC; you can patch things together how you want, or not at all - you can also patch in external sources as you see fit. The logic IC itself is socketed so you can replace it with a different, pin-compatible, IC should you wish to change the voicing of the module. The 'default' option is a CD4070 (quad XOR) but alternatives include the 4001, 4011 and 4093.

THE DEFAULT CONFIGURATION FOR THIS WILL BE A PCB/PANEL/FIRMWARE SET - I don't recommend this is as a beginners project.

* The firmware for this module is the same as that for the Squascillator VCO - you will need to burn four firmware ICs.
* The two jumpers (JP1 and JP2) control the response of the filter pots - use a blob of solder to bridge the centre pad with one of the outer pads

The terminally curious can view [Johnny Beaver's demo of a prototype unit in action on YouTube ...](https://youtu.be/iXnucviOB_w)

### Panel files

If want to roll your own panel, there are two panel files in the repo - the KiCAD board file is the same one that I use for the panels of 'retail' units. If 
you have some KiCAD-fu then you can customise it to your heart's content and then send the resulting file off to you friendly local fab for production. The DXF
file consists of the Edge-Cuts PCB layer and can be consumed by most laser cutters - this panel is unadorned.
