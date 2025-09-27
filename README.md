# 6.-Design-and-Simulation-of-step-up-chopper
## AIM
To design, simulate and analyse a stepup chopper or Boost converter using MATLAB Simulink.
## APPARATUS REQUIRED
	MATLAB
## PROCEDURE
	1.	Open MATLAB and click on the icon for SIMULINK as shown below
 <img width="522" height="376" alt="image" src="https://github.com/user-attachments/assets/f9fe23e6-5f4c-431b-a490-15d58a4e068d" />

Another way is to open is through START icon of MATLAB Start ⇒ Simulink ⇒ Library  browser. 

2.	Click on NEW MODEL or go to FILE ⇒ NEW ⇒ MODEL and a new blank model is created as shown below
 <img width="572" height="382" alt="image" src="https://github.com/user-attachments/assets/9e6206f8-7b9a-4713-bf1e-72cd04f3a256" />

3.	After creating a blank model you need to open the SIMULINK component storeroom/library by going to View ⇒ Library Browser. Select SIMPOWER SYSTEMS then select Power Electronics library and by right clicking on MOSFET and click on add to the model will add the MOSFET in the blank model. Alternatively you can drag the component directly in the model page as shown below
 <img width="940" height="361" alt="image" src="https://github.com/user-attachments/assets/f301d0d1-91d8-4f98-bd3f-6d1be5551780" />

4.	Similarly go to ELECTRICAL SOURCES ⇒ AC Voltage Source and add it to the model. Select Elements and select “SERIES RLC BRANCH” and add it to the model. Simulink do not perform simulation unless and until a measurement block is present in a system. Since we need to measure the input and output voltages and the load current. To add them select Measurement in SIMPOWER SYSTEMS and then add current measurement and voltage measurement blocks to the model. Oscilloscope is not included in SIMPOWER SYSTEMS and is present in the top most block of the left column that is SIMULINK ⇒ Sinks ⇒ Scope. Also add PWM generator from sourced. We can join various blocks by clicking on their edges and then drag the wire till the other connection terminal.
5.	Construct the circuit by joining them together in the form as given below
 <img width="940" height="342" alt="image" src="https://github.com/user-attachments/assets/dd7a66df-45e5-4889-af73-8632079d2880" />

6.	Double click on series RLC branch, Select the Branch type as R and set the values for R.
7.	Double click on PWM generator, set the parameter as per the requirement.
<img width="499" height="386" alt="image" src="https://github.com/user-attachments/assets/40815c63-ac76-4d7f-9ebd-8aa0665a7b42" />

 
8.	Before running the simulation, we have to configure the parameters. Go to Simulation ⇒ Configuration parameters as shown
 <img width="542" height="399" alt="image" src="https://github.com/user-attachments/assets/87797881-f363-4fe6-8cdc-e16c0a65b789" />

9.	Select the ode23tb (Stiff/TR-BDF2) or ode15s (Stiff/NDS) or any suitable solver as
shown below 
 <img width="566" height="401" alt="image" src="https://github.com/user-attachments/assets/5f32e169-862f-47c3-a8df-71a9351e7d96" />

10.	Start the simulation and Double click on scope and observe the graphs.


## Exercise 1
Design a step up chopper for the following specification
Specification
Input Voltage (Vin)=12V
Output Voltage (Vout) = 24V
Switching Frequency (Fs) = 40 KHz
Voltage Ripple (∆V) = 20mV
Current Ripple (∆I) = 2A
## Formulas to be Used
<img width="407" height="457" alt="image" src="https://github.com/user-attachments/assets/c6083c5a-a698-4499-97d4-528c43ab9ef4" />

## Simulation
![simu](https://github.com/user-attachments/assets/a85bb289-5b8e-4c31-bc50-e121b528cadf)

## Output
![graph](https://github.com/user-attachments/assets/20bd7196-9813-4ce8-9273-490de222bf45)

## Result
thus the Simulation-of-step-up-chopper in MATLAB Simulink was studied and verified
