# IMU Sensor (Inertial Measurement Unit):
- A device that combines accelerometers, gyroscopes, and sometimes magnetometers to measure an object's motion, orientation, and direction relative to a reference point.

 - IMUs are used in various applications requiring motion tracking, orientation sensing, and stabilization, such as:
 - IMUs in autonomous vehicles provide real-time data on motion, aiding navigation, localization, and control by precisely determining position, orientation, and velocity, even in challenging conditions.

`Accelerometers` are sensors that measure acceleration, either linear or gravitational.\
`Magnetometers` are sensors that measure the strength and direction of magnetic fields.\
`Gyroscopes` are sensors that measure angular velocity or rate of rotation.\


## MPU 6050:
- The MPU 6050 is a popular and widely used IMU sensor from InvenSense.
- It is a 6-degree-of-freedom motion sensor module combining a 3-axis accelerometer and a 3-axis gyroscope, commonly used in robotics and motion tracking applications.
- It combines:
    - A 3-axis gyroscope to measure angular velocity.
    - A 3-axis accelerometer to measure acceleration.

<hr />

### To connect the MPU6050 IMU sensor to the Jetson Nano, follow these wiring instructions:

1. Connect VCC (Voltage) of the MPU6050 to the 3.3V pin on the Jetson Nano (e.g., pin 1 or pin 17).
2. Ground the GND (Ground) pin of the MPU6050 to a Ground pin on the Jetson Nano (e.g., pin 6 or pin 25).
3. Connect SCL (Serial Clock) from the MPU6050 to the SCL pin on the Jetson Nano (pin 5).
4. Connect SDA (Serial Data) from the MPU6050 to the SDA pin on the Jetson Nano (pin 3).

After wiring, use the following command to verify the connection and detect the MPU6050:
```bash
sudo i2cdetect -y 1
```