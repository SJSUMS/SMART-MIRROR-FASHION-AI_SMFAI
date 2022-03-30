# Smart Mirror Fashion AI - video-based virtual tryon

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

# SMFAI Network 
- Input
	* Reference Person (Video)
	* Target Cloth Item (Image)
- Output
	* video body keypoints tracking
	* cloth transferring try-on video

# Modules
1. Garment Mask
- Input: LIP cloth image
- Output: cloth binary mask

2. Human Pose Shape Estimation and Tracking
- Input: Reference Person Video
- Output:
	* Extracted Video frames
  	* 18 json keypoints in [OpenPose annotations](https://github.com/CMU-Perceptual-Computing-Lab/openpose) annotation.
  	* Body parsing pretained on LIP 20.
	* Improved 7 fine-grained body segmentation.
  	* Improved body binary mask.
	* Temperal and spatial object tracking: [OpenCV](https://docs.opencv.org/)
	* Pose tracking video

3. Try-on
- Input: outputs from #1 and #2
- Output: try-on video

# Tasks
* Final test video
* Final cloth images
* Module development and testing
* Object Tracking 
* Try-on model testing and improvement 
* Network development
* Network testing and evaluation
* Deployment (flask)
* Demo UI Web Page

### Network Modules
|SMFAI NN | Human Pose Shape Estimation, video tracking input/output| LIP test data Cloth Mask| CP-VTON Inference |
|:------ |:------ | :----- | :----|
|Contributor  | [Mavis Wang](https://github.com/mavisw) | [Xiaocen Xie](https://github.com/tiffanyxxc) |  [Ililta Gebrihiwet](https://github.com/ililtaG), [Ting-wei (CoCo) Yu](https://github.com/cocosjsu) |


### Citation
@InProceedings{Minar_CPP_2020_CVPR_Workshops,
	title={CP-VTON+: Clothing Shape and Texture Preserving Image-Based Virtual Try-On},
	author={Minar, Matiur Rahman and Thai Thanh Tuan and Ahn, Heejune and Rosin, Paul and Lai, Yu-Kun},
	booktitle = {The IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
	month = {June},
	year = {2020}
}
