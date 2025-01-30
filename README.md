# HD-Vector-Map
# Introduction

This contains a HDVM (high-definition vector map) generation pipeline designed for autonomous vehicles, especially in intricate urban environments. Traditional HDVM creation methods often operate on a planar assumption, causing inaccuracies in real-world scenarios. Our solution, however, integrates data from GNSS (global navigation satellite system), INS (inertial navigation system), LiDAR, and cameras.

The process starts with the extraction of semantic data from raw images using advanced architectures like Vision Transformer (ViT) and Swin Transformer. We then acquire the absolute 3D data of these semantic objects from 3D LiDAR depth and derive high-precision pose estimates from GNSS real-time kinematic (GNSS-RTK) and an INS navigation system. This semantic data aids in the extraction of vector information, such as lane markings, which forms the HDVM.

A significant feature of this repo is its focus on HDVM accuracy. We've examined the impact of two primary error sources: segmentation discrepancies and LiDAR-camera extrinsic parameter deviations. An error propagation scheme is provided to showcase how these sources can affect the HDVM's precision.

![Alt Text](https://your-image-url.com/image.png](https://github.com/DhirajRouniyar/HD-Vector-Map/blob/main/images/pipeline.png)
