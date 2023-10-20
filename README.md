# DigComm_Lab4

## Amplitude Shift Keying

Amplitude shift keying is the act of modulating symbols via changes in amplitude for transmitted signal. In this lab, we built an RF ASK signal

1. What is the relationship between the digital signal and the presence of the carrier in the ASK signal?

As shown in the below image, symbols for the ASK signal are transmitted by either the carrier signal being active or inactive. In other words, the signal is transmitted so that a 1 is the carrier signal frequency and a 0 is no transmission.
![Image](https://github.com/Ryankearns9/DigComm_Lab4/blob/main/imgs/picture_1.png)



2. What is the ASK signal's voltage when the digitial signal is logic-0? **Tip**: If you're not sure, briefly set the Channel 2 *Input Coupling* control to the GND

As shown in the below image, the ASK signal has a max voltage of 10V and a minimum voltage of -10V. That gives the peak to peak voltage of 20V


3. What feature of the ASK signal suggests that it's an AM signal? **Tip**: If you're not sure, see the preliminary discussion

As shown in the below signal, it can be seen that the signal is AM because the amplitude is changing over time due to the modulation. When a 1 is transmitted, the signal has a high amplitude and when it is a 0, it is a low amplitude. Amplitude modulation is the act of transmitting information via altering the amplitude of the signal. That alteration of signal amplitude is clearly displayed in the below plot

![Image](https://github.com/Ryankearns9/DigComm_Lab4/blob/main/imgs/picture_2.png)



4. Why is the recovered digital signal not a perfect copy of the original?

The below two images shows the recovered signal after passing through the low pass filter. Image 1 displays the signal with a wide frequency passband and image 2 shows a narrow passband. As seen, the narrow filter results in a much nosier signal. This is because a square wave requires an infinite passband to show perfectly reconstruct the signal. Anything less than infinite results in the Gibb's Phenomenom. The act of filtering out the signal is preventing a perfect reconstruction of the original signal.

**Figure: Wideband filter**
![alt text](https://github.com/Ryankearns9/DigComm_Lab4/blob/main/imgs/picture_3a.png)

**Figure: Narrowband filter**
![alt text](https://github.com/Ryankearns9/DigComm_Lab4/blob/main/imgs/picture_3b.png)



5. What can be used to "clean-up" the recovered digital signal?

A Schmitt Trigger or a comparator can be used to clean up the signal. In both cases, these modifications can be used to assign a 1 to a signal above a certain amplitude and a 0 to a signal below a certain amplitude. In the case of the comparator the signal is compared to a reference voltage. If it is above the reference voltage, it is assigned a 1 or high output. If it is below the reference voltage, it is assigned a 0 or low output. 

**Figure: Wideband filter after comparitor**
![alt text](https://github.com/Ryankearns9/DigComm_Lab4/blob/main/imgs/picture_4a.png)

**Figure: Lowband filter after comparitor**
![alt text](https://github.com/Ryankearns9/DigComm_Lab4/blob/main/imgs/picture_4b.png)




6. How does the comparator turn the slow rising voltages of the recovered digital signal into the sharp transition?

As mentioned in the previous section, the comparator fixes the signal by transmitting either a high or low output based on whether the signal is above or below the referenced voltage. This creates a sharp output because it ignores how far away the signal is from the reference and instead just looks to see if the signal is above or below.


Frequency Shift Keying

1. What's the name of the VCO output frequency that correspods with the logic-1s in the ditial data? **Tip:** If you're not sure, see the preliminary discussion

The "Mark frequency" is the frequency that corresponds to 1's. As shown in the below figure, this is the higher frequency 

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/blob/main/imgs/FSK_Pic1.PNG)

2. What's the name for the VCO output frequency that corresponds with the logic-0s in the digital data?

The logical 0's correspond to the "Space frequency". As shown in the above figure, this is the lower of the two frequencies


3. Based on the observations of the FSK signal, which of the two is the higher frequency? Explain the answer

As noted above, the higher frequency is the 1's. Also called the "Mark Frequency." This can be seen visually with the applied graph but can also be understood by looking at the equation FM transmission taken from the Lecture 3 slides. See below:

$A_c\cos()$

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/blob/main/imgs/Bandpass.PNG)

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/blob/main/imgs/FSK_Pic2_LPF.PNG)

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/blob/main/imgs/FSK_Comparator.PNG)

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/blob/main/imgs/FSK_baseband_filter_withGain.PNG)

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/blob/main/imgs/FSK_baseband_filter.PNG)

4. Which of the FSK signal's two sinewaves is the filter picking out?
5. What does the filtered FSK signal look like?
6. What is used to "clean up" the recovered digital data?
7. How does the comparator turn the slow rising voltages of the recovered digital signal into sharp transitions?