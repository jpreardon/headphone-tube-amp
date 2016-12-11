# Project Log

### 2016-12-10

#### Part 1

After organizing the components and studying the schematic a bit more, I realized I was missing a couple 1/2 watt resistors (they were 1/4 watt on the BOM, but 1/2 on the schematic). Luckily, Radio Shack had some. While I was there, I also picked up a couple 1/8" jacks for input.

I started mounting the output jack and the potentiometer on the enclosure. Unfortunately, they don't project enough through the case. The jack just catches the nut, but only by a thread or two. The, pot, no way, even after I broke off the tab used to keep it from rotating :) More about the pot later.

Here's what it looks like so far.

![enclosure front](https://scontent-iad3-1.cdninstagram.com/t51.2885-15/s1080x1080/e15/fr/15251777_967469766688077_6027269915923185664_n.jpg)

I think the only other thing going on the front is a small power switch, and maybe a power LED. The switch will probably go right over the sticker.

I soldered some wires on the jacks and the pot. I tested it out with some headphones to make sure it worked as expected. It did, but it seems like this pot might be kind of shitty. It cuts out a little near the max. It needs to get replaced with one with a longer shaft anyway, so not a big deal.

### Part 2

I connected everything up, was happy to see the heaters glow when I plugged it in. I set the bias and checked the DC offset. I noticed that the offset was a little high on the right channel (~14 mv as opposed to the < 10mv I was expecting, the left channel was around 7.5 mv).

I tested with some cheap earbuds and was happy to actually hear music! I plugged in some better headphones and listened to some music:

- Sharon Jones & The Dap Kings: What if We All Stopped Paying Taxes
- Sex Pistols: Sub-Mission
- Rush: Tom Sawyer

Sounds great! It is bright, as others have reported. There is a low level hiss, which is only noticeable when there is no sound. I'll have to see what I can do to get rid of that. It also picks up some RFI, most noticeable if an iPhone is a foot or so away from the circuitry.

Now I guess I need to make a board for this thing and put it in the case.

### 2016-12-06

Tubes came in yesterday, and the rest of the parts today. Power supplies shipped today as well.

Since the tube isn't going to fit so well on the breadboard, I was looking for a way to wire it up temporarily so it isn't flopping around. I found this a  cigar box in my small junk collection. I think I "borrowed" it from Carl's shop a couple years ago. Anyway, I drilled some holes in the sliding cover, and mounted the tube socket along with some wires that I will hook up later. The wires were a mess, so I labeled all of them.

Even though it is meant to be temporary, I guess this little cigar box could function as a more permanent enclosure. It will need some ventilation holes in it though.

I put [some pictures](http://jpreardon.com/2016/12/06/temporary-amp-enclosure/) on my blog.


### 2016-12-01

Shopping day!!!

Ordered:

- 2 [power supplies](http://www.ebay.com/itm/321987484194?_trksid=p2060353.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT)
- [Bigger Breadboard](http://www.digikey.com/product-detail/en/digilent-inc/340-002/1286-1062-ND/4840822)
- [Perf Board](https://www.digikey.com/product-detail/en/vector-electronics/8029/V2025-ND/1886431)

Plus the following from the BOM (except what I have on hand, the case and heat sinks)

Part | Value | QTY | Source | Part #
---|---|---|---|---
R1 | 100k, 1/4W | 2 | On Hand |
R2 | 150, 1/4W | 2 | On Hand |
R3 | 4.7k, 1/4W | 2 | On Hand |
R4 | 10, 1/4W | 2 | On Hand |
R5 | 1k, 1/4W | 2 | [Digikey](http://www.digikey.com/product-detail/en/yageo/CFR-25JB-52-1K/1.0KQBK-ND/96) | CFR-25JB-52-1K
U1 | LM317 | 2 | On Hand |
C1 | 2.2uF, 16V | 2 | [Digikey](http://www.digikey.com/product-detail/en/panasonic-electronic-components/ECQ-E1225KF/EF1225-ND/56392) | ECQ-E1225KF
C2 | 100uF, 16V | 2 | [Digikey](http://www.digikey.com/product-search/en?keywords=647-UFG1C101MPM) | UFG1C101MPM
C3 | 470uF, 16V | 2 | [Digikey](http://www.digikey.com/product-detail/en/nichicon/UFG1E471MHM1TO/493-10909-1-ND/4317836)| UFG1E471MHM1TO
Q1 | IRF510 | 2 | [Digikey](http://www.digikey.com/product-search/en?keywords=IRFI510GPBF) | IRFI510GPBF
Socket | 9pin PCB | 1 | [Tube Depot](https://www.tubedepot.com/products/9-pin-pc-mount-socket) | -
V1 | 12AU7 | 1 | [Tube Depot](https://www.tubedepot.com/products/electro-harmonix-12au7-eh-preamp-vacuum-tube/) | -
P1 | 50k | 2 | [Digikey](http://www.digikey.com/product-search/en?keywords=3299W-1-503LF)| 3299W-1-503LF
Jack | 1/4" Stereo| 1 | [Digikey](http://www.digikey.com/product-detail/en/switchcraft-inc/112BX/SC1317-ND/1217816) | SC1317-ND
Audio Pot | 10K | 1 | [Digikey](http://www.digikey.com/product-detail/en/bourns-inc/PDB182-E420K-103A/PDB182-E420K-103A-ND/3780709) | PDB182-E420K-103A
Case | | 1 | - | -
Mica | | 4 | - | -
Heatsink | | 4 | - | -

### 2016-11-30

Putting together shopping list. I'm going to put this together on a breadboard first, so I'll skip the enclosure and PCB stuff for now.

### 2016-11-28

Spent some time reading over the [project page](http://diyaudioprojects.com/Solid/12AU7-IRF510-LM317-Headamp/) in detail.

Researched PCB fabrication

- [This one](http://www.instructables.com/id/Easy-Consistent-Cheap-Toner-Transfer-Method-for-Si/?ALLSTEPS) requires a laminator.
- I saw another tutorial using toner transfer that looked like a huge pain in the ass, due partly to the heavy, glossy printer paper used. The one above certainly seemed better.
- I liked [Colin's](http://www.jameco.com/Jameco/workshop/video/make-learn-to-etch-cicuit-board-with-collin-cunningham.html) tutorial, which uses photoresist.
- There's some talk [here](http://www.diystompboxes.com/smfforum/index.php?topic=99788.0) about liquid tinning, I think I'd like to do that.
