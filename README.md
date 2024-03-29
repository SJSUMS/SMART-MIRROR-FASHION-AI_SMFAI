#### Data298 MSDA Project 2022.05<br>
Team 8: Mavis Wang, Coco Yu, Xiaocen Xie, Ililta Gebrihiwet

# Smart Mirror Fashion AI
A smart-mirror-based fashion AI using CP-VTON-PLUS.

## Network Integration
<img src="https://raw.githubusercontent.com/SJSUMS/SMFAI/main/video_tryOn_system_pipe.png"></img>

### Input
	* Reference Person (Video)
	* Target Cloth Item (Image)
### Output
	* body keypoints tracking video
	* cloth transferring try-on video

### Dataset
- [Processed train/test VTON](https://drive.google.com/file/d/19RCQFjkbFaufXU518KAtkQtlfhTd9hsj/view?usp=sharing)
- [Processed Custom Person Video](https://github.com/SJSUMS/SMFAI/tree/main/data)
- [Processed CP-VTON Clothing and Mask](https://drive.google.com/file/d/19RCQFjkbFaufXU518KAtkQtlfhTd9hsj/view?usp=sharing)

## Video Pre-processing Pipeline
<img src = 'https://raw.githubusercontent.com/SJSUMS/SMFAI/main/data_process_pipe.png' width="800"></img>

## Key Improvement
- Improved pose tracking
- Improved human parsing (fixed-neck)
- Improved body pose estimation <br>

## Results
<img src="https://raw.githubusercontent.com/SJSUMS/SMFAI/main/samples/SMFAI_VVT.gif"></img><br>


## [Project Management](https://github.com/SJSUMS/SMART-MIRROR-FASHION-AI_SMFAI/blob/main/298_T8_Roadmap.pdf)

### SMFAI Modules
- [x] Video Processing and Tracking
- [x] Garment Mask
- [x] Human body Pose Shape Estimation
- [x] CP-VTON GMM
- [x] CP-VTON TOM

### Tasks
- [x] Roadmap
- [x] Data collection
- [x] Finalize test dataset - ref_person video
- [x] Finalize test dataset - target cloth
- [x] Individual module development, testing, and improvement
- [x] Test Video Object Tracking
- [x] SMFAI network pipeline testing
- [x] Network development
- [x] Network testing
- [x] Network evaluation
- [x] Models integration

### Citation
	@InProceedings{SJSU MSDA Program Project SMFAI,
		title={Smart Mirror-Based Fashion AI Based on Machine Learning},
		author={Mavis Wang, Coco Yu, Xiaocen Xie, Ililta Gebrihiwet},
		month = {May},
		year = {2022}
	}
	@InProceedings{Minar_CPP_2020_CVPR_Workshops,
		title={CP-VTON+: Clothing Shape and Texture Preserving Image-Based Virtual Try-On},
		author={Minar, Matiur Rahman and Thai Thanh Tuan and Ahn, Heejune and Rosin, Paul and Lai, Yu-Kun},
		booktitle = {The IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
		month = {June},
		year = {2020}
	}
	
This project is highly influenced by [Toward Characteristic-Preserving Image-based Virtual Try-On Network](https://arxiv.org/abs/1807.07688) 
and reproduced based on the repo [CP-VTON-Plus](https://github.com/minar09/cp-vton-plus) Network.
