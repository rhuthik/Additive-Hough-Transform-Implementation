# Hough Transform Line Detection

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
