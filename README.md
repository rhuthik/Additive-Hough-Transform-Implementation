# Additive Hough Transform

## Description

This project implements the Additive Hough Transform algorithm for line detection using Python and compares it with the Normal Hough Transform. The Hough Transform is a popular technique in computer vision and image processing for detecting lines in an image. It works by converting the image space into a parameter space, where lines are represented by curves. By finding the intersections of these curves, we can identify the lines present in the original image.The Additive Hough Transform is an enhanced variation of the classic Hough Transform that improves the accuracy of line detection by considering local origins within the image.

This project provides two variations of the Hough Transform:

1. Normal Hough Transform: This implementation uses the classic Hough Transform algorithm to detect lines. It generates an accumulator matrix to store the voting values and then finds the peaks in the accumulator to determine the lines.

2. Additive Hough Transform: This variation improves upon the Normal Hough Transform by considering local origins within the image. It divides the image into blocks and calculates the rho values of both the local origins and the initial block. By summing these rho values, the Additive Hough Transform enhances the line detection accuracy.

## Installation

To run the code in this project, you need to have the following dependencies installed:

- `matplotlib`
- `numpy`
- `argparse`
- `math`
- `cv2` (OpenCV)

You can install these dependencies using pip:

pip install matplotlib numpy opencv-python

## Usage

To use the Hough Transform line detection, follow these steps:

1. Clone the repository or download the code files.
2. Make sure you have the required dependencies installed.
3. Provide the path to your input image in the `path` variable in the code.
4. Run the Python script.

The code will perform line detection using both the Normal Hough Transform and the Additive Hough Transform. It will display the results, showing the detected lines overlaid on the original image, as well as the accumulator matrix.

## Code Structure

The code is organized as follows:

- Importing the necessary libraries and modules.
- Definition of helper functions.
- Normal Hough Transform implementation.
- Simple padding function to make the image square.
- Preprocessing the image and finding edges using Canny Edge Detection.
- Performing the Normal Hough Transform and drawing the detected lines.
- Additive Hough Transform implementation.
- Finding the rho values of the local origins and the first block.
- Performing the Additive Hough Transform and drawing the detected lines.
- Displaying the results using Matplotlib.

## Examples

The code provided includes an example that reads an image file and performs line detection using both the Normal Hough Transform and the Additive Hough Transform. The results are displayed using Matplotlib, showing the detected lines overlaid on the original image and the accumulator matrices.

Please note that you need to adjust the `path` variable in the code to point to a valid image file on your system.


## License

This project is licensed under the [MIT License](LICENSE). You are free to modify, distribute, and use the code in any way you find appropriate.
