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

**Note**: video_device should be same as the usb port in the computer.

## 4. Run

```
roslaunch usb_cam usb_cam-test.launch
```

