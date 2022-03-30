# Smart Mirror Fashion AI - video-based virtual tryon

This project is highly influenced by [Toward Characteristic-Preserving Image-based Virtual Try-On Network](https://arxiv.org/abs/1807.07688) 
and reproduced based on the repo [CP-VTON-Plus](https://github.com/minar09/cp-vton-plus) Network.


# Test Data
- Reference Person Try-On Video: public clothing website.
- Target Clothes: LIP, [FPI (Fashion Product Image)](https://www.kaggle.com/paramaggarwal/fashion-product-images-dataset)

# SMFAI Network 
- Input
	* Reference Person (Video)
	* Target Cloth Item (Image)
- Output
	* video body keypoints tracking
	* cloth transferring try-on video

# Modules
1. Garment Mask
3. Human Pose Shape Estimation
4. Try-on (CP-VTON-PLUS)
5. Video Pose Tracking


# Tasks
* Final test video
* Final cloth images
* Module development and testing
* Object Tracking 
* Try-on model testing and improvement 
* Network development
* Network testing and evaluation
* Deployment (flask)
* Demo Web Page

# Demo Video

### Citation
@InProceedings{Minar_CPP_2020_CVPR_Workshops,
	title={CP-VTON+: Clothing Shape and Texture Preserving Image-Based Virtual Try-On},
	author={Minar, Matiur Rahman and Thai Thanh Tuan and Ahn, Heejune and Rosin, Paul and Lai, Yu-Kun},
	booktitle = {The IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
	month = {June},
	year = {2020}
}
