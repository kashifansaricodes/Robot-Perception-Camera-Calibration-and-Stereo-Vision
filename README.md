# Camera Calibration and Stereo Vision

## Overview
Comprehensive implementation of camera calibration and stereo vision systems. The project consists of two parts:
1. Single Camera Calibration
2. Stereo Vision System
---
   
![Screenshot from 2025-01-12 02-48-38](https://github.com/user-attachments/assets/ac06aab6-d963-4e95-ad0c-26eb05aa1cc8)
---

![Screenshot from 2025-01-12 02-47-53](https://github.com/user-attachments/assets/cd969c2a-2ec4-4b74-ab4a-89361f1f2ecc)

![Screenshot from 2025-01-12 02-47-38](https://github.com/user-attachments/assets/dcebb62a-0cd0-42d6-b5b8-d778e824f972)

## Part 1: Single Camera Calibration

### Objectives
1. Collect calibration images.
2. Implement calibration pipeline.
3. Analyze reprojection error.
4. Visualize calibration results.

### Implementation Pipeline
1. **Image Collection**
   - Use 50 calibration board images.
   - Patterns: Chessboard or circular.

2. **Calibration Process**
   - Detect corners or centroids in calibration images.
   - Optimize camera parameters.
   - Undistort images based on calculated parameters.

3. **Error Analysis**
   - Calculate reprojection error.
   - Visualize and assess accuracy.

## Part 2: Stereo Vision System

### Objectives
Implement a complete stereo vision pipeline using provided datasets.

### Implementation Pipeline
1. **Calibration**
   - Match features between stereo images.
   - Estimate Fundamental and Essential matrices using RANSAC.
   - Extract rotation and translation parameters.

2. **Rectification**
   - Compute and apply homography transformations.
   - Visualize epipolar lines for accuracy.

3. **Depth Computation**
   - Generate disparity maps.
   - Compute depth values.
   - Visualize depth using heatmaps.

### Dataset Parameters
- Camera matrices (cam0, cam1)
- Focal length (f)
- Principal points (cx, cy)
- Baseline information
- Image dimensions
- Disparity bounds

## Usage
1. Run the notebooks in Google Colab.
2. Upload calibration images and stereo datasets.
3. Execute pipeline steps sequentially.
4. Analyze results and visualizations.

## Technical Requirements
- Python 3.x
- OpenCV
- NumPy
- Matplotlib
- Google Colab

## References
D. Scharstein, H. Hirschmüller, et al. High-resolution stereo datasets with subpixel-accurate ground truth.
German Conference on Pattern Recognition (GCPR 2014), Münster, Germany, September 2014.
