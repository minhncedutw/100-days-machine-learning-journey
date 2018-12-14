# 100-days-machine-learning-journey
Each day i study a little about machine-learning/deep-learning and share what i learnt

# Journey Plan:
1. CNN
    - Classification: 2D, 3D
    - Regression
    - Differentiation
    - Graph CNN
1. RNN
1. Reinforcement Learning
1. Meta Learning
1. Semi Supervised Learning
1. Active Learning
1. Quantum Machine Learning
1. NeuroEvolution
1. Decentralize Data
1. Others
    Clustering

# Journey tracking

## Day 1 - 2018/12/11: Point Cloud Classification-Segmentation algorithms

> A point cloud is a set of data points in space. 
Point clouds are generally produced by 3D scanners: LIDAR, Kinect, ...

**Approach Classification**
1. Pixel-based: Multi-view CNN(MVCNN)
2. Voxel-based: VoxNet, VRN Ensemble, ...
3. 3D point-based: PointNet

**Great article**

[3D POINT CLOUD CLASSIFICATION USING DEEP LEARNING – RECENT WORKS - 20Sep2017](http://www.itzikbs.com/3d-point-cloud-classification-using-deep-learning)

*Benchmark table of Point Cloud Classification*
![](./figures/1_algorithm-benchmarks.PNG)
[image source](http://blog.ruofeidu.com/summary-pointnet-pointnet-and-pu-net/)

## Day 2 - 2018/12/12: Train Network with Noise to Reduce Overfitting

**Learning Stories** [Train Neural Network với Nhiễu để giảm Overfitting](https://medium.com/@minhnc.edu.tw/train-neural-network-v%E1%BB%9Bi-nhi%E1%BB%85u-%C4%91%E1%BB%83-gi%E1%BA%A3m-overfitting-dfb8984e9eeb)

## Day 3 - 2018/12/13: Active Learning

> Active Learning is not a kind of Deep Learning or Reinforcement Learning. It is a process by which train model on the data it will learn the most from.

> It seems like inherit from the idea of Semi Supervised Learning

**Learning Stories** [Học có chọn lọc(Active Learning)](https://medium.com/@minhnc.edu.tw/active-learning-89af14245083)

## Day 4 - 2018/12/14: Pseudo-labelling: a Semi-Supervised Learning Technique

**What is Semi-Supervised Learning?**

It is to use both labeled data and unlabeled data to train a classifier.
![](https://s3-ap-south-1.amazonaws.com/av-blog-media/wp-content/uploads/2017/09/20182516/dataiku-hadoop-summit-semisupervised-learning-with-hadoop-for-understanding-user-web-behaviours-12-638.jpg)

**How to do it?**

![](https://s3-ap-south-1.amazonaws.com/av-blog-media/wp-content/uploads/2017/09/20185606/pseudo-labeling.png)

**Learning Stories** [Pseudo-labelling: Một phương pháp học bán giám sát](https://medium.com/@minhnc.edu.tw/pseudo-labelling-m%E1%BB%99t-ph%C6%B0%C6%A1ng-ph%C3%A1p-h%E1%BB%8Dc-b%C3%A1n-gi%C3%A1m-s%C3%A1t-ac6f08b9e6d1)

## Day 5 - 2018/12/15: Scalable Agent Alignment via Reward Modeling

**Learning Stories** [Định hướng trợ thông qua mô hình hóa phần thưởng cho tương tác người-máy](https://medium.com/@minhnc.edu.tw/%C4%91%E1%BB%8Bnh-h%C6%B0%E1%BB%9Bng-tr%E1%BB%A3-th%C3%B4ng-qua-m%C3%B4-h%C3%ACnh-h%C3%B3a-ph%E1%BA%A7n-th%C6%B0%E1%BB%9Fng-cho-t%C6%B0%C6%A1ng-t%C3%A1c-ng%C6%B0%E1%BB%9Di-m%C3%A1y-25d4f139c3a0)