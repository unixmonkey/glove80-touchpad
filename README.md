# glove80-touchpad
Touchpad sidecar mod for the Glove80 keyboard using the [ERGO Touchpad](https://ergonomictouchpad.com/ergonomic_touchpad.php) ([Amazon](https://www.amazon.com/gp/product/B087Z7RGGK/)).

![glove80-touchpad](https://github.com/user-attachments/assets/65a0a5c3-9d9c-401b-9a78-cb132499ce76)

## Why

I recently started getting RSI-like pain and went on a deep dive into the word of ergonomic split keyboards, but I knew a large part of my issue was my mouse usage habits, and that moving from the keyboard to the mouse (or trackpad) over and over again certainly wasn't helping.

Unfortunately, there currently are very few commercially available ergonomic keyboards that have built-in pointing devices.
However, the [MoErgo Glove80](https://www.moergo.com/collections/glove80-keyboards) keyboard tries to be highly ergonomic, as well as [customizable](https://www.moergo.com/pages/glove80-ergonomic-keyboard-customization) platform, and even provides built-in anchor points and some basic 3d models that can be used to add your own pointing devices right between the thumb cluster and forefinger areas. I figured this could be how I could possibly _make_ the Glove80 the perfect keyboard for me.

So I bought the Glove80, and a 3d printer, and got to work. This is helping me, and so I hope my efforts can help others.

## What you'll need

1. The [MoErgo Glove80 keyboard](https://www.moergo.com/collections/glove80-keyboards)
2. A 3D printer (or a friend/library/makerspace/business with one)
3. [ERGO Touchpad](https://ergonomictouchpad.com/ergonomic_touchpad.php) ([Amazon](https://www.amazon.com/gp/product/B087Z7RGGK/)).
4. 2.5mm screws (for the Glove80 mounting holes). I'm using 8mm deep ones I got in [this kit](https://www.amazon.com/dp/B0BLCFD9HR)
5. These [3d model files](/models/)

Optionally, if you want the USB cable to be detachable:

6. Soldering equipment, and a steady hand ([this is a great kit for cheap](https://www.amazon.com/gp/product/B07Q2B4ZY9/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&th=1))
8. A USB-C breakout board (I used [this treedix board](https://treedix.com/products/treedix-4pcs-usb-type-c-breakout-board-serial-basic-breakout-female-connector-type-pcb-converter-board) also available on [Amazon here](https://www.amazon.com/dp/B096M2HQLK)

## Test the touchpad

While unlikely, it's entirely possible the touchpad may be DOA (Dead on Arrival), so plug it in to a computer and make sure it works before we start questioning our sanity if it somehow no longer works after soldering.

The ERGO works a little different compared to many touchpads, but I found it very easy to adapt to:
- Tap to left-click
- Tap in the top-right corner to right-click
- Slide your finger along the rightmost edge to scroll
- Double-tap to click and hold (useful for dragging windows/files around) - This one takes a little practice
  
![ergo-touchpad](https://github.com/user-attachments/assets/1c510572-bb2b-4797-a366-e398384f6302)

It comes with velcro, so if you have a regular sidecar printed, you can use mostly out-of-the-box like that, but I wanted something a bit cleaner.

## 3d printing

This 3d model works pretty well and looks fairly sharp, in my opinion. It's main features are:

- It is expanded to the edge of the thumb cluster, and flares out to completely support the touchpad
- It is perfectly flush to the Ergo touchpad, when the velcro is removed
- It is angled and tilted just a bit to make it easier to use with your index finger
- It has a hole and platform for a USB-C connector and board (optional)
- It has a bottom plate (also optional)

![right-hand-touchpad-model](https://github.com/user-attachments/assets/2e6256ec-1910-475e-8ac6-b583d737a37a)
![right-hand-touchpad-back](https://github.com/user-attachments/assets/742a2d49-9385-4dbd-80c3-80710523e2c4)

If you want to use on the left-hand of the Glove80, mirror the model along the flat outer surface.

## Assembly

Carefully peel the velcro off of the back of the Ergo touchpad, making sure to not damage the USB cable that is tucked under it.

![peel-velcro](https://github.com/user-attachments/assets/86c6a1ad-99d9-4a55-96e1-f7cc181b328c)

Note: Those two green buttons are right and left click, so you could possibly wire them up to actual buttons if desired. I might try a version with a left-click button to make dragging easier.

Now, you should be able to thread the USB cable through the hole in the model, and optionally secure it with some tape on the underside.

If you don't care about a detachable USB cable, you can stop here, and simply screw the sidecar to your Glove80 and stop here.

## Adding a Detachable USB-C Connector

The model includes a small platform and hole for a Treedix USB-C connector & board. This can be used to make it easy to unplug the whole thing at the box, instead of at the computer.

1. Cut the Ergo Touchpad USB cable about 4-5 inches (100-130mm) from the board
2. Score and peel away an inch (~20mm) or so of the protective jacket to expose the USB wires inside
3. On each individual wire, score and peel back each wire to expose about 2-3mm of copper
4. Melt a very small amount of solder onto the exposed copper to get them nice and ready for soldering
5. Melt a very small amount of solder onto the Treedix connector pads where we will be attaching the wires

This is how it should look all wired up:

![usb-c soldering](https://github.com/user-attachments/assets/853847c8-6fb5-4ad3-ba3a-a044ed8be759)

After soldering, you can either screw, tape, or hot-glue the board to the platform.

Then, tuck the wires inside and screw on the back (if you printed that model), with 2.5mm screws (same as the sidecar mounts).

## TODO

- Experiment with the shape of the outer edge
- Possibly wire up buttons to Kailh switches

## See Also

- My [Glove80 Ergo Trackpoint mod](https://github.com/unixmonkey/glove80-trackpoint)
- My [Glove80 Wireless Trackball mod](https://github.com/unixmonkey/glove80-trackball) (in progress)

I love the freedom from RSI pain this keyboard has saved me from, and I love it even more with these mouse-replacements. My pain has gotten much more managable, and I've enjoyed getting into 3d modeling and printing!

Thank you to the many people who have posted on the [MoErgo Discord Community](https://www.moergo.com/discord) that helped inspire me to make this happen, and are always dropping great tips on how to optimize my computing experience.
