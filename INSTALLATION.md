# Prep

Your PCB might arrive with some [slight perforations, from the breakaway panelization design](https://github.com/rorosaurus/gba-sp-usb-c/blob/master/images/breakaway-perforations.jpg) during PCB manufacturing. These can be left alone, or optionally filed/sanded away.

The half-circle pad(s) behind the USB-C connector might have some debris across it. You can safely clear that away with a toothpick or similar - that will make it easier to solder to later.

# Test before you install!

I test every board before shipping, but you should be certain it still works before you install it! Plug it in to a ````Type-C <-> Type-C```` cable and USB-C power source. **Do not perform this test with a ````Type-A -> Type-C```` cable - that cable won't verify the board works for full USB-C!** Use a multimeter to measure the voltage across any of the grounded holes and the +5V half-circle in the back. Ensure it reads ~5V. Flip your USB-C cable the other way around and verify it still reads 5V! Alternatively, if you have a USB-C multimeter [like this](https://smile.amazon.com/gp/product/B07X3HST7V/) you can simply plug into that and read the display.

# Installation Video

I highly recommend you watch [makho's video](https://www.youtube.com/watch?v=SoghQUyFCGM) of installing this PCB! This is an *awesome* overview that will be very helpful to reference. The below instructions simply outline what he does in the video.

# Instructions

The below pictures are from an older board revision, with only 1 half-circle. Your board is the same, you just have 2 half-circles to solder (for better reinforcement when plugging in).

## Step 1: Disassemble your Nintendo DS Lite and remove the motherboard

You can follow [this iFixit guide](https://www.ifixit.com/Guide/Nintendo+DS+Lite+Motherboard+Replacement/4784) for good disassembly instructions.

## Step 2: Remove the existing charge port

Use a solder-sucker, or solder wick to remove the solder from these 6 through-hole pins from the original charge port.

![Removing charging port](https://github.com/rorosaurus/nds-lite-usb-c/blob/master/images/removing-charging-port.jpg)

Take your time here, so you don't damage anything. Once you've removed most of the solder, the port should come off easily.

![Removed charging port](https://github.com/rorosaurus/nds-lite-usb-c/blob/master/images/removed-charging-port.jpg)

## Step 3: Prepare the new charge port

Assemble and test the new USB-C charge port!

![Assembled top](https://github.com/rorosaurus/nds-lite-usb-c/blob/master/images/assembled-top.jpg)

![Assembled bottom](https://github.com/rorosaurus/nds-lite-usb-c/blob/master/images/assembled-bottom.jpg)

Ensure that your USB-C PCB and the motherboard are flat and flush before continuing.

## Step 4: Position and attach the new charge port

The 5V half circle pad should line up just above the F1 fuse. You should be able to see the hole underneath it.

![Positioning top](https://github.com/rorosaurus/nds-lite-usb-c/blob/master/images/positioning-top.jpg)

Verify the side lines up flush with your DS Lite's case, as desired.

![Positioning side](https://github.com/rorosaurus/nds-lite-usb-c/blob/master/images/positioning-side.jpg)

The view from the bottom will show the VGND holes are just *slightly* not lined up with the USB-C port pins/holes. They are close enough, however - so when we bring them up to heat and add solder, a solid connection can be made. Verify that the VIN hole can see the 5V half circle pad from the top.

![Positioning bottom](https://github.com/rorosaurus/nds-lite-usb-c/blob/master/images/positioning-bottom.jpg)

When you are confident with your positioning, I recommend soldering the 5V half circle pad to the VIN hole underneath. This makes it easy to tweak the position of the USB-C port, since the port itself won't be too hot to touch.

If you want to reinforce the 5V and GND half circle pads with trimmed resistor leads like in the install video, this is the time to do that. :) You could also use a [male pin header](https://commons.wikimedia.org/wiki/File:6_Pin_Header.jpg) (slide off the plastic shroud and trim).

![Attach 5V pin](https://github.com/rorosaurus/nds-lite-usb-c/blob/master/images/attach-5v-pin.jpg)

Once you've verified your positioning is perfectly in place, flip the motherboard over and heat the remaining VGND holes, flowing solder into those joints and ensuring a solid connection to the USB-C port above.

## Step 5: Case trimming

![Case sizing](https://github.com/rorosaurus/nds-lite-usb-c/blob/master/images/case-sizing.jpg)

See how the current case fit is, and trim the case as necessary with a dremel, sandpaper, and flush cutters.

![Completed](https://github.com/rorosaurus/nds-lite-usb-c/blob/master/images/completed.jpg)

# Troubleshooting

### Did you test the board before installing?

See above instructions! It's critical that you test this to ensure it was not damaged during shipping!

### Try with a different cable and/or charger

This mod should work with all combinations of cables and chargers, but try a different one to help diagnose the problem by eliminating variables.

### Flip the USB-C cable to the other orientation

If it works only in one orientation, then check the two small resistors. Ensure they are oriented properly and soldered to their pads. Reheat the solder joints with your iron and confirm continuity with your multimeter.

If it still only works in one orientation, sadly one of the six USB-C port pins has a bad connection to my PCB (damaged in shipping, most likely).

You can reflow these pins with your soldering iron, adding solder if needed. If you apply too much solder and the pins get bridged, you can use solder wick or a solder sucker to remove some.


### Did you accidentally lift up some of the original charging port's pads?

You can test with your multimeter that you have continuity from the USB-C port to the expected destination. You'll have to follow the traces or look up where they lead. You can often rewire directly to the destination if you've messed up the original charging port's pad.

### You heard a "click" or your console is no longer powering on

You might have just blown a fuse. Check F1 (or similar) for continuity and replace the part if necessary (replacement part list in the [Game Boy Discord](https://discord.gg/gameboy)). After searching for and fixing the short that caused the fuse to blow, of course!

### Still stuck?

If you're still stuck, the friendly folks in #modding on the [Game Boy Discord](https://discord.gg/gameboy) might be able to help you. Make sure you are patient and respectful - and clearly describe the problem and what you have tried to solve it so far.

I'm always available through Amazon/Tindie as well!