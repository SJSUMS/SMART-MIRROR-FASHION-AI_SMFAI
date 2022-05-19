# Smart Mirror Fashion AI - video-based virtual tryon
## A Video-based virtual try-on using image-based CP-VTON+ repo.
- Improved human parsing
- Improved body pose <br>
<img src="https://raw.githubusercontent.com/SJSUMS/SMFAI/main/samples/SMFAI_VVT.gif"></img>

### Required Data Pre-Processing (for CP-VTON+) Pipeline
<img src = 'https://raw.githubusercontent.com/SJSUMS/SMFAI/main/data_process_pipe.png' width="800"></img>

## Training Data
- [Vition](https://drive.google.com/file/d/14tKmGjpt2rjvc4n8kkpdqs73EfUN0ys_/view?usp=sharing)
- [VITON_PLUS](https://1drv.ms/u/s!Ai8t8GAHdzVUiQQYX0azYhqIDPP6?e=4cpFTI)
- [processed train/test](https://1drv.ms/u/s!Ai8t8GAHdzVUiQQYX0azYhqIDPP6?e=4cpFTI)

## Test Data
- Reference Person Try-On Video: custom, VVT, online shop.
- Target Clothes: LIP, [FPI (Fashion Product Image)](https://www.kaggle.com/paramaggarwal/fashion-product-images-dataset)
- [CP-VTON-Plus (Google Drive)](https://drive.google.com/file/d/19RCQFjkbFaufXU518KAtkQtlfhTd9hsj/view?usp=sharing)

## SMFAI Network 
<img src="https://raw.githubusercontent.com/SJSUMS/SMFAI/main/video_tryOn_system_pipe.png"></img>
### Input
	* Reference Person (Video)
	* Target Cloth Item (Image)
### Output
	* body keypoints tracking video
	* cloth transferring try-on video

## Related Models
1. OpenPose Keypoints
2. SCHP Body Parsing
3. CP-VTON+ (Inference)

## [Tasks and Roadmap](https://docs.google.com/document/d/1MXUAQKdEA03zjPbgdNf1WuMQgRmi9ZkXiTjHhuz830Y/)

## Sample Results & Demo
- [Model Integration Video](https://youtu.be/OKBlrNRCLjs)
- [Sample try-on Results (Custom and VVT Dataset)](https://youtube.com/shorts/ptAGrvSjFB8)

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
