# Finding MCUs by pinouts
One of the easiest ways to identify a microcontroller is by its power bus layouts.

This document needs to be converted into a database, and a tool should be written to find matches by pins.

## SOIC and DIP

### Atmel ATtiny 13,25,45,85
GND the last pin on the first row, VCC the last pin. 

### Atmel ATtiny 44/84, ATtinyX12, ATtinyX14, ATtinyX24
VCC 1, GND the last pin.

### Atmel ATtiny 48/88, 261,461,861
VCC and GND are at the middle of the left row, VCC and then GND.
E.g. VCC is 7 and GND is 8 on 28-pin.

### Atmel AT89LP216
16-lead: GND 4, VCC 12

### CMsemicon CMS79F51xx
VCC pin 1, GND pin 16 on many 16-lead.
VCC 1, GND 2 on 8-lead and some 16-lead.

### Cypress CY8C21234
GND is 8 and 6, VCC is 16 on 16-pin.

### Cypress CY8C401
VDD is 7, GND is 8 on a 16-pin controller.

### Freescale Kinetis KE04
16&20 pin SOIC: VCC 3, GND 4.

### FMD TF60F023
VCC pin 4, GND pin 13 on SOP16.

### Fujitsu F2MC-8FX MB95
VCC 6, GND 3 on SOP and DIP 16.

### Holtek HT66F0176
GND 1, VCC 16 on 16-pin.
GND 1 and last VCC on 20, 24 pin too.

### Infineon XMC1000 Family - ARM!
In SOIC-16, GND is 5 and VCC is 6.

### Infineon CY8CMBR3110
VDD is 7, GND is 8 on a 16-pin controller.

### Microchip PIC10F200/202/204/206 10F220/222/224/226
VCC is 2, GND is 7.

### Microchip Some PIC12
VCC 1, GND the last pin.

### Microchip PIC16
It's hell. 

* 16F684/688/1823/1824/1825 - VCC 1, GND last.
* 16F84/627/628/648/88/1826/1827 - GND left middle (5), VCC right middle (14)
* 16F1933/1936/1938/1512/1513/1516/1518/882/883/886 - GND 19, VCC 20 out of 28.

### Micron MT25QU
VCC 2, GND 10 (second pin on each side) on SO16

### Motorola HC908
TSSOP - GND and then VCC are in the middle of the left side.
DFN - GND and then VCC are in the middle of the left side.

### NEC 78K0S/KY1 μPD78F921
SSOP16 GND 4, VCC 5
DIP16 GND 8, VCC 9

### NXP LPC81xM - ARM
DIP8 VCC 6, GND 7
SOP16 GND 13, VCC 12

### NXP MC9S08PL16S, NXP MC9S08PB
Pin 3 VCC, pin 4 GND for 20, 16 and 8 pin SOIC.

### NXP MC68HC908QL4
VCC 1, GND 16 on DIP16.
GND 4, VCC 5 on SOP16.

### NXP / Phillips P87LPC7xx, P89LPC9xx 8051
16-pin DIP and SOP - GND 4, VCC 12.

### NXP HC08 HC908QY
PDIP&SOIC - VCC is 1, GND is last
TSSOP - GND and then VCC are in the middle of the left side.
DFN - GND and then VCC are in the middle of the left side.

### Nuvoton N79E8 8051
16 pin: GND 5, VCC 12
20 pin: GND 5, VCC 15 (?!)

### PADAUK
131-S16A and S16B have opposite VCC and GND: pin 1 and pin 16 (the last one).
PMC131, 131-S14, S16A, D16A will have VCC on pin 1.
S16B and D16B will have GND on pin 1.

### Renesas RL78/G10
GND is second to last and VCC is the last pin on the left side (i.e. pins 4 and 5 on 10-pin body)

### Silicon Labs EFM8BB1x CIP-51
SOIC-16: GND - 4, VCC - 5

### Silicon labs C8051F80x-83x
SOIC-16: GND 4 and VCC 5 (middle pins on the left)

### Sinomicon SM51F20TD2 8051
GND 5, VCC 15 or GND 1, VCC 20 on 20-lead
GND 1, BCC 16 on 16-lead

### Sonix SN8F5702 8051
GND pin 1, VCC last pin on SOP14/16

### STC STC15W201S
SOP16 - VCC  6, GND 8.

### STM ST62 ST6200C
VCC 1, GND 16 in 16-pin package.

### STM ST7LITE1xB
16 and 20 pin SO/DIP: GND 1, VCC 2

### TI COP8SA
SO16: VCC 6, GND 11.
SO20: VCC 6, GND 15
SP28: VCC 6, GND 23 (basically, same position, just chip gets longer)
DIP40: VCC 8, GND 33

### TI MSP430FR25x2
16-pin PW: VCC 5, GND 6.

### XDS XDS901
VCC 1, GND 16.
