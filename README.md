# Computer Vision Assignments Solved Using Python + OpenCV
#### Contains laboratory assignment solutions using Python3 and cv2.
#### Each assignment is solved using inbuilt cv2 operations and user-defined functions.

### Computer Vision Lab 2
*	Image addition
*	Image Subtraction
*	Image Enhancement is performed using the following three methods:
 *	GrayScale Histogram Equalization: We find out the histograms of the grayscale image and look for the distribution of intensities. We will use cv2.equalizeHist() function with the purpose of equalizing the contrast of a given grayscale image. cv2.equalizeHist() function normalises the brightness and also increases the contrast.
 *	Intensity Slicing: It highlights a specific range of grey levels in an image. 1st transformation brightens the desired range of grey levels but preserves grey levels unchanged. 2nd transformation displays a high value of all grey levels in the range of interest and a low value for all other grey levels.
 *	Sharpen: The process of blurring, sharpening, embossing, edge detection, and others, require that a kernel be applied to the image pixels, which is also why this process is also referred to as Convolution- i.e, the process during which the kernel is applied to the image. Commonly used sharpening kernel is: https://en.wikipedia.org/wiki/Kernel_(image_processing)

### Computer Vision Lab 3
* Image Enhancement by adding a constant value ‘90’ to first half of the image
* Image Enhancement by adding a constant value ‘90’ to second half of the image
* Image Enhancement like gamma transformation on the entire image
* Image Enhancement – dynamic range of the image to be improved

### Computer Vision Lab 4
* Find the mean of the grayscale image   
* Apply zero padding, find the mean of the resultant image
* Apply high padding, find the mean of the resultant image
* Apply mid padding, find the mean of the resultant image
* Write the inference obtained from 1,2,3,4
* Apply image smoothening (say, median filter, max filter, min filter, average filter) to any of 3x3 region of interest in the grayscale image
* Apply image smoothening (say, median filter, max filter, min filter, average filter) to any of 5x5 region of interest in the grayscale image
* Write the inference obtained from 6,7

### Computer Vision Lab 5
* Read any coloured image A, Lh, Lv,Ldp, Ldn
  * Let A be an image that consists of black dots on a plain white background
  * Let Lh be an image that consists of 1 black lines in the horizontal direction against white background
  * Let Lv be an image that consists of 1 black lines in the vertical direction against white background
  * Let Ldp be an image that consists of 1 black lines in the diagonal direction (45degrees) against white background
  * Let Ldn be an image that consists of 1 black lines in the diagonal direction (-45degrees) against white background
*  Convert A, Lh, Lv,Ldp, Ldn into grayscale image Ag, Lhg, Lvg,Ldpg, Ldng and Perform -
  *  Detect the presence of a point in an image Ag
  *  Store the spatial location of the point in that image
  *  Detect the presence of line in the image Lhg
  *  Store the spatial location of the line points and its orientation
  *  Detect the presence of line in the image Lvg
  *  Store the spatial location of the line points and its orientation 
  *  Detect the presence of line in the image Ldpg
  *  Store the spatial location of the line points and its orientation
  *  Detect the presence of line in the image Ldng
  *  Store the spatial location of the line points and its orientation
  *  Write the inference obtained from 3.3.2, 3.3.4, 3.3.6,3.3.8.3.3.10

### Computer Vision Lab 6
* Binarize Image
* Use thresholding approach to segment the image into 2,3,4,5…n clusters.

### Computer Vision Lab 7
* Convert the grayscale image into rgb, cmyk
* Convert the color image into grayscale
* Consider an image with extensions such as .jpeg, png, tiff, etc
* Use block based segmentation on grayscale image to identify the homogenous regions for the images obtained from a – c. Save the output image
* Record the inferences
* Use block based segmentation on color image to identify the homogenous regions. Save the output image (You can use range values of the image intensities of a shade)

### Computer Vision Lab 8
* Apply the following on the grayscale image
  * Detect edges using Roberts, Prewitts and Sobel
  * Subtract the edges from each of the methods from the input grayscale 
  * Record the inference as which from step 3.1.b yields good quality image
 
### Computer Vision Lab 9
* Transform the image in the following ways:
  * Translation - f (x, y) → f (x′, y′) where x′ = x + ∆x and y′ = y + ∆y. Note that ∆x and ∆y are the translation in x and y, respectively.
  * Scaling - f (x, y) → f (x′, y′) where x′ = Ax · x and y′ = Ay · y. Note that Ax and Ay are the scaling factor in x and y, respectively.
  * Zooming - using pixel replication

### Computer Vision Lab 10
* Add some noise to the image and save it as second image - Adding salt and pepper noise to first quadrant of the image
* Apply image fusion on the input image and noisy image
  * Pixel by pixel approach: F(i,j) = max(A(i,j),B(i,j))
  * The pepper noise, i.e., the black spots have been eliminated but the salt noise, i.e., the white spots still remain. This is intuitive as image fusion always selects the max pixel value.
* Save the output as O1
* Apply image addition on the input image and noisy image
* Save the output as O2
* Compare the percentage of similarity between O1,O2 using any metric

### Computer Vision Lab 11
* Add some noise to the image and save it as second image - Added salt and pepper noise to first quadrant of the image
* Apply Wavelet Decomposition on the input image
* Save the output as O1
* Apply Wavelet Decomposition on img2
* Save the output as O2
* Compare the image quality of img2 and O2 using metrics
* Apply 2nd , 3rd, ….n levels of decomposition on O1 and save the outputs - To get these, we will apply wavelet transform to the images repeatedly.
* Compare the image quality of the image obtained from decomposition at various levels - The image quality slowly deprecates as the size of the image keeps reducing

### Computer Vision Lab 12
* Convert to Binary Image
  * Dilation on binary image
  * Erosion on binary image
  * Consider another image with two object bridged by thin line, Convert into binary image, Save the output as O3.
  * To the O3, apply opening, Save the output as O4.
  * To the O3, apply closing, Save the output as O5

### Computer Vision Lab 13
* Extract any related 5 blob features.
  * Detecting only circluar blobs.
  * Detecting only convex blobs.
  * Detecting blobs with min inertia 0.7.
  * Detecting blobs with min area 400.
  * Detect blobs by color (here all blobs are of same color).
