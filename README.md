# autonomousRobot

***autonomous AGV***


Create catkin workspace 



```console
$ mkdir -p ~/catkin_ws/src
$ cd ~/catkin_ws/
$ catkin_make 
```


```rosrun rosserial_python serial_node.py /dev/ttyACM0```

```rosrun teleop_twist_keyboard teleop_twist_keyboard.py _speed:=0.12 _turn:=1.0```


IMU calibration

Run the following command and follow the insturctions.

```rosrun imu_calib do_calib```

After ca;ibration is done. imu calibration can be tested using 

```rosrun imu_calib apply_calib ```

If everything is ok. we can start the robot using.

```roslaunch linorobot minimal.launch``` 

and wait for 

```ruby[ INFO] [1565444505.368941652]: Calibrating gyros; do not move the IMU
[ WARN] [1565444512.353489593]: Still waiting for data on topics /imu/data_raw and /imu/mag...
[ WARN] [1565444522.353166997]: Still waiting for data on topics /imu/data_raw and /imu/mag...
[ WARN] [1565444532.352596657]: Still waiting for data on topics /imu/data_raw and /imu/mag...
[ INFO] [1565444535.280895852]: Gyro calibration complete! (bias = [0.000, 0.000, -0.000])
[ INFO] [1565444535.883415191]: First pair of IMU and magnetometer messages received.
```


***Utilities***


Get disk usages

Installation

```console
$ sudo apt-get install ncdu 
```

Usage

Just type ```console ncdu [path]``` in the command line. After a few seconds for analyzing the path, you will see something like this:

```ruby
$ ncdu 1.11 ~ Use the arrow keys to navigate, press ? for help
--- / ---------------------------------------------------------
.  96,1 GiB [##########] /home
.  17,7 GiB [#         ] /usr
.   4,5 GiB [          ] /var
    1,1 GiB [          ] /lib
  732,1 MiB [          ] /opt
. 275,6 MiB [          ] /boot
  198,0 MiB [          ] /storage
. 153,5 MiB [          ] /run
.  16,6 MiB [          ] /etc
   13,5 MiB [          ] /bin
   11,3 MiB [          ] /sbin
.   8,8 MiB [          ] /tmp
.   2,2 MiB [          ] /dev
!  16,0 KiB [          ] /lost+found
    8,0 KiB [          ] /media
    8,0 KiB [          ] /snap
    4,0 KiB [          ] /lib64
e   4,0 KiB [          ] /srv
!   4,0 KiB [          ] /root
e   4,0 KiB [          ] /mnt
e   4,0 KiB [          ] /cdrom
.   0,0   B [          ] /proc
.   0,0   B [          ] /sys
@   0,0   B [          ]  initrd.img.old
@   0,0   B [          ]  initrd.img
@   0,0   B [          ]  vmlinuz.old
@   0,0   B [          ]  vmlinuz```


Docker image

```console
docker run -it --rm -p 6080:80 ros-kinetic-linorobot```

In Google chrome 

```console
localhost:6080```





