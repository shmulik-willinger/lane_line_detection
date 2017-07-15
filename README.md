# **Finding Lane Lines on the Road**
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

Overview
---

When we drive, we use our eyes to decide where to go.  The lines on the road that show us where the lanes are act as our constant reference for where to steer the vehicle.  Naturally, one of the first things we would like to do in developing a self-driving car is to automatically detect lane lines using an algorithm.

In this project we will detect lane lines in images using Python and OpenCV ("Open-Source Computer Vision"), which is a package that has many useful tools for analyzing images.  

For this project I used Anaconda Python 3 distribution with Jupyter Notebook along with the numpy, matplotlib, and OpenCV libraries. I also used "moviepy" package for video processing.


The Project
---

## In this project, the code will identify lane lines on the road, first in images, and later in a video streams ##

The main pipeline in the LaneLines.ipynb notebook contain a couple of steps using gaussian kernel, canny edge detection and hough transformation in order to detect the lines.

Other helper functions in charge of refining and extrapolating the lines for smoothing the output.

More details can be found in the writeup_report.md file.

The test_images and test_videos folders contain some inputs I used in the projects, the outputs folder contains the images and videos with the lines after the pipeline processing.

## Example Image

Original Image             |  Gray
:-------------------------:|:-------------------------:
![]( https://github.com/shmulik-willinger/lane_line_detection/blob/master/readme_img/original.jpg?raw=true)  |  ![]( https://github.com/shmulik-willinger/lane_line_detection/blob/master/readme_img/gray.jpg?raw=true)

Gaussian Blurred             |  Canny edge detection
:-------------------------:|:-------------------------:
![]( https://github.com/shmulik-willinger/lane_line_detection/blob/master/readme_img/gaussian.jpg?raw=true)  |  ![]( https://github.com/shmulik-willinger/lane_line_detection/blob/master/readme_img/canny.jpg?raw=true)


Hough transformation   (with region mask)           |  Final result
:-------------------------:|:-------------------------:
![]( https://github.com/shmulik-willinger/lane_line_detection/blob/master/readme_img/hough.jpg?raw=true)  |  ![]( https://github.com/shmulik-willinger/lane_line_detection/blob/master/readme_img/final.jpg?raw=true)


Video example

[![video lane_line_detection](https://github.com/shmulik-willinger/lane_line_detection/blob/master/readme_img/lane_line_detection.gif)](http://www.youtube.com/watch?v=u0OumobnHaE)


How to use
---

Jupyter is an Ipython notebook where you can run blocks of code and see results interactively. All the code for this project is contained in a Jupyter notebook.

To start Jupyter in your browser, use terminal to navigate to your project directory and then run the following command at the terminal prompt (be sure you've activated your Python 3 environment)

`> jupyter notebook`

A browser window will appear showing the contents of the current directory.  Click on the file called "LaneLines.ipynb".  Another browser window will appear displaying the notebook.  Follow the instructions in the notebook to run the project.  
