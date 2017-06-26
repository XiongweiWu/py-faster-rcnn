# Under Construction

### Disclaimer

This repository contains python implementation of **Perceptual Generative Adversarial Network for Small Object Detection**. 

# Perceptual Generative Adversarial Network for Small Object Detection
This paper is from:

	@article{li2017perceptual,
			title={Perceptual Generative Adversarial Networks for Small Object Detection},
			author={Li, Jianan and Liang, Xiaodan and Wei, Yunchao and Xu, Tingfa and Feng, Jiashi and Yan, Shuicheng},
			journal={arXiv preprint arXiv:1706.05274}, 
			year={2017}
	}


### Training Process

PGAN consists three Training steps, P branch Training, A branch Training and G branch Training.

1. In P branch training, the parameters in Generator and A branch are fixed, only P branch and Backbone are trained. In this step, only large objects are trained.

2. In G branch training, the parameters in Generator are trained, with the standard G loss. Other parameters are fixed. Only small objects are trained.

3. In A branch training, The parameters in A branch are trained, with the standard A loss. Other parameters are fixed. Here all objects are trained.

4. Repeat step 2 and step 3 iteratively until converge.



