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

### 1. ardupilot_gz_bringup

Added iris_runway_mapping_launch.py


### 2. ardupilot_gz_gazebo

Added runway mapping world for launch file to work


---

