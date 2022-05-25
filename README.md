#### Data298 MSDA Project 2022.05<br>
Team 8: Mavis Wang, Coco Yu, Xiaocen Xie, Ililta Gebrihiwet

# Smart Mirror Fashion AI
A video virtual try-on network using CP-VTON-PLUS.

### SMFAI Network
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

### Human Video Data-Processing
<img src = 'https://raw.githubusercontent.com/SJSUMS/SMFAI/main/data_process_pipe.png' width="800"></img>

### Human Pose Shape model Improvement
- Improved pose tracking
- Improved human parsing (fixed-neck)
- Improved body pose estimation <br>

### Test Results
<img src="https://raw.githubusercontent.com/SJSUMS/SMFAI/main/samples/SMFAI_VVT.gif"></img><br>
<img width=800 src="https://raw.githubusercontent.com/SJSUMS/SMFAI/main/samples/SMFAI_custom.png"></img>


## [Project Management](https://github.com/SJSUMS/SMART-MIRROR-FASHION-AI_SMFAI/blob/main/298_T8_Roadmap.pdf)

### SMFAI Modules
- [x] Video Processing and Tracking @ Mavis Wang
- [x] Garment Mask @ Xiaocen Xie
- [x] Human body Pose Shape Estimation @ Mavis Wang
- [x] CP-VTON GMM @ Ililta Gebrihiwet
- [x] CP-VTON TOM @ Coco Yu

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

### Final Demo [Slide](https://github.com/SJSUMS/SMFAI/blob/main/Slide.pdf)
- [x] Evaluation @ Xiaocen Xie
- [x] Modeling @ Coco Yu
- [x] Testing Results @ Mavis Wang
- [x] [Model Integration](https://youtu.be/OKBlrNRCLjs) @ Mavis Wang
- [x] Web App Portal @ Ililta Gebrihiwet

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
