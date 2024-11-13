# Vehicle_Stability_System
A vehicle stability system, or Electronic Stability Control (ESC), is an automotive safety feature that improves handling by monitoring wheel speed, steering, and acceleration. If it detects potential skidding, the system adjusts braking and engine power to help the driver maintain control, reducing the risk of accidents.

## Description
## 1)
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
## 2)
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
![image](https://github.com/user-attachments/assets/e0e4add8-70ad-487d-8a8a-3118fb99409b)

Repeating the practical for spees 20km/hr and 40 Km/hr as well
## 3)
ABS braking on dry surfaces
Experiment setup:
For the first test, set the board as described next.
1. Move the switch for the right-hand roadway condition to the dry setting.
2. Move the switch for the left-hand roadway condition to the dry setting.
3. Turn the ignition switch fully to the right.
4. Move the brake control to the zero setting.
5. Move the accelerator pedal control to the zero setting.

Increase the vehicle's speed to 50 km/h, and then brake the vehicle in a controlled manner.
After that, accelerate the vehicle again to investigate the braking performance at different
applied forces. Determine whether or not the ABS intervenes.
Brake pedal depressed about 20%
Brake pedal depressed about 70%
Brake pedal depressed about 100%

Determine whether or not the ABS intervenes and in which wheel brake?
Front left wheel brake
Front right wheel brake
Rear left wheel brake
Rear right wheel brake

## 4)
ABS braking on wet surfaces
Experiment setup:
For the first test, set up the board as described next.
1. Increase the speed to 50 km/h (leave the roadway condition dry to be able to accelerate
more rapidly).
2. Once the set speed has been attained, move the switch for the right-hand roadway condition
to the wet setting.
3. Leave the left-hand roadway condition dry.

Brake the vehicle in a controlled manner. After that, accelerate the vehicle again to
investigate the braking performance at different applied forces. Determine whether or not the
ABS intervenes.
Brake pedal depressed about 20%
Brake pedal depressed about 70%
Brake pedal depressed about 100%

In which wheel brake does the ABS control unit intervene?
Front left wheel brake
Front right wheel brake
Rear left wheel brake
Rear right wheel brake

## 5)

Speed signals during braking by the ABS
We will now study the speed signal during ABS braking.
1. Set both roadway conditions to dry.
2. Set the speed to 99 km/h.
3. Connect the measuring leads as shown below to register the speed signal.

In the oscilloscope set its parameters as shown below.
Channel A: 2 V / div; DC; Y-POS: -
Channel B: 2 V / div; DC; Y-POS: -
Time: 50 ms / div
Mode: X/T

1. Set the brake pedal to 100% to simulate full braking.
2. Drag & drop the graph obtained at about 50 km/h to the placeholder provided below.
![image](https://github.com/user-attachments/assets/78f8e6d7-a10b-49a1-b8c4-cac8dee1fe0a)

## 6)
Workshop order: ABS | A customer has complained that the ABS indicator lamp in their car stays on all the time.
![image](https://github.com/user-attachments/assets/e43062b1-3231-469a-8c27-6216c9dd3a4d)

The diagnosis of the ABS malfunction was carried out through a combination of fault code reading and physical measurements. Here's a breakdown of the steps:
## 1. Fault Code Reading:
The technician used a diagnostic tool to read the fault memory of the vehicle's electronic control unit (ECU).
The fault code indicated a potential issue with the wheel speed sensor.
## 2. Physical Measurements:
The technician likely used an oscilloscope to analyze the electrical signals from the wheel speed sensor.
This would involve checking the sensor's output voltage, signal frequency, and waveform shape.
By comparing the measured values to the expected values, the technician could determine if the sensor was functioning correctly.


