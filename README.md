# Depth Estimation on the KITTI Dataset

## Overview
This repository contains a Python notebook that explores two methods of depth estimation: **Monocular** and **Stereo**. Depth estimation is essential for applications like autonomous driving and robotics, as it calculates the distance of objects from a camera. The project utilizes the **KITTI dataset**, which is widely used for autonomous driving research.

## Dataset
The project uses the **KITTI dataset**: [KITTI dataset](https://www.cvlibs.net/datasets/kitti/). This dataset provides high-resolution images from stereo cameras and ground truth depth information from a LiDAR sensor.

## Models
### Monocular Depth Estimation
- Uses a single image to predict depth.
- Simpler setup but often less accurate compared to stereo methods.
- This project uses **Monodepth** to predict depth from single frames.

### Stereo Depth Estimation
- Involves comparing images from two cameras positioned at slightly different angles (similar to human vision).
- More accurate for nearby objects.
- The **Manydepth** model is used, which leverages two frames for improved depth accuracy.

## Key Features
- **Monocular vs Stereo Comparison**: Understand the trade-offs between using fewer inputs (monocular) and achieving higher precision (stereo).
- **LiDAR Integration**: Projects LiDAR data onto camera images to observe disparity and validate depth estimation accuracy.
- **Classical and DL Approaches**: Generates disparity maps using both classical (StereoSGBM) and deep learning methods.

## License
This project is licensed under the MIT License.

