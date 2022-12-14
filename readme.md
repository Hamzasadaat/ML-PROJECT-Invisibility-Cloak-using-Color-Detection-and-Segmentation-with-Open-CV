# Invisibility Cloak using Color Detection and Segmentation with Open CV

Hamza Sadaat
# Abstract:
Have you ever thought of making visible things invisible, just like the Harry Potter? The cloak was magical and invisible in Harry Potter, the movie. As we know there is no magic and no invisible cloak which exists in the world. It’s all about the graphics tricks.
The concept of an invisibility cloak is a mixture of science, fantasy, and the collective imagination. This paper helps to create one’s own ‘Invisibility Cloak’. It will make use of Python and OpenCV module specifically targeting Image Processing and Image Segmentation to create a false sense of invisibility in the frame. It will explore how an object of a specific color or texture can be manipulated using the OpenCV library of python.
# I. INTRODUCTION:
Computer vision came into the picture in late 1960s. Its whole purpose was to increase the intellect of the artificial mechanism available by installing the cameras into them and describe whatever they saw just like humans’ visual system. Thus, Computer vision should be able to detect actual daily-life 3D objects through 2D pictures. OpenCV is Open Computer Vision Library of python. With more updates, it has been modified since then to aim for the real-time computer vision. It can be easily run on operating systems Windows and Linux. This library can be easily interfaced with programing languages like Python, MATLAB, Ruby and others as well. Along with Numpy and Python image processing (shape & color detection) can be performed at ease.
# II. METHODOLOGY:
The working is opposite to the concept of green screening. As in the case of green screening background is removed but in this application we remove the foreground. Red colored cloth is used as a cloak for this application. We can use any color with a little bit of changes in the code.

This chart shows the steps to be followed in order generate the
augmented output.

![image](https://user-images.githubusercontent.com/76808385/191723725-c4808a2e-53a4-444c-be2e-38b6039f48b9.png)


1. Capture and store the background frame.
2. Identify the red colored cloth (cloak) by using the color
detection & segmentation algorithm.

![image](https://user-images.githubusercontent.com/76808385/191723753-fda7b346-98fe-41a0-a712-ad6999e005c6.png)

3. Segmenting out the red colored fabric by generating a mask.
4. Generate the final augmented(magical) output to create
Invisibility cloak.

![image](https://user-images.githubusercontent.com/76808385/191723777-ffbcd7bb-6e4a-40cf-ae64-3863fefbb96d.png)


# III. LIMITATIONS:
1. We use the range 0 to 100 & 170 to 180 to avoid the detection of skin as
red. This is because generally in winters, the skin gets red. The large
range of 120 to 255 for saturation is used because ‘our cloth should be of
a highly saturated Red-color’.
2. We require to use the lower-range value as 70 so that ‘we could detect
red color in the creases of the cloth as well.
3. Despite of the cloak’s color being red there might be some areas where,
due-to shadow, the red channel values of the corresponding-pixels are a
bit low.

# RESULT:
Our main task is to substitute the current frame pixels corresponding to
the fabric with the backdrop pixels to create the effect of an invisibilitycloak
to achieve this, we require to save a frame of the backdrop. Since
we’re using a red color fabric to transform it into an invisibility-cloak we
would focus on the discovery of red color in the frame. Firstly, we would
capture a live frame, change the picture from R.G.B to H.S.V color
space & then specify an appropriate range of ‘H.S.V’ values in order
recognize the red color.
# V. CONCLUSION:
Computer vision can be used to solve the most problems with less
sophistication. All the basics regarding the color detection technique
along with different ways to achieve it have been profoundly discussed
in the paper. During the course of programming, we can use both Python
and MATLAB for Computer Vision, but we prefer Python because it
takes less simulation time than MATLAB. Someone having prior coding
experience finds it easy to implement.
