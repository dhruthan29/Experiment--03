# Experiment--03
# Design Differential amplifier for the following specification vdd=3.3v p<=3mw vicm=1.72v vocm=1.81v vp=0.7v perform dc analysis,transient analysis,ac analysis and extract required parameter 
Circuit Diagram:
 
C:\Users\Althaf M S\Pictures\Screenshot 2025-03-04 214351.png 
# DC Analysis
Go to simulate select the dc output and run the simulation
This analysis used to find the id value.Go to simulate select a dc sweep analysis,Give the values as shown below and run the simulation

"C:\Users\Althaf M S\Pictures\Screenshot 2025-03-04 214423.png"
# AC Analysis
go to simulate select the ac analysis give the values as shown in below and run the simulation
"C:\Users\Althaf M S\Pictures\Screenshot 2025-03-04 215932.png"
Below graph shows the output of the ac analysis




# Transient Analysis
Go to simulate select transient analysis set the stop time as 1ms and run the simulation ,The below graph shows the output of transient analysis



# INFERENCE
.For a differential amplifier to work properly, you need to set the MOSFETs in their active region (saturation region for long-channel MOSFETs). This typically involves proper sizing of resistors, current sources, and gate voltages
. Varry the MOSFET length and width (m1&m2)get calculated id current in dc analysis
.set the Ac amplitude as 1 in the ac analysis
. From the frequency response, you can determine the bandwidth of the differential amplifier by identifying the frequency
