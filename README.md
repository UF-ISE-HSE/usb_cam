# usb_cam
This repository is the drive for using usb camera in ros.

## 1. Prerequisites
### 1.1 **Ubuntu** and **ROS**
Ubuntu 64-bot 16.04 or 18.04 or 20.04.
ROS Kinetic or Melodic or Noetic

## 2. Build
Clone the repository and catkin_make:

```
cd ~/catkin_ws/src
git clone https://github.com/UF-ISE-HSE/usb_cam.git
cd ../
catkin_make
source ~/catkin_ws/devel/setup.bash
```

## 3. Parameters
Update the information in launch/usb_cam-test.launch

This descriptions of parameters can be found in this link [usb_cam](http://wiki.ros.org/usb_cam). 
**Note**: video_device should be same as the usb port in the computer, the default of the usb port is "/dev/video0".
If the port is not the default, run
```
cd /dev
```
see which video is available.

## 4. Run

```
roslaunch usb_cam usb_cam-test.launch
```
The output topic name of the image information is "/usb_cam/image_raw". 
