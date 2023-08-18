# PointNet-for-Point-Cloud-Classification

![PointNet](https://stanford.edu/~rqi/pointnet2/images/pnpp.jpg)

<!-- <a href = "https://stanford.edu/~rqi/pointnet2/images/pnpp.jpg">  -->

## Introduction

This repository implements the PointNet architecture for the classification, detection, and segmentation of unordered 3D point sets, commonly referred to as point clouds. Point clouds are widely used in computer vision applications and are typically captured by lidar or radar sensors. PointNet2 (Qi et al., 2017) is a seminal deep learning paper that directly operates on raw point cloud data without the need for discretization or projection.

The primary focus of this project is to demonstrate how to:

- Load datasets containing point clouds of various objects.
- Implement the PointNet architecture from scratch.
- Train the PointNet model on a dataset of labeled point clouds.
- Evaluate the model's performance on new, unseen point clouds.

## About PointNet

PointNet tackles the challenge of working with unstructured point cloud data directly, allowing for the processing of 3D data without the need for transforming it into 2D or 3D voxel representations. This approach preserves the inherent structure of point clouds and has shown promising results in various 3D vision tasks.
If you want to know more about this topic do refer this [Article on Medium](https://medium.com/@luis_gonzales/an-in-depth-look-at-pointnet-111d7efdaa1a)

PointNet (the v1 model) either transforms features of individual points independently or process global features of the entire point set. However, in many cases there are well defined distance metrics such as Euclidean distance for 3D point clouds collected by 3D sensors or geodesic distance for manifolds like isometric shape surfaces. In PointNet++ we want to respect spatial localities of those point sets. PointNet++ learns hierarchical features with increasing scales of contexts, just like that in convolutional neural networks. Besides, we also observe one challenge that is not present in convnets (with images) -- non-uniform densities in natural point clouds. To deal with those non-uniform densities, we further propose special layers that are able to intelligently aggregate information from different scales.


## Getting Started
You can work on custom dataset by refering to  this 
[GitHub Repo](https://github.com/charlesq34/pointnet2). This repo is the original Repo for PointNet++. 

The dataset link in that repo does not work (<i>probably</i>). 
So I have provided a zip file which you can find it 
[here](https://www.kaggle.com/datasets/balraj98/modelnet10-princeton-3d-object-dataset).


### Dataset

1. Prepare your dataset of labeled point clouds.
2. Organize your dataset folders and annotations.

## Acknowledgments

This project is inspired by the groundbreaking work on PointNet by Qi et al. (2017). For more information, refer to the original [PointNet2 paper](https://stanford.edu/~rqi/pointnet2/).





## Contact

For questions or feedback, please feel free to reach out:

- Author: Kunal Tilaganji 

Project Link: [Link](https://github.com/kunaltilaganji/PointNet-for-Point-Cloud-Classification)
