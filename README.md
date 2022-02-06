# PLL 
The phase-locked loop (PLL) block is a feedback control system that automatically adjusts the phase of a locally generated signal to match the phase of an input signal. PLLs operate by producing an oscillator frequency to match the frequency of an input signal.
## Basic Components:
![image](https://user-images.githubusercontent.com/97835399/152667557-79e4e8b1-c343-43c9-9e7e-6e2f105998bf.png)
## EDA Tools:
1) Ngspice  
2) Magic 
## Pre-Layout Simulation:
Pre-Layout Simulation consist of the Circuit Level Simulation using Ngspice Tool. The Prelayout Simulation of the following subcircuits are given below:
### 1) Phase Frequency Detector:
Phase Frequency Detector Compares the Reference signal with the input signal with help of 2 flip-flops (which is used to detect the falling edge of two different signals )and a delay element.

![image](https://user-images.githubusercontent.com/97835399/152669130-dd9f5ce3-8da2-40d4-b674-93f8b6d9bf3d.png)
The output waveform for the Phase Frequency Detector using Ngspice is given below-
![image](https://user-images.githubusercontent.com/97835399/152668589-71480067-c89c-474c-8c06-ba47f22d0ea5.png)
### 2) Charge Pump: 
![image](https://user-images.githubusercontent.com/97835399/152669191-6fc6af62-4c3d-4d2a-87cd-aaa40abca93b.png)

Charge Pump Converts the digital Phase Frequency Signal into an analog control signal which is given to the oscillator. The principle of the Charge can be realized by the use of Current Steering Circuit. The complete operation of the Charge Pump is based on the average timing of the UP/DOWN ouput signal of PFD.

The output waveform for the Charge Pump using Ngspice is given below-

![image](https://user-images.githubusercontent.com/97835399/152668993-3a589a8e-eb47-45c0-8e5c-600d70eb2939.png)
![image](https://user-images.githubusercontent.com/97835399/152668959-efd41df1-df70-45ab-add0-bde44346a01c.png)
### 3) Voltage Controlled Oscillator :
The basic Component of the VCO is ring Oscillator Which is the series Combination of the odd no of inverters which has certain delay associated with it this causes a output signal to flip after a certain delay. To make the fixed frequency of the ring to variable we need one additional circuit where two current sources are used as supplies at the top and bottom this is known as current straving mechansim.
![image](https://user-images.githubusercontent.com/97835399/152669569-54b26fff-a683-497e-a827-3d62437a3fc2.png)
 
 Output waveform for the VCO using Ngspice is given below-
 ![image](https://user-images.githubusercontent.com/97835399/152669625-46cc5e6c-b089-4bf0-865a-08915e5a3e2f.png)

### 4) Frequency Divider:
Frequency Divider circuit is connected through the feedback loop. This is done through the Toggle Flip flop the output of the toggle flip flop is half the frequemcy of the input signal.The toggle flip flop in the frequency divider circuit can be relaised with the help of inverters and Transmission Gates which is shown below.
![image](https://user-images.githubusercontent.com/97835399/152670809-a95425ae-0d0f-4eb4-95aa-7b165e5646b4.png)

Output waveform for the Frequency Divider using Ngspice is given below :
![image](https://user-images.githubusercontent.com/97835399/152670912-525dcbcc-a728-48e4-930f-f8426f4e79b6.png)
## Post Layout Simulation: 
to be cont..










