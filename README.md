# Vehicle_Stability_System
A vehicle stability system, or Electronic Stability Control (ESC), is an automotive safety feature that improves handling by monitoring wheel speed, steering, and acceleration. If it detects potential skidding, the system adjusts braking and engine power to help the driver maintain control, reducing the risk of accidents.

## Description
Experiment setup
The experimental board is shown below. In this measurement, we will determine the speed
sensor's supply voltage.

![Screenshot 2024-11-13 141811](https://github.com/user-attachments/assets/b300bf2d-9db8-4c73-b89e-5e3534a3173f)

1. Turn the ignition switch fully to the right.
2. Under Instruments => Measuring devices, open voltmeter A and set it to a measuring range of 10 V.
Open voltmeter A from the menu Instruments/Measuring Devices.
Make the following settings:
RANGE: 10 V | MODE: RMS | DC
![image](https://github.com/user-attachments/assets/0c674a2f-bfac-4b99-afa1-2c1a628ae322)

-> The supply voltage to the speed sensor____ volts

Now let's visualize the speed sensor's signal:

1. Turn the ignition switch fully to the right.
2. Raise the speed to 10 km/h.
3. Open the oscilloscope.

Open the Oscilloscope from the menu Instruments/Measuring Devices.
Select the following settings:
Channel A: 5 V / div; DC; Y-POS: -
Channel B: - / div; -; Y-POS: -
Time: 20 ms / div | Mode: X-T | Trigger: CHANNEL Channel A; Rising Edge;
LEVEL: 0,5 Division div; PRETRIGGER: 2 | Division div; ; Standard

Repeating the practical for spees 20km/hr and 40 Km/hr as well

