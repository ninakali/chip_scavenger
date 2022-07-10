# POORLY made substitutes for components

I had a few chats in the past where people brushed off the availability of common passive components. Because they are so simple, they can be made from things found in a typical western household. But is that so?

## Resistance is (mostly) futile
A few online guides say resistors can be made easily from paper clips, a strip of paper and a pencil.
![()](01_r_src.jpg)

Even a century-old hobbyist magazine stated that a resistor of 2-3 MOhms can be made this way. I tried to scribble on a scrap of paper tightly, and the paper quickly got damaged.
![()](02_r_poor.jpg)

Not surprisingly, graphite has some conductivity. The resistance is around 2.5 MOhms indeed, but it is probably highly volatile, and the whole thing looks, to put it mildly, fragile.
![()](03_r_2.5mohm.jpg)

Using better paper, pencil and firm surface gives a less fragile, more conductive resistor. It worked for me as a current-limiting resistor for lighting up an LED. Still, it seemed that the (s)crap resistance changed not only from the position of the clips but from the voltage applied.
![()](04_r_18kohm.jpg)

**Verdict**: not suitable for anything useful. If you want to make resistors at home, you need better technology.


## Paper + cheap glue + foil = PCB? (Ha-ha, no)
There are plenty of guides on using factory-made bare PCBs, but there is very little information on how to make boards at home. The only YouTube video I found recommended glueing some paper and aluminium foil together. I was sceptical but tried it nevertheless. I guess this could work for a school project, but it is not suitable even for DIP (2.54mm grid) components. If you cut your tracks well, they won't stay attached to the cardboard base. If you cut carefully, a short circuit is likely. It's very unreliable, fragile, and overall unpleasant to work with.

![()](05_foil_pcb.jpg)

**Verdict**: Nope. Just nope. Better invest in some cotton paper and epoxy, I guess...

## Paper + cheap glue + foil = Capacitor? (Um, kind of)
This is yet another recipe that can be found both online and in vintage magazines. In theory, you put two pieces of aluminium foil, separate them with paper, and get a capacitor. For a flat one, capacity is C = e * e0 * S / d.

If I'm not mistaken:
* e0 = 8,85*10^-12
* e for paper is between 2 and 3.5; let's say 2.5
* S is 0.2 by 0.2 metres = 0.04 sq m
* d is about 0.1 mm for my paper => 0.0001 m
* C => 885 * 10^-12 = 885 pF = 0.885 nF = 0.000885 uF

The actual capacitance depends on the paper, the glue and the precision of your work. If you roll the capacitor, as I did, its capacitance will also change. Nevertheless, it was not high enough to register on my multimeter (therefore, less than 0.01 uF). The capacitor seemed to be working, charging and discharging. Still, due to the sloppy implementation, it had relatively high resistance. On top of that, it charged to a few dozen mV without any power source (though this is somewhat expected, I think). It's bulky, and its capacity will vary depending on the humidity because water will affect glue and paper.

![()](06_c_poor.jpg)

**Verdict**: _maybe_ could be used with some caution and careful execution.
