This project is highly influenced and inferred by [Toward Characteristic-Preserving Image-based Virtual Try-On Network](https://arxiv.org/abs/1807.07688) and [CP-VTON](https://github.com/sergeywong/cp-vton).


# Dataset
Training/Testing: [VTON](https://github.com/xthan/VITON), [Processed](https://drive.google.com/open?id=1MxCUvKxejnwWnoZ-KoCyMCXo3TLhRuTo)

# Modules
- Garment Detection

- Human Pose Shape Estimation
  * Keypoints: 18 body keypoints from the pretrained [OpenPose](https://github.com/CMU-Perceptual-Computing-Lab/openpose)
  * Body parsing: pretraind on [MHP dataset](https://lv-mhp.github.io/).
  * Video tracking: [OpenCV](https://docs.opencv.org/)
  
- Garment Warping / Geometric Matching Module

- Reconstruction / Try-On Module


# Demo


### Contributor
|Module  | Human Pose Estimation | Garment Segmentation | Garment Warping (GMM) |  Try-On (TOM)|
|:------ | :----- | :------ | :----- | :----|
|Contributor  | Mavis Wang | Xiaocen Xie |  Ililta Gebrihiwet  | CoCo Yu |


### Citation
@inproceedings{wang2018toward,
	title={Toward Characteristic-Preserving Image-based Virtual Try-On Network},
	author={Wang, Bochao and Zheng, Huabin and Liang, Xiaodan and Chen, Yimin and Lin, Liang},
	booktitle={Proceedings of the European Conference on Computer Vision (ECCV)},
	pages={589--604},
	year={2018}
}
