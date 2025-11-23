# -Frequency-Modulation-and-Demodulation-using-NumPy-and-Matplotlib-

__Aim:__

To implement and analyze frequency modulation (FM) using Python's NumPy and Matplotlib libraries.

__Apparatus Required:__ 

1. Software: Python with NumPy and Matplotlib libraries
   
2. Hardware: Personal Computer

 
__Theory:__

Frequency Modulation (FM) is a method of transmitting information over a carrier wave by varying its 
frequency in accordance with the amplitude of the input signal (message signal). The frequency of the carrier 
wave is varied according to the instantaneous amplitude of the message signal.

__Algorithm:__

1. Initialize Parameters: Set the values for carrier frequency, message frequency, sampling frequency, and 
   frequency deviation.
   
2. Generate Time Axis: Create a time vector for the signal duration.
    
3. Generate Message Signal: Define the message signal as a cosine wave.
    
4. Compute the Integral of the Message Signal: Calculate the integral of the message signal over time.
    
5. Generate FM Signal: Apply the FM modulation formula to obtain the modulated signal.
 
6. Plot the Signals: Use Matplotlib to plot the message signal, carrier signal, and modulated signal.

__Programme:__

```
import numpy as np
import matplotlib.pyplot as plt
Am = 6
fm = 476
Ac = 12
fc = 4760
fs = 47600
b = 6.1
t=np.arange(0, /fm, 1/fs)
m = Am*np.cos(2*3.14*fm*t)
plt.subplot(3,1,1)
plt.plot(t,m)
c= Ac*np.cos(2*3.14*fc*t)
plt.subplot(3,1,2)
plt.plot(t,c)
s=Ac*np.cos(2*3.14*fc*t+b*np.sin(2*3.14*fm*t))
plt.subplot(3,1,3)
plt.plot(t,s)
```
__Tabulation:__

<img width="3312" height="2088" alt="image" src="https://github.com/user-attachments/assets/dd0ab2db-6877-4801-a243-acdc8935e7f5" />



__Output:__

<img width="877" height="655" alt="image" src="https://github.com/user-attachments/assets/06aa84f1-ee1a-441d-a7e3-4cacbce0638e" />


__Result:__

Thus the FM Modulation is generated using python and the output is verified.
