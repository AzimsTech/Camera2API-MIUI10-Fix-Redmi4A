# Fix Camera2API in MIUI10 (Redmi4A/5A)
## MIUI 10 Breaks Camera2 API Support Here's Magisk Module to Fix It

![cover](https://i.imgur.com/Ah7kgM0.png)

Starting with the MIUI 10 update, Xiaomi decided to remove camera2 api files in system. As such, Redmi 4A/5A users which uses MIUI will not able to enable camera 2 API support. MIUI 10 lacks lib file which is require for camera2 api functionality to work.

I just found and picked up the necessary file for Camera2API to work from MIUI10.

    system\lib\hw\camera.msm8937.so
  
This module also adds camera2api support in the build.prop systemlessly, so you don't have to. This is done by editing build.prop to add or enable "persist.camera.HAL3.enabled=1". 

# Trobleshooting
1. Install Camera2 Probe from playstore to check if it working.
![example](https://i.imgur.com/o8IvgzV.png)
2. If your gcam app still doesn't work please use another one from [https://www.celsoazevedo.com/files/android/google-camera/](https://www.celsoazevedo.com/files/android/google-camera/)
