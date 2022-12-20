# AGD my Alaska-Gold-Detector-Project

12/20/2022 - Auto-Mation-Assist - Johannes P Fassotte

The AGD metal detector project is a DIY project for the electronics for a dual channel pulse injection metal detector using sample and hold technology. It is of analog design that is capable of detecting the small gold typically found in Alaska. The design allows for the use search coils that are designed to be used for the GPX 5000 which have a inductance of around 300uH. Testing of the electronics was completed with CoilTek 9 and 14 inch Elite mono coils and a Detech 8 inch DD coil.

This project is very complex and requires good knowledge of electronics, suitable enclosure design, proper equipment for installing the surface mount components, and suffcient test equipment for intial alignment. There are 3 circuit boards, RX and logic board, TX board, and an Interface board for the front panel user controls.

The front panel has the power input connector, on/off switch, standby switch, headphone speaker switch, TX pulse width control, first sample width control, second sample width control, front end gain adjust, detect sensitivity control, sample ratio control, normal invert switch, and volume control. The sample ratio control, normal invert switch allow for mixing the two receive channels together in different ratios if external conditions are noisy.

The rear panel has the typical five pin coil connector and a small isolated tip ring sleeve connector. This connector can drive a 50uA meter which can be used to give a visual indication of the voltage being routed to the VCO driver. A switch in the meter enclosure allows for displaying the voltage from two different sources. The indicator is not required but its nice to have that ability.

I designed this project because I did not want a metal detector that has a digital display and instead has standard controls where you can see seting in one glance. Power is supplied by a 12 volt 10ah LIFePO4 Lithium battery carried like the GPX 5000 and supplies a negative voltage referance to the circuits common. Current draw from the battery varies with TX pulse width and I have not accurate measured that. The current meter on my test power supply indicates 350 to 500 milliamps for different TX pulse rates. TX pulse being limited to about 53us max.

I use two of these detectors and added four inch speakers with heavy magnets in the enclosures. This was for flexibily but added substantial weight. My enclosure gets mounted at the rear of the shaft with custom rail on top of my enclosure and with standard GPX 5000 hardware.

I find the sound produced by some detectors to be hard on the ears and thus to make it as pleasent as possible the detect tone output in my design is a sine wave, and is internally automatically adjusted to idle at 300 Hz after power up stabilization is completed. It will increase in frequency in response to having detected metal. Decay after going across a large piece of metal will drive the tone below 300 Hz which makes it hard to hear due to its low frequency and is a good indication of an potential overload condition. On power up the detect tone will decrease to its idle value after the circuitry has stabilized and also adjusted itself to the external conditions.

For my own in house testing in a very noisy environment I use a gold picker that weights in at .025 grams and has a flat surface that is about 1/8 inch in diameter, and a bit more oval than round. The detector will respond to this when it is about 3 inches from the bottom of the coil and with the internal automatic transition calibration set properly for the TX to RX transition with a CoilTek 9 inch elite coil. 

It takes a good deal of time to assemble this project and the parts costs are not inexpensive. I'm happy with the overall performance of this design and its ability to respond to small gold that has a resonable surface area. Since like the GPX 5000 there is the single cable to the battery pack and also the headphone connector. I dont notice the battery back on my back or belt but do find that the cable to bother me sometimes. I tried the available coiled cables but found that a long straight 5 conductor self built 7ft 8inch cable was better. Internally battey power is regulated to +10/-10 Vdc and most of the electronic components use those voltages.  The CMOS logic only uses the negative 10 Vdc while TX coil power is supplied directly from the negative side of the battery. The LIFePO4 12V Lithium battery is charged with a charger designed for that type of battery to 14.4 Vdc. Actual fully charged battery is likely about 13.7 volts.

This project is just for assembly of the circuit boards, other items required to build the complete metal detector are readily available from vendors that normally sell those items and will vary depending on the builders desires. The enclosure and its end plates needs to be aluminum to provide protection agaist RFI.

