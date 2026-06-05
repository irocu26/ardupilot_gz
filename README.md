# Usage Guide

## If you have already removed it , and want to pull changes 
```bash
cd ~/ardu_ws/src/ardupilot_gz
git pull origin main
```

## Remove Existing Original Ardupilot Repository

```bash
rm -rf ~/ardu_ws/src/ardupilot_gz/
```

---

## Clone Custom Repository

```bash
cd ~/ardu_ws/src

git clone https://github.com/irocu26/ardupilot_gz.git
```

---

# Notes

After cloning the repository, rebuild the workspace if required:

```bash
cd ~/ardu_ws

colcon build --packages-select ardupilot_gz_application ardupilot_gz_bringup ardupilot_gz_description ardupilot_gz_gazebo
```

---

```bash

source ~/ardu_ws/install/setup.bash
ros2 launch ardupilot_gz_bringup iris_runway_mapping.launch.py
```

# Changelog

## Current Version Updates

### Added GZ_ROS bridge to support rgbd camera image, depth_image , points 

#### You can subscribe to following topics

1. `Stereo Image: "/camera_left/image" , "/camera_right/image" ` 
---

