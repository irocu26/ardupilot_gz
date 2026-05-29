# Usage Guide

## Remove Existing Repository

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


# Changelog

## Current Version Updates

### Added GZ_ROS bridge to support rgbd camera image, depth_image , points 

#### You can subscribe to following topics

1. `Raw RGBD Image: "/rgbd_camera/image" ` 
2. `Depth RGBD Image: "/rgbd_camera/depth_image" ` 
3. `Point CLoud of RGBD Image : "rgbd_camera/points" `

---

