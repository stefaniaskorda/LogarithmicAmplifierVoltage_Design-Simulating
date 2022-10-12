# microelectronics-and-packaging

Logarithmic Amplifier Project for the course Microelectronics&amp;Packaging

This project implemented for the course Microelectronics and Packaging at 7th semester in Electrical and Computer Engineering School of National Technical University of Athens.

## 0.Context: The circuit we have chosen is known as a logarithmic amplifier voltage, as the output voltage which produces, it is proportional to its neper logarithmic input voltage.
the circuit consists of a voltage source, a resistor, an opamp and a bjt transistor. In particular, we chose as an opamp the LM714, npn: 2N2222 and R=10KΩ. The schematic is shown below:

<img src= "https://github.com/stefaniaskorda/LogarithmicAmplifierVoltage_Design-Simulating/blob/main/logamplifier_circuit.png" width = "300">

## 1.Simulation of the circuit 
We ran a dc sweep simulation in LTspice to make sure our circuit is working properly. Spice doesn't have the LM741 model, so we had to import it. As we saw in the datasheet of LM714, it has a source voltage of +/-15v, so we put V+=15-1=14V and v-=-14v, as positive and negative supply voltage respectively. We set the dc sweep for Vin from 0.1 to 10v to see the VOUT curve as a function of the input voltage.

## 2.Designing PCB
In the specific part of the report, the schematic design of the circuit arrangement we have chosen, the voltage logarithmer, as well as the design of the board for the specific arrangement will be made through the EAGLE design program.

### The diagram using Eagle:
<img src="https://github.com/stefaniaskorda/LogarithmicAmplifierVoltage_Design-Simulating/blob/main/eagle_diagram.png" width = "400">

### The final PCB design:
<img src = "https://github.com/stefaniaskorda/LogarithmicAmplifierVoltage_Design-Simulating/blob/main/pcb.png" width = "400">## 3.Implementation of Heatsinks

## 4. Design of Heatsinks
Fusion360 was used as CAD program for the design of Heatsinks for the bjt (2n2222) and for the opamp (lm741).
Below are the designs:

### opamp lm741
* 1st Heatsink
<img src="https://github.com/stefaniaskorda/LogarithmicAmplifierVoltage_Design-Simulating/blob/main/heatsinkopamp1.png" width = "400">

* 2nd Heatsink
<img src="https://github.com/stefaniaskorda/LogarithmicAmplifierVoltage_Design-Simulating/blob/main/heatsinkopamp2.png" width = "400">

* 3rd Heatsink
<img src="https://github.com/stefaniaskorda/LogarithmicAmplifierVoltage_Design-Simulating/blob/main/heatsinkopamp3.png" width = "400">

* 4rth Heatsink
<img src="https://github.com/stefaniaskorda/LogarithmicAmplifierVoltage_Design-Simulating/blob/main/heatsinkopamp4.png" width = "400">

### bjt 2n2222

* 1st Heatsink
<img src="https://github.com/stefaniaskorda/LogarithmicAmplifierVoltage_Design-Simulating/blob/main/sinkbjt1.png" width = "400">

* 2nd Heatsink
<img src="https://github.com/stefaniaskorda/LogarithmicAmplifierVoltage_Design-Simulating/blob/main/hbjt2.png" width = "400">

## 5.Thermal Analysis

The thermal analysis of the board will be carried out to observe the ability of the heatsinks to fulfill their role, but also to make a comparison between them in terms of the cooling capacity of each one.

To be able to carry out the analysis we will use the online program SimScale.
Before we proceed with the simulations, the following fields in SimScale are required to be filled out.
More specifically, what needed to be filled in or changed in the simulation environment is included in the list below.
* Element Materials:
* LM741 (OPAMP): The OPAMP body (the polymer) is Epoxy. Its pins are made of lead.
* 2N2222 (NPN): The body of the bipolar is tin (Tin) . Its pins are made of lead.
* Heat sinks: All heat sinks are made of aluminum.

### opamp lm741
* 1st Heatsink
<img src="https://github.com/stefaniaskorda/LogarithmicAmplifierVoltage_Design-Simulating/blob/main/thopamp1.png" width = "400">

* 2nd Heatsink
<img src="https://github.com/stefaniaskorda/LogarithmicAmplifierVoltage_Design-Simulating/blob/main/thopamp2.png" width = "400">

* 3rd Heatsink
<img src="https://github.com/stefaniaskorda/LogarithmicAmplifierVoltage_Design-Simulating/blob/main/thopamp3.png" width = "400">

* 4rth Heatsink
<img src="https://github.com/stefaniaskorda/LogarithmicAmplifierVoltage_Design-Simulating/blob/main/thopamp4.png" width = "400">

### bjt 2n2222

* 1st Heatsink
<img src="https://github.com/stefaniaskorda/LogarithmicAmplifierVoltage_Design-Simulating/blob/main/thbjt1.png" width = "400">

* 2nd Heatsink
<img src="https://github.com/stefaniaskorda/LogarithmicAmplifierVoltage_Design-Simulating/blob/main/thbjt2.png" width = "400">

## 6. Conclusion

For the opamp lm741 the 2nd Heatsink approoved as the best one and for the bjt 2n2222 the 1st one was the best as heatsinks.

