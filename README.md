![flow-MX36](https://raw.githubusercontent.com/jsallan/flow/main/images/20230623_180005~2.jpg) 

# flow
A product line of sculpted split ergo mech keyboards.

**\*\*Note:** as of 24-June-2023, the flow-MX36 is released and the flow-choc40 is in dev.
## Main Attributes
- integrated 34mm trackball using the PMW3360 sensor
- ceramic trackball bearings
- options for both choc v1 switches and MX switches
- USB-C interlink cable
- uC trays for PI Pico and Pro Micro (in dev)

**\*\*Note:** I think that a row and/or col could be added with some effort. I'm curious if this would make these keyboards more accessible. If you have time, I'd love to hear your perspective...here's a [survey](https://www.surveymonkey.com/r/B2MHMTC).
## Motivation
There's a number drivers for the keyboard series. Below is a summary of the top 3:
- proven comfort from previous split designs, [MX](https://www.thingiverse.com/thing:5404852) and [choc](https://github.com/jsallan/trinidox)
- trackball mandatory for enhanced convenience
- a finished look, e.g. hidden switches, smooth lines, hidden plate etc.

## Process
These keyboards started life as dactyl manuforms. The dactyl generators are great to quickly optimize key position, tenting angle etc. Once the design reached a point of comfort, the dactyl design was imported into Fusion 360. The dactyl was used for key and trackball positioning. 

The MX variant didn't have an existing trackball, so it took a number of iterations to nail down a comfortable position.

## MX and choc differences
Through a period of discovery, the comfortable trackball position relative to the thumb keys is quite different between choc and MX. This is ultimately the reason for the different keyboards. Of course the thickness of the key matrices are different, but I initially thought that could be overcome by clever design features. However once it was determined that trackball positions had to be different, two designs was the only path forward. This actually worked out well because the MX and choc key matrices on the reference designs were quite different, meaning a merge conflict was avoided.

## Print List
The print list assumes you want to print a trackball on the right and no trackball on the left.
| **Item** | **Mirrored?** | **Qty** | **stl** |
|----------|----------|---------|---------|
| left case | Yes | 1 | [MX](https://github.com/jsallan/flow/blob/main/stl/MX36/MX36%20std.stl) or choc |
| right case | No | 1 | [MX](https://github.com/jsallan/flow/blob/main/stl/MX36/MX36%20tball.stl) or choc |
| plate| 1-yes and 1-no  | 2 | [MX](https://github.com/jsallan/flow/blob/main/stl/MX36/MX36%20plate.stl) or choc |
| bearing holder | No | 3 | [here](https://github.com/jsallan/trinidox/blob/main/stl/tball_bearing_holder%20v14.stl) |
| uC holder | No | 2 | [PI Pico](link) or ProMico |

## Part List
Please note that the links below are intended as examples. These happen to be the same products that I bought, but I'm not an affiliate and have no business relationship with the sellers.
### Required for the case
| **Item** | **Qty** | **Link** |
|----------|----------|----------|
| uC | 2 | PI Pico: [WeAct at AliExpress](https://www.aliexpress.com/item/1005003708090298.html) or [Raspberry PI](https://www.raspberrypi.com/products/raspberry-pi-pico/)|
| 34mm trackball | 1 | [Amazon](https://www.amazon.ca/Perixx-PERIPRO-303-1-34-Inches-Trackball/dp/B08DD7ZDTG?ref_=ast_sto_dp&th=1&psc=1) |
| 2.5mm ceramic bearings | 3 | [AliExpress](https://www.aliexpress.com/item/4000829130283.html) |
| brass inserts M3 x D5.0 x L4.0 | 10 | [AliExpress](https://www.aliexpress.com/item/1005002526998853.html) |
| torx screws 50pcs M3, 8mm | 10 | [AliExpress](https://www.aliexpress.com/item/1005002369233576.html) |
| USB-C breakout board | 2 | [AliExpress](https://www.aliexpress.com/item/1005003245060475.html) | 
| USB-C interlink cable | 1 | [AliExpress](https://www.aliexpress.com/item/1005002811739151.html) |
| Furniture bumpers | 10 | [AliExpress](https://www.aliexpress.com/item/1005003044229837.html) |

**You'll also need one PMW3360 sensor board.** You can either purchase one from [tindie](https://www.tindie.com/products/jkicklighter/pmw3360-motion-sensor/), or [make your own](https://github.com/Ariamelon/Ogen).  

### Considerations for the electronics
The list below is not comprehensive because the items involve a lot of personal preference...some folks use hotswaps, some don't. Don't even get me started about keyswitches.
| **Item** | **Comments** |
|----------|----------|
| keyswitches | omg the options |
| keycaps | omg the options |
| hotswaps | makes it real easy to try different switches or reuse in another board |
| amoebas pcbs | not required, but a nice quality-of-life improvement. Essential if you want RGB. |
| diodes | gotta have em...unless you type 1 click at a time with no rollover (no one does) |
| wire | I use enamel coated wire, but there's lots of options |
| headers on uC | makes swapping out the uC easy |
| Short dupont cables | if using headers on uC, get these from [AliExpress](https://www.aliexpress.com/item/4000203371860.html) |
| magnetic adapter and cable | if you like to change keyboards often, these are useful from [AliExpress](https://www.aliexpress.com/item/1005002356514892.html) |

## Build Guides
There are many great build guides already written by people with a much better command of the english language than myself...so I'm not intending to put together a comprehensive how-to. Instead, below are some links that I've found super useful as I've built keyboards, and I hope they can serve others as well.
[Minidox Amoeba build](https://www.dlford.io/keyboard-build-guide-per-key-rgb-leds/) - very good overall build guide, especially if you intend to use amoebas and RBG LEDs.
[Sofle RBG build guide](https://josefadamcik.github.io/SofleKeyboard/build_guide_rgb.html) - useful for LED pinout.

## Buy Me a Coffee
[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://bmc.link/jsallan)
Absolutely no expectation...it seems to be a thing.

