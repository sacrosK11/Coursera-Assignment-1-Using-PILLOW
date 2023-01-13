# Coursera-Assignment-1-Using-PILLOW

#Assignment-1-Using-PILLOW -- UMichigan Coursera

Python 3 Programming - UMichigan --> Assignment 1: Building a Better Contact Sheet with PILLOW

Here I share my way how to solve the Assignmet 1 from Week 1 of the Coursera University of Michigan - Course 5 Python Project: pillow, tesseract, and opencv

For the solution, check file 'Assigment1_solution.py'

Assignment 1: Building a Better Contact Sheet

In the lectures for this week you were shown how to make a contact sheet for digital photographers, and how you can take one image and create nine different variants based on the brightness of that image. In this assignment you are going to change the colors of the image, creating variations based on a single photo. There are many complex ways to change a photograph using variations, such as changing a black and white image to either "cool" variants, which have light purple and blues in them, or "warm" variants, which have touches of yellow and may look sepia toned. In this assignment, you'll be just changing the image one color channel at a time

Your assignment is to learn how to take the stub code provided in the lecture (cleaned up below), and generate the following output image:

![assignment1_Instructions_pic](https://user-images.githubusercontent.com/119893079/212377161-3c7c04e7-d24f-4180-abf6-390650803007.png)

From the image you can see there are two parameters which are being varied for each sub-image. First, the rows are changed by color channel, where the top is the red channel, the middle is the green channel, and the bottom is the blue channel. Wait, why don't the colors look more red, green, and blue, in that order? Because the change you to be making is the ratio, or intensity, or that channel, in relationship to the other channels. We're going to use three different intensities, 0.1 (reduce the channel a lot), 0.5 (reduce the channel in half), and 0.9 (reduce the channel only a little bit).

For instance, a pixel represented as (200, 100, 50) is a sort of burnt orange color. So the top row of changes would create three alternative pixels, varying the first channel (red). one at (20, 100, 50), one at (100, 100, 50), and one at (180, 100, 50). The next row would vary the second channel (blue), and would create pixels of color values (200, 10, 50), (200, 50, 50) and (200, 90, 50).

Note: A font is included for your usage if you would like! It's located in the file readonly/fanwood-webfont.ttf

Need some hints? Use them sparingly, see how much you can get done on your own first! The sample code given in the class has been cleaned up below, you might want to start from that.
HINTs

    Check out the PIL.ImageDraw module for helpful functions

    Did you find the text() function of PIL.ImageDraw?

    Have you seen the PIL.ImageFont module? Try loading the font with a size of 75 or so.

    These hints aren't really enough, we should probably generate some more.
