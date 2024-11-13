# Vehicle_Stability_System
A vehicle stability system, or Electronic Stability Control (ESC), is an automotive safety feature that improves handling by monitoring wheel speed, steering, and acceleration. If it detects potential skidding, the system adjusts braking and engine power to help the driver maintain control, reducing the risk of accidents.

## Methodology

1. **Speed Sensor Voltage Measurement**
   - Turn the ignition on and use a voltmeter set to 10 V (DC) to measure and record the speed sensor's supply voltage.

2. **Speed Signal Visualization**
   - Increase speed to 10, 20, and 40 km/h. Use an oscilloscope with specific settings to display the sensor signal.

3. **ABS on Dry Surfaces**
   - Drive at 50 km/h on a dry surface and apply the brakes at 20%, 70%, and 100% pedal pressure. Record ABS activation on each wheel.

4. **ABS on Wet Surfaces**
   - Accelerate to 50 km/h with one side of the road set to wet. Apply brakes at different intensities, recording ABS activation on specific wheels.

5. **Speed Signals During ABS Braking**
   - At 99 km/h on dry roads, apply full braking. Capture the speed signal with an oscilloscope to observe ABS response around 50 km/h.

6. **ABS Fault Diagnosis**
   - Use a diagnostic tool to check fault codes and verify wheel speed sensor output with an oscilloscope to diagnose ABS malfunctions.

7. **ASR Intervention**
   - Set one side of the road to wet, accelerate at 20%, 50%, and 100%, and observe ASR actions, including controlled braking and indicator lights.

8. **ESP Self-Test**: Turn ignition off, then to start. Observe ESP and engine LEDs for self-test activation.

9. **ESP Intervention**: Set road conditions to dry, drive at 50 km/h, then simulate oversteer/understeer with a 15° steering angle left and right. Record which wheels engage in controlled braking.

10. **CAN Bus Measurement**: Connect to the steering angle sensor, set oscilloscope to 5 V/div (Channel A) and 2 V/div (Channel B) with a 100 μs/div time base, adjust trigger, and capture CAN bus signal.


## Tools and Resources

- **Lucas Nuelle Experimental Kit**: Used for hands-on experimentation with vehicle stability components, including ABS and ASR testing setups.

- **MATLAB and Google Colab**: Utilized for data visualization and analysis, enabling a deeper understanding of speed sensor signals and ABS/ASR response under varying conditions.

- **OBD-II Diagnostic Tools**: Employed for reading vehicle diagnostics and sensor data. These include:
  - **OBD-II Scanner**: For accessing and interpreting fault codes related to ABS and stability control systems.
  - **OBD-II Cables**: Used to connect the diagnostic scanner to the vehicle for real-time data capture.

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
1. Fault Code Reading:
The technician used a diagnostic tool to read the fault memory of the vehicle's electronic control unit (ECU).
The fault code indicated a potential issue with the wheel speed sensor.
2. Physical Measurements:
The technician likely used an oscilloscope to analyze the electrical signals from the wheel speed sensor.
This would involve checking the sensor's output voltage, signal frequency, and waveform shape.
By comparing the measured values to the expected values, the technician could determine if the sensor was functioning correctly.

## 7)
ASR intervention
We will now learn about the action of ASR under various driving circumstances and road conditions.
Experiment setup:
Set the board as described next
1. Set the right-hand roadway condition to wet.

Set the accelerator pedal to 100%. What do you observe on the board?
The front right wheel undergoes controlled braking.
The ASR control lamp shines while the ASR is active.
The motor for building up brake pressure operates.

Brake the vehicle again, then operate the accelerator pedal once more as indicated below
and specify whether or not the ASR intervenes in each case.
Accelerator pedal at 20%
Accelerator pedal at 50%
Accelerator pedal at 100%

## 8)
ESP self-test
ESP performs a self-test when the vehicle is started.
Experiment setup:
Set the board as follows:
1. Turn the ignition switch fully to the left (OFF).
2. Now turn the ignition switch fully to the right to simulate starting of the vehicle.
3. Observe the LED's for the ESP and engine.

## 9)
ESP intervention
Experiment setup:
Set the board as follows:
1. Set both roadway conditions to dry.

Set the speed to about 50 km/h. Then select whether the vehicle should oversteer or
understeer, and change the steering angle as indicated below. In which situations do which
wheels undergo controlled braking?
Oversteer - steering
angle of 15° to the left
Oversteer - steering
angle of 15° to the right
Understeer - steering
angle of 15° to the left
Understeer - steering
angle of 15° to the right

## 10)
CAN bus measurement
We will now record the CAN bus signal from the steering angle sensor.
Experiment setup:
1. Connect the measuring leads as shown below.
![image](https://github.com/user-attachments/assets/8db680b5-77d8-4692-9742-e68d98c7ab4e)
Open the Oscilloscope from the menu
Instruments/Measuring Devices.
Select the following settings:
Channel A: 5 V / div; DC; Y-POS: -
Channel B: 2 V / div; DC; Y-POS: -
Time: 100 μs / div
Mode: X/T
2. Move the trigger upward by one and a half divisions.

## Results

1. **Speed Sensor Supply Voltage**: Measured accurate voltage supply to speed sensor, ensuring functionality.
2. **Speed Sensor Signal**: Successfully visualized speed signals at various speeds, confirming sensor responsiveness.
3. **ABS on Dry Surface**: Observed ABS activation at different braking intensities, with controlled braking in dry conditions.
4. **ABS on Wet Surface**: Noted ABS intervention and stability differences under wet-road braking.
5. **Speed Signal During ABS**: Monitored speed signal during full braking, observing expected deceleration patterns.
6. **ABS Fault Diagnosis**: Detected ABS malfunction via fault codes, identifying wheel speed sensor issues.
7. **ASR Intervention**: Recorded ASR activity under different acceleration levels on wet surfaces, with controlled braking observed.
8. **ESP Self-Test**: Observed ESP self-check on ignition, confirming activation as designed.
9. **ESP Intervention**: Verified ESP-controlled braking under simulated oversteer/understeer scenarios.
10. **CAN Bus Measurement**: Captured CAN bus signal from steering sensor, validating correct signal transmission.

## Skills Acquired

- **Diagnostic and Measurement Techniques**: Gained proficiency in using diagnostic tools (oscilloscope, voltmeter) for accurate voltage and signal measurements.
- **Sensor Data Analysis**: Developed skills in analyzing data from speed and steering angle sensors.
- **Vehicle Stability System Testing**: Practiced configuring and testing ABS, ASR, and ESP systems under various road and driving conditions.
- **CAN Bus Signal Analysis**: Learned to record and interpret CAN bus signals, essential for understanding in-vehicle communication networks.
- **Practical Problem-Solving**: Enhanced ability to troubleshoot system faults, identify issues, and understand real-world vehicle dynamics.

## Importance of the Project

This project underscores the critical role of Electronic Stability Control (ESC) and related systems (ABS, ASR, ESP) in enhancing vehicle safety and control. By simulating real-world conditions and faults, the project provides valuable insight into how these systems prevent skidding, maintain stability, and assist drivers in emergencies. The hands-on experience with diagnostics and stability control systems equips students with practical knowledge applicable to automotive safety, diagnostics, and repair, preparing them for real-world applications in the automotive industry.

## Conclusion

The practicals confirmed the effectiveness of the vehicle stability systems (ABS, ASR, ESP) under various conditions, highlighting their crucial role in safety. Accurate diagnostics and measurements demonstrated the systems’ responsiveness to different road conditions, braking intensities, and steering inputs, providing insight into their operational reliability and performance.


