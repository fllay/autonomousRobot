# autonomousRobot
autonomous AGV

```rosrun rosserial_python serial_node.py /dev/ttyACM0```

```rosrun teleop_twist_keyboard teleop_twist_keyboard.py _speed:=0.1 _turn:=0.5```


IMU calibration


```rosrun imu_calib do_calib```
Apply imu calibration

run 

```roslaunch linorobot minimal.launch``` and wait for 
```
[INFO] [1565428616.040840]: sys = 1 gyr = 3 acc = 3 mag = 3
[ INFO] [1565428616.056373487]: Gyro calibration complete! (bias = [0.000, -0.000, -0.000])
[INFO] [1565428616.342433]: sys = 1 gyr = 3 acc = 3 mag = 3
[INFO] [1565428616.642796]: sys = 1 gyr = 3 acc = 3 mag = 3
[ INFO] [1565428616.658482660]: First pair of IMU and magnetometer messages received.```




