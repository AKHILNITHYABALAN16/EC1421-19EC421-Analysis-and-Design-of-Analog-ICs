# EC1421-19EC421-Analysis-and-Design-of-Analog-ICs
# DESIGN OF ACTIVE LOW PASS,HIGH PASS AND BAND PASS FILTERS USING OP-AMP 

## AIM: 

To design and obtain the frequency response of 
i) First order Low Pass Filter (LPF) 
ii) First order High Pass Filter (HPF) 
iii) Band pass filter
 
## APPARATUS REQUIRED

<img width="625" height="170" alt="image" src="https://github.com/user-attachments/assets/900fc8b3-3a8c-4208-bf52-98cc9e281e21" />

## THEORY
## LOW PASS FILTER 
 A LPF allows frequencies from 0 to higher cut of frequency, fH.  At fH the gain is 0.707 
Amax, and after fH gain decreases at a constant rate with an increase in frequency.  The gain 
decreases 20dB each time the frequency is increased by 10.  Hence the rate at which the gain 
rolls off after fH is 20dB/decade or 6 dB/ octave, where octave signifies a two fold increase in 
frequency.  The frequency f=fH is called the cut off frequency because the gain of the filter at this 
frequency is down by 3 dB from 0 Hz.  Other equivalent terms for cut-off frequency are -3dB 
frequency, break frequency, or corner frequency.
# HIGH PASS FILTER 
The frequency at which the magnitude of the gain is 0.707 times the maximum value of 
gain is called low cut off frequency.  Obviously, all frequencies higher than fL are pass band 
frequencies with the highest frequency determined by the closed –loop band width all of the op
amp. 
# BAND PASS FILTER 
A band pass filter has a pass band between two cutoff frequencies fH and fL such that fH > 
fL.  Any input frequency outside this pass band is attenuated.  There are two types of band-pass 
filters.  Wide band pass and Narrow band pass filters.  We can define a filter as wide band pass if 
its quality factor Q <10.  If Q>10, then we call the filter a narrow band pass filter.  A wide band 
pass filter can be formed by simply cascading high-pass and low-pass sections.  The order of 
band pass filter depends on the order of high pass and low pass sections.

## CIRCUIT DIAGRAM: 
## LOW_PASS

<img width="1280" height="792" alt="image" src="https://github.com/user-attachments/assets/24f03094-d172-4b50-92f4-ef6a84e3b109" />

## HIGH-PASS

<img width="1250" height="838" alt="image" src="https://github.com/user-attachments/assets/0321f4d9-2d71-43dc-98ec-aeabd5cef3a0" />

## BAND-PASS

<img width="1155" height="688" alt="image" src="https://github.com/user-attachments/assets/61c5cbea-5abd-4fe7-b4d8-fba6eb736257" />


## MODEL GRAPH:
## LOW_PASS

<img width="1142" height="836" alt="image" src="https://github.com/user-attachments/assets/dcb5a63f-d56e-457e-b27d-9bd21b8612e6" />

## HIGH-PASS

<img width="1158" height="860" alt="image" src="https://github.com/user-attachments/assets/3355ed3e-0d1e-409f-a5ca-52fd56389d50" />

## BAND-PASS

<img width="1060" height="866" alt="image" src="https://github.com/user-attachments/assets/bac3c4f5-dea6-4cc6-bc10-b0d817628175" />


## PROCEDURE - (LPF & HPF): 
1. Connect the circuit as shown in the circuit diagram. 
2. Select the corresponding cut-off frequency (higher or lower) and determine the value of C&R. 
select the value of R1 & Rf depending on desired passband gain Af.. 
3. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
4. Tabulate the output voltage Vo with respect to different values of input frequency. 
5. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to  get approximately the same characteristic as shown in the model graph. 
# PROCEDURE:BAND PASS FILTER 
1. Select the lower and higher cut-off frequency and calculate the value of R & C for the given 
frequencies. 
2. Design for LPF & HPF separately and then combine the circuit by first placing the HPF 
followed by a LPF (i.e) HPF in series with LPF. 
3. Connect the circuit as shown in the circuit diagram. 
4. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
5. Tabulate the output voltage Vo with respect to different values of input frequency. 
6. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to get approximately the same characteristic as shown in the model graph

## DESIGN:LPF & HPF:

<img width="429" height="324" alt="image" src="https://github.com/user-attachments/assets/b0f0ac0a-3006-494c-9096-e91ae2d6e87c" />

# DESIGN: BAND PASS FILTER
Design a BPF to pass a band of 400Hz to 2KHz with a pass band gain of 4.  
1. Select the highest cut-off frequency of LPF as fH = 10 KHz and the lowest cut-off frequency 
of HPF as fL = 1 KHz.  
2. Design the HPF first by taking fL = 1KHz. Assume the value of C < 1μf.  
Let C = 0.1μf.  
3. Calculate R from the expression.  
Given: fH = 2KHz  = 1/ (2πR1C1) 
   Let C1 = 0.1 µF, R1 = 7.9 KΩ 
Given: fL = 400Hz  = 1/ (2πR2C2) 
   Let C2 = 0.1 µF, R2 = 39.8 KΩ 
  Pass band Gain=4 
   Now   Ao = 1 + (Rf / R1)  
               2-1=(Rf / Ri) 
                Ri = Rf 
                 Let  Ri = Rf = 10 KΩ
## TABULATION:
## LOW_PASS

<img width="1089" height="924" alt="image" src="https://github.com/user-attachments/assets/a137de47-b5c5-4c11-9b73-4353b32d3f7a" />

## HIGH-PASS

<img width="1280" height="1213" alt="image" src="https://github.com/user-attachments/assets/b3657150-9e01-44a0-a67f-55c7c3adfa50" />

## BAND-PASS

<img width="1280" height="1156" alt="image" src="https://github.com/user-attachments/assets/d8511a3a-c5f7-4992-be18-105451e2a4d3" />

## GRAPH:
## LOW_PASS

<img width="1280" height="829" alt="image" src="https://github.com/user-attachments/assets/456d8123-e791-4faf-9513-b412db711a62" />

## HIGH-PASS

<img width="1280" height="857" alt="image" src="https://github.com/user-attachments/assets/1daa53d1-0635-4d40-9488-f6393ba1140e" />

## BAND-PASS

<img width="1280" height="809" alt="image" src="https://github.com/user-attachments/assets/7054c283-af94-4b74-9576-9d5fdcb546e1" />

 ## RESULTS:
Thus an Active Low pass, High pass and Band Pass Filters are designed and 
tested using op-amp IC 741. 

