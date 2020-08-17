# stereo-reconstruction

An implementation of stereo reconstruction from two given rgb images.
### Steps:
1. SIFT matching with ratio test.
2. Compute fundamental matrix with RANSAC and visualize epipolar line.
3. Compute four sets of possible camera poses from fundamental matrix and camera intrinsic matrix.
4. Triangulation
5. Disambiguate camera poses with Cheirality test.
6. Stereo rectification.
7. Disparity map estimation.


<p align="center">
  <img src="/result/epipolar.png" height="200">
  <br>Epipolar line visualization<br>
  <br><br>
  <img src="/result/camera_pose.png" height="400">
  <br>Camera pose estimation from rgb images<br>
  <br><br>
  <img src="/result/triangulation.png" height="400">
  <br>Triangulation<br>
  <br><br>
  <img src="/result/stereo_rectification.png" height="200">
  <br>Stereo rectification<br>
  <br><br>
  <img src="/result/disparity.png" height="200">
  <br>Disparity map estimation<br>
</p>

## Dependencies
* Numpy
* matplotlib
* scipy 1.2.1
* OpenCV 3.4.2
* scikit-learn 0.22.1

## Acknowledgment
Visualization code and data are from UMN Fall 2019 CSCI 5561 course material.
