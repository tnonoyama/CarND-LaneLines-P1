# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then binarized it, masked its region, drawed lines, and finally combined the original image and the lines.

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by designing the threshold value as 50, the minLineLengh value as 100, and maxLineGap as 160.


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when the edge of the dashed line desappears from the bottom of the image.
In this case, the line would get short bacause the function couldn't detect any line edge.


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to stretch the line edge.
But i don't know how I should do it.
