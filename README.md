# Histogram-Equalization
 Custom implementation of histogram equalization in Python for image contrast enhancement
 
This project demonstrates a custom implementation of histogram equalization, a widely used image processing technique that enhances the global contrast of grayscale images. The goal is to redistribute pixel intensity values to better utilize the available range, making details more visible in under- or over-exposed images.

Problem Statement:

Low-contrast images often have a narrow range of intensity values, making important features hard to distinguish. Histogram equalization enhances image contrast by flattening and spreading out the most frequent intensity values, improving the visibility of fine details.

Solution Overview:
-A Python function w
ritten from scratch using NumPy to perform histogram equalization.

-A test image to demonstrate the effects.

-A visual comparison with OpenCV’s built-in cv2.equalizeHist() function to verify correctness.

-An interactive Jupyter notebook to explore the process step-by-step.

Note: This implementation avoids using OpenCV's equalizeHist() function in the custom logic. The OpenCV function is used only for comparison.

Project Structure:

-histogram-equalization/

-custom_equalize.py : Python script with the custom implementation

-HistogramEqualization.ipynb : Notebook version with visualizations and explanations

-example_image.jpg : Sample image used for demonstration

-comparison_result.png : Side-by-side comparison of outputs (optional)

How It Works:
-Compute the histogram of the grayscale image.

-Normalize the histogram to get a probability distribution.

-Calculate the cumulative distribution function (CDF).

-Map original pixel values to new values using the CDF.

-Construct and return the equalized image.

Requirements:
-Python 3.x

-numpy

-opencv-python

-matplotlib
