# StompFuzz

---

*For more DIY pedal fun, visit the [MAS Effects](https://mas-effects.com) page.*

---

This is a fun and practical guitar pedal, and a great opportunity to practice surface mount (SMD) soldering (and do so with nothing but your regular soldering iron). It fits neatly over a 3PDT stomp switch.

### How to get it

You can either download the gerber files from this repo, or [buy the PCB on my store here](https://mas-effects.square.site/product/stompfuzz-pcb/24?cp=true&sa=false&sbp=false&q=false&category_id=7), or get a [kit that includes SMD components and footswitch](https://mas-effects.square.site/product/stompfuzz-kit/26?cp=true&sa=false&sbp=false&q=false&category_id=7).

### Pics and Wiring Diagram

![stompfuzz](stompfuzz.jpg)

![stompfuzz wiring](stomp-fuzz-wiring.png)
## Intro

This is a bazz fuss circuit, with endless possibilities to try. 

If you want a tinier, simpler version check out the [picofuzz](https://github.com/mstratman/picofuzz).

I recommend experimenting with component values. e.g. see these writeups for some ideas to get started

* [tonefiend project](https://www.tonefiend.com/wp-content/uploads/DIY-Club-Project-2-v02.pdf)
* [home-wrecker.com writeup](http://home-wrecker.com/bazz.html)

## Schematic

NOTE: Resistors and capacitors are 0805 packages.

You can and should substitute other values for all the components. But these are decent starting points.

![stompfuzz schematic](stompfuzz-schematic.png)

## Omitting potentiometers

All of the pots on this pedal are optional. Here are steps to omit any or all of the 3:

**Omit Volume**: Jumper V2 to V3

**Omit Tone**: Omit C3, solder nothing to T1 and T3

**Omit Gain**: Jumper G1 to G3

![omitting potentiometers](/omitting-knobs.png)

## Combinations to try:

TODO: This should be filled in and fleshed out further

MMBTA14LT1G + 10k
MMBT6427LT1G  + 10k
MMBF5457
MMBT3904VL  + 510k
MMBT5088LT1G + 100k


Diodes:
1N914BWS
BAT46JFILM

* C1: 0.001uF
* C2: 0.1uF
* C3: 0.22uF
* R1: 510k 
* D1: 1N914BWS
* Q1: MMBT3904VL


## Tone

Tone control blends between C1 and C3. Pick two different values to change which frequencies get cut when the tone is high or low.

## Buzz Box

Try chaining it with a [picofuzz](https://github.com/mstratman/picofuzz) to allow you to switch between a single and dual fuzz.

## Optional add-ons:

* diode for polarity protection
* filter power supply for noise. e.g. 22uF cap between +9V and GND
* LED: and optionally anti-pop on LED

Note this already has a 1M resistor on the input cap to help limit switch popping
