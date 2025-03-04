# Experiment--03
# Design Differential amplifier for the following specification vdd=3.3v p<=3mw vicm=1.72v vocm=1.81v vp=0.7v perform dc analysis,transient analysis,ac analysis and extract required parameter 
# Calculation
![Uploading 9dda96d1-906f-4a08-a816-1cbf0d3b29d7.jfif…]()

   
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
