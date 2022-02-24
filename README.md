# Talking-voltmeter-using-arduino
file links:
https://drive.google.com/drive/folders/16jtjSkmy61tPRD0kMsCotCLItTNDr7-d?usp=sharing

brief intro:
hello guys, today we are going to make a smart talking voltmeter. This one is built on Arduino and gives the reading by speaking itself. This function is cool and attractive because when we are working on circuits, we have to see again and again the readings and then switch the voltmeter leads to measure again the voltage. We will learn how to add supported libraries and where to get them, how talking function of Arduino works, how it reads the voltage and what changes should we have to do in order to increase the range and precision.
Note* For now we are considering a low voltage range from 0-5volts. Which is properly supported by Arduino. To measure high Voltages, we have to add a resistance voltage divider network and change the code accordingly the values of resistance. Every thing is mentioned in the code given below.
Components required:
1) Arduino Nano
2) Pam8403 (Class D amplifier)
3) 100k Resistor
4) Speaker
5) 100nf capacitors
6) Breadboard and wires

Working:
Through Analog functions of the microcontroller, we can read the voltage using this. But without a resistor divider network, only a small voltage can be measured (In the range of microcontroller).
Using an Arduino to measure voltages is relatively simple. Inside the Arduino, there are multiple analog input pins connecting to an analog-to-digital converter (ADC). The Arduino ADC is a ten-bit converter, and the output value ranges from 0 to 1023. We will obtain this value using the analogRead() function.
