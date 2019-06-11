# Invisibility-Cloak
This is a program to make an invisibility cloak using opencv.
Who doesn't want to get invisbile from this real world? This code turns a red colour cloth into an invisibility cloak.

# Setup/Requirements
    The code is written in Python (Python3) You need the following libraries

        numpy
        OpenCV
        time
# Colour of the Cloak
So what I have done is used a red colour cloth as out invisibility cloak. First determine pixels corresponding to red colour or the region covered by the cloth. To detect red colour we use the HSV colour space.

Conversion of image into HSV colour space using the following line of code.

img_hsv=cv2.cvtColor(img, cv2.COLOR_BGR2HSV)

Using HSV(Hue-Saturation-Value) colour space we can distinguish between different colours much accurately than we can in RGB colour space.

# HSV
The hue range actually from 0-360. But in openCV it is upto 180 only
I have used red which is 0-10.

SAturation is purity of red. since i have used the cloak which is highly concentrated in red colour, i have a value of 120-255

Value is the brightness and is selected 70 -255
