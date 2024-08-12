# Edge Detection Techniques

## Overview

This project demonstrates various edge detection techniques using Python and OpenCV. The techniques include Sobel Edge Detection, Laplacian of Gaussian (LoG) Edge Detection, and Canny Edge Detection. The code processes images to highlight edges and provides visual comparisons of the results from different edge detection methods.

## Project Structure

- `edge_detection.py`: Contains the code to apply Sobel, LoG, and Canny edge detection methods to images.
- `original_image1.jpg`, `original_image2.jpg`, `original_image3.jpg`: Sample images for testing (uploaded by the user).

## Requirements

- Python 3.x
- OpenCV (`cv2`)
- NumPy
- Matplotlib

You can install the required packages using pip:

```bash
pip install opencv-python-headless numpy matplotlib
```

## Usage

**File:** `edge_detection.py`

**How to Run:**

1. Ensure you have Python installed along with the required packages.
2. Run the script using Python:

    ```bash
    python edge_detection.py
    ```

3. **Upload Images:** The script will prompt you to upload images. You can upload up to three images for processing.

**What the Code Does:**

- **Sobel Edge Detection:** Computes gradients along x and y directions and calculates the magnitude of the gradient to detect edges.
- **Laplacian of Gaussian (LoG) Edge Detection:** Applies Gaussian blur to the image and then computes the Laplacian to detect edges.
- **Canny Edge Detection:** Uses the Canny algorithm to detect edges by identifying areas of rapid intensity change.
- **Display Results:** Shows the original image and the results of the three edge detection methods side by side for comparison.

## Code Details

### `sobel_edge_detection(image)`

- **Converts** the image to grayscale.
- **Computes** gradients along the x and y directions.
- **Calculates** the gradient magnitude and applies a threshold to detect edges.

### `log_edge_detection(image)`

- **Converts** the image to grayscale.
- **Applies** Gaussian blur to reduce noise.
- **Computes** the Laplacian of the blurred image and applies a threshold to detect edges.

### `canny_edge_detection(image)`

- **Converts** the image to grayscale.
- **Applies** the Canny edge detector to identify edges.

### Image Processing and Display

- **Uploads** up to three images and processes them using the defined edge detection methods.
- **Displays** the original image and the results of the edge detection methods in a grid layout.
