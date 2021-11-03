# Camera-Calibration-using-Open-CV
Calibrating the values of intrinsic and extrinsic parameters of the camera and hence understanding lens distortion using checkerboard calibration method.

# Abstract 
A camera, when utilized as a visual sensor, is a vital piece for a few areas like robotics, surveillance, space exploration, social media, industrial automation, and even the entertainment industry. It is fundamental for us to know the parameters of a camera to utilize it successfully as a visual sensor. The process of estimating the parameters of a camera is called camera calibration. This means we have all the information (parameters or coefficients) about the camera required to determine an accurate relationship between a 3D point in the real world and its corresponding 2D projection (pixel) in the image captured by that calibrated camera. There are many types of camera calibration techniques . The major techniques are - Calibration pattern ,Geometric clues, Deep Learning based .Chessboard images are used for implementation of this project. Checkerboard method is used in these implementation which falls into the category of  Calibration pattern , this method is better than others  and widely used because of many reasons that we will discuss . For accomplishing this Open CV library in Python and Python Programming Language are used. The camera is calibrated as a result of this implementation . A lot of important parameters of camera are obtained like Intrinsic camera matrix ,Lens distortion coefficients etc. and hence will help us understand lens distortion.

# Introduction
The process of estimating the parameters of a camera is called camera calibration.
 A camera calibration algorithm has the following inputs and outputs

Inputs : A collection of images with points whose 2D image coordinates and 3D world coordinates are known.
Outputs: The 3×3 camera intrinsic matrix, the rotation and translation of each image

# Motivation ( Issue and Challenges)
 It is essential to know the parameters of a camera to use it effectively as a visual sensor.  Distortion effects are introduced by a lens .By the derived distortion coefficients to  we can obtain the un-distorted  image.
 

# Steps of work
1)Define real world coordinates of 3D points using checkerboard pattern of known size. 

2)Capture the images of the checkerboard from different viewpoints. 

3)Use findChessboardCorners method in OpenCV to find the pixel coordinates (u, v) for each 3D point in different images 

4)Find camera parameters using calibrateCamera method in OpenCV, the 3D points, and the pixel coordinates. 


# How our propose system will work?
We are using Calibration pattern . We will perform calibration by capturing several images of an object or pattern of known dimensions from different view points. We are using images of the chessboard for this purpose.

# Literature works 
**Geometric clue**s: In these method other geometric clues are there like straight lines and vanishing points which can be used for calibration.

**Deep Learning based**: In these method we have a single image of the scene, it may still be possible to obtain calibration information of the camera using a Deep Learning based method.


# Future Applications
This model can be applied to any vision sensors.

# References
[1] https://nikatsanka.github.io/camera-calibration-using-opencv-and-python.html

[2] https://learnopencv.com/camera-calibration-using-opencv/

[3] https://learnopencv.com/understanding-lens-distortion/

[4] https://github.com/spmallick/learnopencv/tree/master/UnderstandingLensDistortion
