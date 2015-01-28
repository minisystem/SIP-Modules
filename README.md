SIP-Modules
===========

Analogue SIP modules

Single Inline Pin [SIP] Package Modules for Analogue Synthesizer Design
===============================================================

******************************
IMPORTANT!- READ THIS FIRST!!!
*************************************************************************************************************
THESE REPOSITORIES ARE A MESS RIGHT NOW BECAUSE OF MY PREVIOUS AD HOC VERSION CONTROL
I will eventually tidy them up but at the moment I don't know which are the latest and fully correct versions 
*************************************************************************************************************

What are these?
===============

These are designs for modules that make up the bulidng blocks of an analogue synthesizer. They were inspired 
by the original Curtis Electromusic (CEM) chips used in dozens of 70s and 80s synthesizer designs. They are *NOT* 
electronically equivalent to the original CEM chips. They were designed to be compact modules for building 
a polyphonic analogue synthesizer. They use SMT parts but are designed for hand soldering. As there are parts on both sides of the board a substantial redesign might be required for automated assmebly by a pick-and-place assembly service.

VCO SIP
=======
This is an analogue Voltage Controlled Oscillator (VCO) module in a 30 mm x 18 mm 12 pin SIP package.
It is a classic SAW core design derived from the Terry Michaels/Mikulik/Electronotes/ASM-1 circuit. It employs 
waveshapers from George Hearn's HMVCO1c design, with modifications to limit output levels to 10V pp. Other
changes from the original Electronotes design include elimination of the linear FM input and swapping the CA3140 
integrator for the cheaper LF351. It uses an inexpensive BCM847 NPN matched transistor pair in contrast
to the super matched pairs (LS318, LM394, SSM2210, etc) called for in other SAW core designs.

VCF-VCA SIP
===========
This is a 4 pole LM13700 OTA-based Voltage Controlled Filter (VCF) in a 40 mm x 18 mm 10 pin SIP package.  It is derived from Roland filter designs based around the IR3109 quad OTA filter. Voltage controlled resonance is implemented with an LM13700 OTA cell and the spare OTA is used for a Voltage Controlled Amplifier (VCA), thus combining two functions into one module, similiar to the Roland D80017A VCF-VCA module used in the Juno 106.

EG ADSR SIP
===========
This is a voltage controlled Envelope Generator (EG) with Attack, Decay, Sustain and Release stages in a 30 mm x 18 mm 10 pin SIP package. It is derived from similar designs by Massimo Ischia and Scott Rider (OldCrow) with modifications to respond to 0-10V control voltages and to produce a 0-10V output.
