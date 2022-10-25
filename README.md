# Deep-Template-Matching
Learning Accurate Template Matching with Differentiable Coarse-to-fine Correspondence Refinement

Official implementation of Deep-Template-Matching (Learning Accurate Template Matching with Differentiable Coarse-to-fine Correspondence Refinement) using pytorch ([pytorch-lightning](https://github.com/Lightning-AI/lightning))


## Introduction
we propose an accurate template matching method based on differentiable coarse-to-fine correspondence refinement. Considering the
domain gap between the mask template and the grayscale image, we leverage an edge-aware module to eliminate the difference for robust matching. Based on coarse correspondences with novel structure-aware information by transformers, an initial warping transformation is estimated and performed as a preliminary result. After the initial alignment, we execute a refinement network on reference and aligned images to obtain sub-pixel level correspondences and thus obtain the final geometric transformation. 

##



## Installation
We provide the [download link](https://drive.google.com/drive/folders/1Mu9QdnM5WsLccFp0Ygf7ES7mLV-64wRL?usp=sharing) to
- Assembled hole dataset
- hole dataset

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
