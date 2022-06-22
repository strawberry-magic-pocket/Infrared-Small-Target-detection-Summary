# Infrared-Small-Target-detection-Summary
This is a summary of infrared small target detection algorithms in single-frame infrared images.  
## DataSets
- [SIRST](https://github.com/YimianDai/sirst): SIRST is a dataset for single-frame infrared small target detection. As far as I know, it is the only open dataset and they provided the images with five kinds of annotations to support image classification, instance segmentation, bounding box regression, semantic segmentation, and instance spoting.
  * Yimian Dai, Yiquan Wu, Fei Zhou, Kobus Barnard; Proceedings of the IEEE/CVF Winter Conference on Applications of Computer Vision (WACV), 2021, pp. 950-959.[ ![](https://img.shields.io/badge/link-paper-blue)](https://openaccess.thecvf.com/content/WACV2021/html/Dai_Asymmetric_Contextual_Modulation_for_Infrared_Small_Target_Detection_WACV_2021_paper.html)
- [Dataset for infrared image dim-small aircraft target detection and tracking under ground / air background](http://www.dx.doi.org/10.11922/sciencedb.902): The dataset is provided by the National University of Defense Technology(NUDT). [![](https://img.shields.io/badge/link-paper-blue)](https://www.aeroweaponry.avic.com/CN/10.12132/ISSN.1673-5048.2019.0234)
- Others
 
   I have collected some infrared images containing small targets from Github, and have uploaded them to this repository. You can download and use them, but **please don't forget to cite the original authors' literatures**.
## Papers
### I. Background Characteristics-Based methods
These methods are widely used to estimate the background so as to achieve target detection according to the difference between the original infrared images and the evaluated background.
1. **Top-hat** 
    * Victor T. Tom, Tamar Peli, *et al..* The morphology-based algorithm for point target detection in infrared backgrounds[J].Signal and Data Processing of Small Targets,1993. [ ![](https://img.shields.io/badge/link-paper-blue)](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/1954/0000/Morphology-based-algorithm-for-point-target-detection-in-infrared-backgrounds/10.1117/12.157758.short)
    * Xiangzhi Bai, Fugen Zhou. Analysis of new top-hat transfromation and the application for infrared dim small target detection[J]. Pattern recognition, 2010.[![](https://img.shields.io/badge/link-paper-blue)](https://www.sciencedirect.com/science/article/abs/pii/S0031320310000105)
 
2. **Max-mean/ Max-median**
   * Suyog D. Deshpande, *et al..* Max-mean and max-median filters for detection of small targets[J]. Signal and Data Processing of Small Targets, 1999.[![](https://img.shields.io/badge/link-paper-blue)](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/3809/0000/Max-mean-and-mamedian-filters-for-detection-of-small/10.1117/12.364049.short?SSO=1)
   
3. **Two-Dimensional Least Mean Square(TDLMS)**
   * Yuan Cao, RuiMing Liu, Jie Yang. Small Target Detection Using Two-Dimensional Least Mean Square (TDLMS) Filter Based on Neighborhood Analysis[J]. International Journal of Infrared Millimeter Waves, 2008.[![](https://img.shields.io/badge/link-paper-blue)](https://link.springer.com/article/10.1007/s10762-007-9313-x#citeas)
   * Pingyue Lv, Shengli Sun, *et all..* Space moving target detection and tracking method in complex background[J]. Infrared Physics & Technology, 2018. [![](https://img.shields.io/badge/link-paper-blue)](https://www.sciencedirect.com/science/article/abs/pii/S135044951730600X)

### II. Target Characteristics-Based Methods [![](https://img.shields.io/badge/code-Matlab-orange)](https://github.com/moradisaed?tab=repositories)
The main idea of these methods is to use the local information in the spatial domain to construct a saliency map.

  #### Local contrast method and its improved versions
1. **LCM**
   * C.L.Philip Chen, Hong Li, *et al..* A Local Contrast Method for Small Infrared Target Detection[J]. IEEE Transactions on Geoscience and Remote Sensing, 2013.[![](https://img.shields.io/badge/link-paper-blue)](https://ieeexplore.ieee.org/abstract/document/6479296)
  
2. **ILCM**
   * Jinhui Han, Yong Ma, *et al..* A Robust Infrared Small Target Detection Algorithm Based on HUman Visual System[J]. IEEE Geoscience and Remote Sensing Letters, 2014.[![](https://img.shields.io/badge/link-paper-blue)](https://ieeexplore.ieee.org/document/6819810)
  
3. **MPCM**
   * Yantao Wei, Xinge You, Hong Li. Multiscale patch-based contrast measure for small infrared target detection[J]. Pattern Recognition, 2016. [![](https://img.shields.io/badge/link-paper-blue)](https://www.sciencedirect.com/science/article/pii/S0031320316300358)
 
4. **RLCM**
   * Jinhui Han, Kun Liang, *et al..* Infrared Small Target Detection Utilizing the Multiscale Relative Local Contrast Measure[J]. IEEE Geoscience and Remote Sensing Letters, 2014.[![](https://img.shields.io/badge/link-paper-blue)](https://ieeexplore.ieee.org/abstract/document/8289318)
   
5. **WLDM**
   * He Deng, Xianping Sun, *et al..* Small Infrared Target Detection Based on Weighted Local Difference Measure[J]. IEEE Transactions on Geoscience and Remote Sensing, 2013.[![](https://img.shields.io/badge/link-paper-blue)](https://ieeexplore.ieee.org/document/7460907)
   
#### Filter-kernel
1. **LoG**
   * Sungho Kim, Yukyung Yang, *et al..* Small Target Detection Utilizing Robust Methods of the Human Visual System for IRST[J]. Journal of Infrared, Millimeter, and Terahertz Waves, 2009.[![](https://img.shields.io/badge/link-paper-blue)](https://link.springer.com/article/10.1007/s10762-009-9518-2)

2. **DoG**
  * Xin Wang, Guofang Lv, Lizhong Xu. Infrared dim target detection based on visual attention[J]. Infrared Physics & Technology, 2018. [![](https://img.shields.io/badge/link-paper-blue)](https://www.sciencedirect.com/science/article/pii/S1350449512000801)

3. **IDoGb**
   * Jinhui Han, Yong Ma, *et al..* An Infrared Small Target Detecting Algorithm Based on Human Visual System[J]. IEEE Geoscience and Remote Sensing Letters, 2014.[![](https://img.shields.io/badge/link-paper-blue)](https://ieeexplore.ieee.org/abstract/document/7399358)

#### Gray-difference
1. **ADMD**
   * Saed Moradi, Payman Moallem, *et al..* Fast and robust small infrared target detection using absolute directional mean difference algorithm[J]. Signal Processing, 2020. [![](https://img.shields.io/badge/link-paper-blue)](https://www.sciencedirect.com/science/article/pii/S016516842030270X)

### III. Matrix-Optimal Based Methods
1. **IPI**
   * Chenqiang Gao, Deyu Meng, *et al..* Infrared Patch-Image Model for Small Target Detection in a Single Image[J].
   
     [![](https://img.shields.io/badge/link-paper-blue)](https://ieeexplore.ieee.org/abstract/document/6595533) [![](https://img.shields.io/badge/code-Matlab-orange)](https://github.com/gaocq/IPI-for-small-target-detection)

2. **RIPT**
   * Yimian Dai, Yiquan Wu. Reweighted Infrared Patch-Tensor Model With Both Nonlocal and Local Priors for Single-Frame Small Target Detection[J]. IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, 2017. 
  
     [![](https://img.shields.io/badge/link-paper-blue)](https://ieeexplore.ieee.org/abstract/document/7932858) [![](https://img.shields.io/badge/code-Matlab-orange)](https://github.com/YimianDai/DENTIST)
     
     
## Someone else
[Awesome Infrared Small Target](https://github.com/Tianfang-Zhang/awesome-infrared-small-targets)


   


 





      


