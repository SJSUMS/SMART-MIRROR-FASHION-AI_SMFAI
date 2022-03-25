This project is highly influenced by [Toward Characteristic-Preserving Image-based Virtual Try-On Network](https://arxiv.org/abs/1807.07688) 
and reproduced based on the repo [CP-VTON-Plus](https://github.com/minar09/cp-vton-plus) Network.


# Dataset
- Train/Eval 
	* [VTON](https://github.com/xthan/VITON)
	* [Processed](https://drive.google.com/open?id=1MxCUvKxejnwWnoZ-KoCyMCXo3TLhRuTo)
- Test
	* Reference Person: [LIP (Look Into People)](https://github.com/hyk1996/Single-Human-Parsing-LIP)
	* Target Cloth: [FPI (Fashion Product Image)](https://www.kaggle.com/paramaggarwal/fashion-product-images-dataset)
	* Video: Superdry Inc.

- Inputs (image/video/webcam): 
	1. Reference person (image)
	2. Human keypoints (pose-json)
	3. Human parsing segments (image-parse)
	4. Target cloth (cloth)
	5. Cloth segmentation (cloth-mask)

- Output (image/video):
	1. warped garment images
	2. real-time try-on images


# Modules
1. Garment Detection
  	* Clothing item masks

2. Human Pose Shape Estimation
  	* Keypoints: 18 body keypoints from Cafe [OpenPose](https://github.com/CMU-Perceptual-Computing-Lab/openpose)
  	* Body parsing: fine-grained body segmentation, pretraind on [MHP dataset](https://lv-mhp.github.io/).
  	* Video tracking: [OpenCV](https://docs.opencv.org/)
  
3. Garment Warping
	* CP-VTON Geometric Matching Module

4. Reconstruction
	* CP-VTON Try-On Module


# Demo


### Contributor
|SMFAI Modules  | Human Pose Estimation | Garment Mask | CP-VTON GMM |  CP-VTON TOM |
|:------ | :----- | :------ | :----- | :----|
|Contributor  | [Mavis Wang](https://github.com/mavisw) | [Xiaocen Xie](https://github.com/tiffanyxxc) |  [Ililta Gebrihiwet](https://github.com/ililtaG)  | [Ting-wei (CoCo) Yu](https://github.com/cocosjsu) |


### Citation
@InProceedings{Minar_CPP_2020_CVPR_Workshops,
	title={CP-VTON+: Clothing Shape and Texture Preserving Image-Based Virtual Try-On},
	author={Minar, Matiur Rahman and Thai Thanh Tuan and Ahn, Heejune and Rosin, Paul and Lai, Yu-Kun},
	booktitle = {The IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
	month = {June},
	year = {2020}
}
