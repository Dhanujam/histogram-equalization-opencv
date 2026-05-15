# histogram-equalization-opencv


### Name
DHANUJA M

### Reg. No
212224230057

# Overview

This project demonstrates Histogram Equalization using OpenCV for both grayscale and color images. Histogram Equalization is used to improve image contrast and brightness by redistributing pixel intensity values.

The experiment is performed on the image `parrot.jpg` using Python, OpenCV, NumPy, and Matplotlib.

---

# Objectives

- Read and process grayscale and color images using OpenCV
- Plot image histograms using Matplotlib
- Perform histogram equalization on grayscale images
- Enhance color images using HSV color space
- Compare original and enhanced images visually

---

# Technologies Used

- Python
- OpenCV
- NumPy
- Matplotlib

---

# Files Used

- `parrot.jpg` → Input image
- `grayscale_histogram_equalization.py`
- `color_histogram_equalization.py`

---

# Theory

## What is Histogram Equalization?

Histogram Equalization is an image processing technique used to improve the contrast of an image. It spreads pixel intensity values over a wider range, making hidden details more visible.

---

## Grayscale Histogram Equalization

For grayscale images, histogram equalization is directly applied using:

```python
cv2.equalizeHist()
```

This increases the contrast of the image and improves visibility.

---

## Color Histogram Equalization

Applying histogram equalization directly on RGB channels may distort colors. Therefore, the image is converted into HSV color space.

### HSV Components
- H → Hue
- S → Saturation
- V → Value/Brightness

Histogram equalization is applied only to the V channel to improve brightness while preserving natural colors.

---

# Algorithm

## Part A – Grayscale Histogram Equalization

1. Import required libraries
2. Read image in grayscale mode
3. Display grayscale image
4. Plot histogram of original image
5. Apply histogram equalization using `cv2.equalizeHist()`
6. Display:
   - Original image
   - Histogram of original image
   - Enhanced image
   - Histogram of enhanced image

---

## Part B – Color Histogram Equalization

1. Import required libraries
2. Read color image
3. Plot histograms for B, G, and R channels
4. Convert image from BGR to HSV
5. Apply histogram equalization on V channel
6. Convert enhanced HSV image back to BGR
7. Display:
   - Original color image
   - Histogram of original image
   - Enhanced color image
   - Histogram of enhanced image

---


# Output

## Grayscale Histogram Equalization
- Original grayscale image
- Histogram of original grayscale image
- Enhanced grayscale image
- Histogram of enhanced grayscale image

## Color Histogram Equalization
- Original color image
- Histogram of original color image
- Enhanced color image
- Histogram of enhanced color image

---

# Result

Thus, histogram equalization was successfully performed on both grayscale and color images using OpenCV. The contrast and brightness of the images were improved effectively.

---
