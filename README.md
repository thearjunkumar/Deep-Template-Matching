# Deep-Template-Matching
Learning Accurate Template Matching with Differentiable Coarse-to-fine Correspondence Refinement

Official implementation of Deep-Template-Matching (Learning Accurate Template Matching with Differentiable Coarse-to-fine Correspondence Refinement) using pytorch ([pytorch-lightning](https://github.com/Lightning-AI/lightning))
This paper has accepted by [CVMJ 2023](https://www.springer.com/journal/41095), the manuscript is coming soon.

## Abstruct
Template matching is a fundamental task in computer vision and has been studied for decades. It plays an essential role in the manufacturing industry for estimating the poses of different parts, facilitating downstream tasks such as robotic grasping. Existing works fail when the template and source images are in different modalities, cluttered backgrounds or weak textures. They also rarely consider geometric transformations via homographies, which commonly existed even for planar industrial parts. To tackle the challenges, we propose an accurate template matching method based on differentiable coarse-to-fine correspondence refinement. Considering the domain gap between the mask template and the grayscale image, we leverage an edge-aware module to eliminate the difference for robust matching. Based on coarse correspondences with novel structure-aware information by transformers, an initial warping transformation is estimated and performed as a preliminary result. After the initial alignment, we execute a refinement network on reference and aligned images to obtain sub-pixel level correspondences and thus obtain the final geometric transformation. Comprehensive evaluations show that our method significantly outperforms state-of-the-art methods and baselines, with good generalization abilities and visually plausible results even on unseen real data.


## Introduction
we propose an accurate template matching method based on differentiable coarse-to-fine correspondence refinement. Considering the
domain gap between the mask template and the grayscale image, we leverage an edge-aware module to eliminate the difference for robust matching. Based on coarse correspondences with novel structure-aware information by transformers, an initial warping transformation is estimated and performed as a preliminary result. After the initial alignment, we execute a refinement network on reference and aligned images to obtain sub-pixel level correspondences and thus obtain the final geometric transformation. 

![image](https://github.com/zhirui-gao/Deep-Template-Matching/blob/demos/teaser.png)



## Installation
We provide the [download link](https://drive.google.com/drive/folders/1Mu9QdnM5WsLccFp0Ygf7ES7mLV-64wRL?usp=sharing) to
- Assembled hole dataset
- Mechanical parts dataset

## Demos


### Single-object demo

![Output sample](https://github.com/zhirui-gao/Deep-Template-Matching/blob/demos/single_object.gif)

### Multi-objects demo
![s](https://github.com/zhirui-gao/Deep-Template-Matching/blob/demos/multi_object.gif)


## Acknowledgements
- [LoFTR](https://github.com/zju3dv/LoFTR)  
- [SuperGlue](https://github.com/magicleap/SuperGluePretrainedNetwork)
- [pidinet](https://github.com/zhuoinoulu/pidinet)
- [PointDSC](https://github.com/XuyangBai/PointDSC)
