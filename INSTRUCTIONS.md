# nds-lite-usb-c
A USB-C port mod for the Nintendo DS Lite

# Instructions

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

![Attach 5V pin](https://github.com/rorosaurus/nds-lite-usb-c/blob/master/images/attach-5v-pin.jpg)

Once you've verified your positioning is perfectly in place, flip the motherboard over and heat the remaining VGND holes, flowing solder into those joints and ensuring a solid connection to the USB-C port above.

## Step 5: Case trimming

![Case sizing](https://github.com/rorosaurus/nds-lite-usb-c/blob/master/images/case-sizing.jpg)

See how the current case fit is, and trim the case as necessary with a dremel, sandpaper, and flush cutters.

![Completed](https://github.com/rorosaurus/nds-lite-usb-c/blob/master/images/completed.jpg)

## Step 6: 3D Print bezel to fill the gap

Coming soon maybe?
