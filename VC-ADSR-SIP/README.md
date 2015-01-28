Voltage Controlled ADSR Envelope Generator
==========================================

This is a voltage controlled Envelope Generator (EG) with Attack, Decay, Sustain and Release stages in a 30 mm x 18 mm 12 pin SIP package. It is derived from similar designs by Massimo Ischia and Scott Rider (OldCrow) with modifications to respond to 0-10V control voltages and to produce a 0-10V output.

Massimo Ischia's version:
http://digilander.libero.it/ismsynth/vc-adsr-1.2.jpg

Scott Rider's version:
http://www.muffwiggler.com/forum/viewtopic.php?p=1151245
(scroll down for schematic in thread)

Notes
=====

Ideally, I'd like to eliminate the trimmers for Attack and Decay/Release times. I tried doing this in an early revision but needed to tweak the resistor values more than I expected so reverted to trimmers. However, in subsequent revisions I've hardly needed to make any adjustments at all. A 0603 or 0805 resistor should be able to bridge the T1 and T2 footprints.

Q1's schematic symbol has a pin numbering that swapped the emitter (pin 1) and base (pin 2) when used with the default SOT23 footprint. I fixed this by swapping the pad numbers on the SOT23 footprint module, but this change applies to *this project only*.

This project was created in Kicad 4022 but routed in 5112 using the CERN push and shove router. This means that the CvPcb footprint association uses the legacy library format and not the new library table format. I haven't tried to do the conversion yet. 