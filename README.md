# [PointPillars: Fast Encoders for Object Detection from Point Clouds](https://arxiv.org/abs/1812.05784) 

A Simple PointPillars PyTorch Implenmentation for 3D Lidar(KITTI) Detection. [[Zhihu](https://zhuanlan.zhihu.com/p/521277176)]

- It can be run without installing [Spconv](https://github.com/traveller59/spconv), [mmdet](https://github.com/open-mmlab/mmdetection) or [mmdet3d](https://github.com/open-mmlab/mmdetection3d). 
- Only one detection network (PointPillars) was implemented in this repo, so the code may be more easy to read. 
- Sincere thanks for the great open-source architectures [mmcv](https://github.com/open-mmlab/mmcv), [mmdet](https://github.com/open-mmlab/mmdetection) and [mmdet3d](https://github.com/open-mmlab/mmdetection3d), which helps me to learn 3D detetion and implement this repo.

## [Compile] 

```
cd ops
python setup.py develop
```



## [How to run]

```
cd PointPillars/

# 1. infer point cloud detection
python test.py --ckpt pretrained/epoch_160.pth --pc_path your_pc_path

e.g.
python test.py --ckpt pretrained/epoch_160.pth --pc_path 1710371446108926370.pcd 

# 2. infer and visualize point cloud
python test.py --ckpt pretrained/epoch_160.pth --pc_path your_pc_path --v

e.g.
python test.py --ckpt pretrained/epoch_160.pth --pc_path 1710371446108926370.pcd --v

```

## Acknowledements

Thanks for the open source code [mmcv](https://github.com/open-mmlab/mmcv), [mmdet](https://github.com/open-mmlab/mmdetection) and [mmdet3d](https://github.com/open-mmlab/mmdetection3d).
