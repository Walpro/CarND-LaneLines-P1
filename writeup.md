
**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)


[image1]: ./lanes_solidWhiteRight.jpg
[image2]: ./lanes_solidYellowCurve.jpg 

---

### Reflection

###1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I applied Gaussian smoothing 
to delete the noise in the image after that I used canny function to detect the edges in the image.
to limit the view into the edges in the road lanes I used a four sided polygon mask.
the next step is to detect the lines in the image which is done by computing the hough transform.
At this point many lines are detected in the edges of  the lanes like illustrated iin the images below. 

![alt white lane detect][image1]

![alt yellow lane detect][image2]


In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...



###2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


###3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
