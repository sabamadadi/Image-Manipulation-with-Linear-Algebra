# Image Manipulation with Linear Algebra

This project demonstrates fundamental image processing techniques implemented from scratch using **Python**, **NumPy**, and **OpenCV**. The operations leverage linear algebra concepts to manipulate image data at the pixel level.

## Features

### 1. Image Reading & Display
- Load images using OpenCV.
- Display images in RGB using Matplotlib.

### 2. Geometric Transformations
- **Resize**: Scale images up or down with pixel mapping.
- **Rotate**: Rotate images by any angle using rotation matrices.

### 3. Filtering & Enhancement
- **Blur**: Apply averaging filters to smooth images.
- **Sharpen**: Enhance edges using convolution kernels.
- **Edge Detection**: Detect edges using the Sobel operator.

### 4. Color Manipulations
- **Grayscale Conversion**: Transform RGB images to grayscale using luminance weights.
- **Inversion**: Create a negative of the image.
- **Color Balance**: Adjust RGB channels independently.

## Implementation Highlights
- Pixel-wise operations with **NumPy** for custom image transformations.
- Manual convolution implementation for blurring, sharpening, and edge detection.
- Flexible, reusable `Image` class for easy experimentation with multiple images.

## Demo
The project supports a wide variety of transformations with simple function calls, such as:

```python
img = Image('photo.jpg')
img.show(img.grayscale_conv(img.get_image()))
img.show(img.rotation(45, img.get_image()))
img.show(img.color_balance(img.get_image(), 0.5, 1.2, 0.8))
