# imgBlurChecker

This is a simple python program that labels a set of images as "Blurry" or "Not Blurry" using OpenCV. 

Use: *python imgBlurChecker.py --images images* to run if the set of images has been stored in the "images" directory of the cloned repository. Otherwise replace "images" with the path to the directory where the images are stored.    


###a. Methodology:

--> Computation of laplacian of the grayscaled version of the input image usig 3x3 2D convolution kernel.
--> Computation of variance of the laplacian.
--> if (variance < specified Threshold) label: "Blurry"; else label: "Not Blurry". 

###b. References:

--> Rafael C. Gonzalez and Richard E. Woods. *Digital Image Processing (3rd Edition)*.
-->*Analysis of focus measure operators for shape-from-focus* [2013 Pertuz et al].
--> www.pyimagesearch.com 