# Experiment--03
# Design Differential amplifier for the following specification vdd=3.3v p<=3mw vicm=1.72v vocm=1.81v vp=0.7v perform dc analysis,transient analysis,ac analysis and extract required parameter 
Components required:
1)N-MOSFET(nmos4),

2)Resistors(3.42k(2),685ohm(1),

3)DC Power supply (3.2V,1.6V),

4)Current source (1 mA).

Theory
A Differential amplifier takes two input signals and amplifies the difference between them, Ignoring anything that's the same in both signals. It's like tuning out the background noise and focusing on the unique parts of a conversation.This makes it super useful for things like measuring tiny differences in voltages in sensitive electronic equipment.

The Differential amplifier circuit consists of:
*Two inputs V1 and V2,

*Two Resistors to set gain,

*Power supply,

*pair of operational amplifers.

Working principle:
The working principle of a differential amplifier can be broken down into a few key steps:

Input Signals: The amplifier receives two input signals, typically labeled as 𝑉1 and 𝑉2.

Difference Calculation: The amplifier focuses on the difference between these two input signals. In mathematical terms, it calculates the difference Vdiff=V1-V2.

Amplification: The amplifier then amplifies this difference by a certain gain factor, which determines how much the difference is magnified. The gain is usually denoted by A.

Output Signal: The amplified difference is then produced as the output signal,Vout=Ad(V1-V2).

Procedure:
1.Open the LTspice software, merge the library file for getting accurate values of NMOS.

2.Select the components which are needed to us like for circuit 1 we need 3.2k & 685ohm resistors,2 CMOSN, three voltage sources(1.6v(2), 3.2v(1)),ground from the components list.

3.Place them all components in necessory way which is helpfull, connect all the components as in given circuit .

4.Link the specification of list of properties of mosfet like threshold voltage, temperature etc.

5.Lets do the DC Analysis first by opting a simulation, we get .op so after placing it we will get the values of it, thet will displayed.

6.After that lets take Transient analysis of 5m cycle so in input and output waveforms in 5 complete cycle, so here we get and seperate and combined waveforms of input and output.

7.For AC analysis, we should do some changes like converting DC SOURCE to sinosoidal waveform (1.6,50m,1k),after that select the AC simulation from the given options of simulation after giving values of (Decade,20,01,1T). So we will get a output after placing node to output waveform.

Given:VDD=3.3; P<=3mW;

Vicm=1.6V; Vocm=1.72V;

Vp=0.7

Iss=p/vdd=3.3*10^-3/3.3=0.90mA

ID1=ID2=Iss/2=0.902mA/2=0.45mA

RD=VDD-Vocm/ID1=3.3-1.81.45mA=3.3K

Rss=VP/Iss=0.7/0.90=777ohms

W=8.23uM

L=180nM
   
# Circuit Diagram:
![Screenshot 2025-03-04 214351](https://github.com/user-attachments/assets/9a2cffc9-2880-45dc-a66b-2b04fe8c06e4)

 

# DC Analysis
Go to simulate select the dc output and run the simulation
This analysis used to find the id value.Go to simulate select a dc sweep analysis,Give the values as shown below and run the simulation

![Screenshot 2025-03-04 214423](https://github.com/user-attachments/assets/79a562e0-b9af-4609-83a6-9d0cbe6f272c)

# AC Analysis
go to simulate select the ac analysis give the values as shown in below and run the simulation 
![Screenshot 2025-03-04 215932](https://github.com/user-attachments/assets/21a43117-91d5-42d4-965b-150380122cfa)

Below graph shows the output of the ac analysis




# Transient Analysis
Go to simulate select transient analysis set the stop time as 1ms and run the simulation ,The below graph shows the output of transient analysis



# INFERENCE
.For a differential amplifier to work properly, you need to set the MOSFETs in their active region (saturation region for long-channel MOSFETs). This typically involves proper sizing of resistors, current sources, and gate voltages
. Varry the MOSFET length and width (m1&m2)get calculated id current in dc analysis
.set the Ac amplitude as 1 in the ac analysis
. From the frequency response, you can determine the bandwidth of the differential amplifier by identifying the frequency
# RESULT
.By varrying Mosfet width and length we get id current 0.45mA
m1 and m2 L=180nm w=7.8nm
.RSS value 777ohm and rd=3.3kohm
