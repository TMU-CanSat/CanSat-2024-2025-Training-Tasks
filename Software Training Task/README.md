
# SOFTWARE TRAINING TASK

# Task Description
The task is to collect data from various sensors, package it into a string, then save it to an SD card and transmit it to the host computer. Also if certain conditions are met perform an action. Use Wokwi to simulate your code and test it. https://wokwi.com/
  
1. Initialize the servo motor at 0 degrees. (5 pts)
2. Write code to read data from all the sensors listed in [Devices]. (10 pts)
3. Collect the following data points: (10 pts)
	- Temperature
	- Distance (HC-SR04) (assume that in this data collection, this is the distance from the ground)
	- Acceleration (X, Y, Z) in m^s2
	- Rotation Rate (X, Y, Z) in rad/s
	- Count (How many transmissions have been made. This should increment by 1 every time a new transmission is sent. Starts at 0.)
4. Create a string with the following format: (15 pts)
	COUNT_TEMPERATURE_DISTANCE_ACCELERATIONX_ACCELERATIONY_ACCELERATIONZ_ROTATIONX_ROTATIONY_ROTATIONZ
5. Transmit the string via Serial to the host computer at a baudrate of 115200. ( 10 pts)
6. Repeat steps 2-5 at a rate of 1 Hz until Count reaches 100. (10 pts)
7. If the Temperature reaches above 35 degrees or is equal to 35 degrees rotate the servo motor 90 degrees. (5 pts)
8. If the Temperature drops below 35 degrees return the servo motor to 0 degrees. (5 pts)
9. (BONUS) Store the string on the SD Card in a file type of your choice. Each new transmission should be saved on a new line so that all data is logged. (15 pts)
10. (**BONUS 2** ) Code something to track whether the sensor system is rising or falling using 1 or 2 of the sensors here.   (15 pts)

***Maximum 100 pts***

## Important Note
You can use any pins on the Arduino to connect the devices. As long as they work of course.
Add comments to your code to explain what is being done.
Explain your thinking if attempting Bonus 2

## Devices

<table>
  <tr>
    <td>1. Arduino Mega</td>
    <td>4. DS18B20 Temperature Sensor</td>
  </tr>
  <tr>
    <td>2. Micro SD Card Module (SPI)</td>
    <td>5. MPU6050 6-Axis Accelerometer & Gyroscope Sensor</td>
  </tr>
  <tr>
    <td>3. HC-SR04 Ultrasonic Distance Sensor</td>
    <td>6. Servo motor</td>
  </tr>
</table>

# Submission
Submit the link to your public Wokwi project in the submission form below: https://forms.gle/kebgJhdWsR92eYedA

## Resources to Look at For Help:
 - The Wokwi website is amazing, and has guides to use all of the sensors/device simulations that they run. 
 - https://docs.wokwi.com/parts/wokwi-arduino-mega
 - https://wokwi.com/projects/358129234661487617
 - https://docs.wokwi.com/parts/wokwi-microsd-card
 - https://docs.wokwi.com/parts/wokwi-mpu6050
 - https://docs.wokwi.com/parts/wokwi-hc-sr04
 - https://docs.wokwi.com/parts/wokwi-servo

