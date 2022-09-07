# IDBNet
* This repository provides the code for our accepted paper on the 【ASOC 2022】"An interactive dual-branch network for hard palate segmentation of the oral cavity from CBCT images"
* Official implementation of [IDBNet](https://www.sciencedirect.com/science/article/pii/S1568494622006184)
## Introduction
Automatic and accurate segmentation of the hard palate from Cone Beam and Computed Tomography (CBCT) images is a fundamental task for the insertion of orthodontic mini-implants. U-Net and its variants fail to handle it well when facing the hard palate with diversity of shape. Further, hard palate has low-density soft tissues and high-density hard bones so as to exhibit different intensity of regions in CBCT images, which may result in mis-segmentation or missing-segmentation. Motivated by these challenges, a novel Interactive Dual-Branch Network (IDBNet) is presented to achieve automatic and accurate the hard palate segmentation of the oral cavity from CBCT images. Specifically, we introduce the designs for hard palate segmentation as follows: (1) Dual-branch encoder–decoder is developed for hard palate with the ability of data expansion and extracting multi-scale interactive features. (2) Channel map interaction module is proposed to reinforce the cross-channel information communication between different level features, thereby enhancing feature representations for variable hard palate. (3) Guide map interaction module is designed to model the similarities and differences of dual-branch hard palate boundaries. Owing to the remarkable designs, our IDBNet has the ability to gradually mine ambiguous hard palate affected by different intensity of regions. Moreover, we collected an in-house dataset with 30 challenging cases, which contained 2260 CBCT slices. Among them, 70% for training and 30% for testing are considered. Five-fold cross-validation experiments on this dataset demonstrate that our method outperforms the Res-UNet method by 8.05% of mean Dice score and 7.97% of structure measure. The utilisation of our proposed segmentation approach for hard palate of the oral cavity warrants further investigation on implantable area, which could aid in formulating clinical plans on the insertion regions of palatal mini-implants.

<div align=center><img width="400" height="800" alt="Our TBraTS framework" src="https://github.com/Cocofeat/IDBNet/blob/main/image/Teeth_E.gif"/></div>

## Requirements
Some important required packages include:  
Pytorch version >=0.4.1.  
Visdom  
Python == 3.7  
Some basic python packages such as Numpy.  
##  :fire: NEWS :fire:
* [08/30] We will release the code as soon as possible. 
## Citation
If you find our work is helpful for your research, please consider to cite:  
```
@journal{Coco2022IDBNet,
  title={An interactive dual-branch network for hard palate segmentation of the oral cavity from CBCT images},
  author={Zou, Ke and Tianjin, Tao and Xuedong, Yuan and Xiaojing, Shen and Wenli, Lai and Hu, Long},
  journal={Applied Soft Computing},
  year={2022}
  doi={https://doi.org/10.1016/j.asoc.2022.109549}
}
```
## Acknowledgement
Part of the code is revised from [PraNet](https://github.com/DengPingFan/PraNet)

## Contact
* If you have any problems about our work, please contact [me](kezou8@gmail.com) 
* Project Link: [IDBNet](https://github.com/Cocofeat/IDBNet/)
