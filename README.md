# K64F-Serial-Communication

This project demonstrates real-time sensor communication using UART, SPI, and I²C protocols with the K64F microcontroller and the onboard FXOS8700CQ accelerometer/magnetometer sensor. Sensor data is transmitted to both a PC terminal and an Arduino Uno, showcasing how multiple embedded communication methods can be implemented and verified using a digital storage oscilloscope.

Features
I²C: Reads sensor data from the FXOS8700CQ  
UART: Sends formatted data to a PC serial terminal  
SPI: Transmits data to an Arduino Uno configured as an SPI slave  
Oscilloscope Analysis: Captures waveforms of data transmissions  
Latency Measurement: End-to-end SPI latency measured at ~13 μs, consistent with the 374.49 kHz SPI clock rate  

Hardware
NXP FRDM-K64F Development Board  
FXOS8700CQ Sensor (onboard K64F)  
Arduino Uno  
Mixed Signal Oscilloscope  

Code Files
K64F main.c: Runs on the K64F; reads sensor data and sends over UART and SPI  
Arduino Uno main.c: Receives SPI transmissions and prints them to the serial monitor  

Results
Verified complete system communication across I²C, UART, and SPI  
Confirmed accurate UART transmission of "Who Am I" sensor ID  
Measured SPI transmission latency of 13 microseconds  
Oscilloscope waveforms confirmed transmission integrity  

Authors
Micheal Dominguez
Kevin Wu
