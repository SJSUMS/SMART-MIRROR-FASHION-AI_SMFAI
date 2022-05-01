# Smart Mirror Fashion AI - video-based virtual tryon
### Features

### Contributions

## Test Data
- Reference Person Try-On Video: public clothing website.
- Target Clothes: LIP, [FPI (Fashion Product Image)](https://www.kaggle.com/paramaggarwal/fashion-product-images-dataset)

## SMFAI Network 
### Input
	* Reference Person (Video)
	* Target Cloth Item (Image)
### Output
	* body keypoints tracking video
	* cloth transferring try-on video

## Modules
1. Garment Mask
3. Human Pose Shape Estimation
4. Try-on (CP-VTON-PLUS)
5. Video Pose Tracking


## Tasks
0. [x] Data collection
1. [x] Finalize test dataset - ref_person video
2. [x] Finalize test dataset - target cloth
3. [x] Individual module development, testing, and improvement
4. [x] Test Video Object Tracking
5. [x] SMFAI network pipeline testing 
6. [x] Network development
7. [x] Network testing
8. [x] Network evaluation
9. [ ] Deployment (Flask)
10. [ ] Demo Web Page

## Demo
[System Integration Video](https://youtu.be/OKBlrNRCLjs)

### Citation
	@InProceedings{Minar_CPP_2020_CVPR_Workshops,
		title={CP-VTON+: Clothing Shape and Texture Preserving Image-Based Virtual Try-On},
		author={Minar, Matiur Rahman and Thai Thanh Tuan and Ahn, Heejune and Rosin, Paul and Lai, Yu-Kun},
		booktitle = {The IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
		month = {June},
		year = {2020}
	}
	
This project is highly influenced by [Toward Characteristic-Preserving Image-based Virtual Try-On Network](https://arxiv.org/abs/1807.07688) 
and reproduced based on the repo [CP-VTON-Plus](https://github.com/minar09/cp-vton-plus) Network.
