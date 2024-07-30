
# Motion Estimation in Computer Vision

This Jupyter notebook demonstrates motion estimation techniques in computer vision using Python. The methods implemented include the Lucas-Kanade and Horn-Schunck algorithms for optical flow estimation. The notebook uses OpenCV, NumPy, and other scientific libraries to process and visualize motion between sequential images.

## Table of Contents
1. Introduction
2. Dependencies
3. Read and Show Images
4. Preprocessing
5. Image Derivatives
6. Lucas-Kanade Method
7. Horn-Schunck Method
8. RAFT
9. Results and Visualization

## Introduction
Motion estimation is a critical task in computer vision, used in various applications such as video compression, object tracking, and autonomous navigation. This notebook explores two fundamental methods for motion estimation: Lucas-Kanade and Horn-Schunck.

## Dependencies
The following Python libraries are required to run the notebook:
- OpenCV
- NumPy
- Matplotlib
- Scipy

Install the necessary packages using pip:
```bash
pip install opencv-python numpy matplotlib scipy
```

## Read and Show Images
The notebook begins by loading and displaying two consecutive frames from a sequence of images. These images are converted to grayscale for further processing.

## Preprocessing
Gaussian Blur is applied to the images to reduce noise, which helps in more accurate derivative computation.

## Image Derivatives
Image derivatives are computed using convolution with specific masks. These derivatives are essential for calculating optical flow.

## Lucas-Kanade Method
The Lucas-Kanade method is implemented to estimate optical flow. This method assumes that the flow is essentially constant in a local neighborhood of the pixel under consideration and solves for the flow parameters.

### Steps:
1. Initialize `u` and `v` with zero values.
2. Calculate the image derivatives in x, y, and t directions.
3. Use the derivatives to compute the flow vectors.

## Horn-Schunck Method
The Horn-Schunck method is another approach to estimating optical flow, which introduces a global smoothness constraint.
## RAFT
This is an another method for estimating optical flow, it belongs to deep learning domin

### Steps:
1. Initialize `u` and `v` with zero values.
2. Iteratively update the flow vectors using the Laplacian of the flow field.

## Results and Visualization
The notebook provides visualizations of the flow fields computed by both methods, using quiver plots to illustrate the motion vectors.

### Sample Output
![Lucas-Kanade Result](path/to/lucas_kanade_output.png)
![Horn-Schunck Result](path/to/horn_schunck_output.png)

##
The detailed report have been uploded in the repository please go through it.

---

By following the steps outlined in this notebook, you will gain a deeper understanding of motion estimation techniques in computer vision.
