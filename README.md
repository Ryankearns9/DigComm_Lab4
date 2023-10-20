# DigComm_Lab4

## Amplitude Shift Keying

Amplitude shift keying is the act of modulating symbols via changes in amplitude for transmitted signal. In this lab, we built an RF ASK signal

1. What is the relationship between the digital signal and the presence of the carrier in the ASK signal?

As shown in the below image, symbols for the ASK signal are transmitted by either the carrier signal being active or inactive. In other words, the signal is transmitted so that a 1 is the carrier signal frequency and a 0 is no transmission.
![Screenshot]\(https://github.com/Ryankearns9/DigComm_Lab4/tree/main/imgs/picture_1.png)



2. What is the ASK signal's voltage when the digitial signal is logic-0? **Tip**: If you're not sure, briefly set the Channel 2 *Input Coupling* control to the GND

![Image]\(https://github.com/Ryankearns9/DigComm_Lab4/tree/main/imgs/picture_2.png)



3. What feature of the ASK signal suggests that it's an AM signal? **Tip**: If you're not sure, see the preliminary discussion

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/tree/main/imgs/picture_3a.png)

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/tree/main/imgs/picture_3b.png)

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/tree/main/imgs/picture_4a.png)

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/tree/main/imgs/picture_4b.png)

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/tree/main/imgs/picture_5a.png)

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/tree/main/imgs/picture_5b.png)

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/tree/main/imgs/picture_5c.png)

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/tree/main/imgs/picture_5d.png)

4. Why is the recovered digital signal not a perfect copy of the original?
5. What can be used to "clean-up" the recovered digital signal?
6. How does the comparator turn the slow rising voltages of the recovered digital signal into the sharp transition?

Frequency Shift Keying

1. What's the name of the VCO output frequency that correspods with the logic-1s in the ditial data? **Tip:** If you're not sure, see the preliminary discussion

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/tree/main/imgs/Bandpass.PNG)

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/tree/main/imgs/FSK_Pic1.PNG)

![alt text](https://github.com/Ryankearns9/DigComm_Lab4/tree/main/imgs/FSK_Pic2_LPF.PNG)

2. What's the name for the VCO output frequency that corresponds with the logic-0s in the digital data?
3. Based on the observations of the FSK signal, which of the two is the higher frequency? Explain the answer
4. Which of the FSK signal's two sinewaves is the filter picking out?
5. What does the filtered FSK signal look like?
6. What is used to "clean up" the recovered digital data?
7. How does the comparator turn the slow rising voltages of the recovered digital signal into sharp transitions?