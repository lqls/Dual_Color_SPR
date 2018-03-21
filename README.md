# Dual_Color_SPR
Android app for interfacing with the smartphone-based dual color SPR sensor designed by the Peng group at Dalian University of Technology, China(https://www.dlut.edu.cn). There are 24 bits per pixel in color images, which include three 8-bit integers (0−255) that indicate the intensity of  RGB colors. The R values and G values of all the pixels in the region of interest (ROI) are averaged as the intensity of red channel and green channel. After capturing the required images with 640 × 480 resolution, the average intensities of red and green channels were calculated and displayed on the screen in real time. A rectangular area covering the bright image of optical fiber’s end face was chosen as region of interest (ROI). 
Note: The coordinates of the ROI area are related to the connection between the sensor and the mobile phone. Here, the source code does not specify the specific coordinates, and the intensity of entire image is directly calculated. The time interval is 200 ms, and we can average the 10 values to reduce the noise level.

# Source Code Directories
1. MainActivity.java: Application startup animation.
2. ImageSPR.java： Detection activity.
3. CameraUtil.java: Call the phone camera to calculate the red channel and green channel intensity.
4. ChartUtil.java： Display the results.
5. SaveUtil.java: Save results to SD card.
