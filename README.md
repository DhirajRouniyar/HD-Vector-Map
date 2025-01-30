# HD-Vector-Map
# Introduction

This presents a high-definition vector map (HDVM) generation pipeline tailored for autonomous vehicles, particularly in complex urban settings. Conventional HDVM methods often assume a planar surface, leading to inaccuracies in real-world applications. To overcome this, our approach integrates data from multiple sensors, including GNSS (Global Navigation Satellite System), INS (Inertial Navigation System), LiDAR, and cameras.

The pipeline begins by extracting semantic information from raw images using advanced deep learning models like Vision Transformer (ViT) and Swin Transformer. Absolute 3D object data is then obtained from 3D LiDAR depth, while precise pose estimation is derived using GNSS-RTK and an INS-based navigation system. This semantic data is further processed to extract vector elements such as lane markings, forming the HDVM.

A key aspect of this work is ensuring HDVM accuracy. We analyze two major sources of error—segmentation inconsistencies and LiDAR-camera extrinsic calibration deviations. To illustrate their impact on HDVM precision, an error propagation framework is included in the analysis.

![Alt Text](https://github.com/DhirajRouniyar/HD-Vector-Map/blob/main/images/pipeline.png)
