geiger
======

Low Voltage 2.5V PIN Diode Based Geiger Counter

Purpose
======

Super low voltgae Geiger Counter using a modified PIN photodiode. See Bernd Laquai's paper on the subject here: http://www.opengeiger.de/ABGDetektor_en.pdf. The first stage charge amplifier gain is set by the feedback Cap and Resistor. Bigger resistor = more gain, but it pulls the output low and reduces the amplifier's swing on the negative side. 1M is about the biggest resistor you can safely use. The second stage amp takes the negative pulse from the 1st stage and inverts it and boost it x10 so it can be easily read.

Project Structure
=================

/GeigerCounter
* The Eagle PCB project

/Library
* Any components that are not found in the Eagle or SparkFun default libraries, I have made myself and they are here.

/GeigerCounter/FabricationOutput
* This holds the fabrication output script. Based on SparkFun's script. It also holds the zip file Gerber files that were sent out for fabrication.
