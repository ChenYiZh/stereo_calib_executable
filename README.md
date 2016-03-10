## stereo calibration executable

this is the executable of stereo calibration for VisionerTech VMG-PROV 01. use this to calibrate while seeing mismatching or SLAM SDK not working. source code of this executable could be found here.

## Requirement:

1.  recommended specs: Intel Core i5-4460/8G RAM/GTX 660/at least two USB3.0/
2.  windows x64 version.(tested on win7/win10)

## Installation

1.  install "vcredist_x64.exe".
2.  plugin cameras to USB3.0 port. if it's recognized as a "USB web cam"

    ![alt text](https://github.com/flankechen/stereo_calib_executable/blob/master/readme_image/usbwebcam.png "usbwebcam")

    uninstall the driver

    ![alt text](https://github.com/flankechen/stereo_calib_executable/blob/master/readme_image/usbwebview2.png "usbwebview2")

    rescan for hardware

    ![alt text](https://github.com/flankechen/stereo_calib_executable/blob/master/readme_image/usbwebview3.png "usbwebview3")

    success!

    ![alt text](https://github.com/flankechen/stereo_calib_executable/blob/master/readme_image/usbwebview4.png "usbwebview4")

## How to Run
1.  print out "acircles_pattern.png" and stick it to a rigid surface, make it a "calibration board".
2.  run "stereo_calib.exe"， and you will see the image from left and right camera.
3.  place the "calibration board" in front of the camera, press "c" on the key board to capture an image pair(a blue flash appera with success capture). try to capture around 10 pair of the "calibration board" with different angle orientation and distance, try to cover the whole field of view of the cameras.  you can watch a video sample here. the captured image pairs is list in /save_image/ folder.
![alt text](https://github.com/flankechen/stereo_calib_executable/blob/master/readme_image/calib_snap1.png "snap1")
![alt text](https://github.com/flankechen/stereo_calib_executable/blob/master/readme_image/calib_snap2.png "snap2")
4.  press "Esc" on the keyboard. program finds the pattern, perform stereo calibration and show the result. check the blue parallel lines to see left and right image is rectified.
![alt text](https://github.com/flankechen/stereo_calib_executable/blob/master/readme_image/rectified.png "rectified")
5.  press "Esc" on the keyboard to save the result to /save_param/ folder. copy the whole folder to where it's needed.
![alt text](https://github.com/flankechen/stereo_calib_executable/blob/master/readme_image/saved_files.png "saved_files")
