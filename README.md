# MMVRML

## Introduction

Vitrinite reflectance  (VR), the percentage of incident light reflected from a polished vitrinite surface, is the most definitive maturation parameter to characterize the maturation process of coal [1, 2]. The mean maximum vitrinite reflectance (MMVR), one of the most important types of VR, is widely accepted as an important and desirable means for evaluating the potential usefulness of coals in a series of applications [3] , such as determining coal blending procedures, evaluating coal’s suitability for hydrogenation, identification of potential sites for exploration, and so on [4, 5]. The accurate measurement of vitrinite reflectance (especially for mean maximum vitrinite reflectance, MMVR) is an important issue in the fields of coal mining and processing. Inspired by the way that petrologists measure vitrinite reflectance, an automatic framework to estimate MMVR is presented in this study. The MMVR estimation system includes three major procedures, including image segmentation, vitrinite identification and MMVR regression. We employed adaptive K-means clustering to automatically search the optimal number of clusters (i.e., maceral groups) in each photomicrograph, and therefore the users do not need to specify the number of maceral groups in each photomicrograph. Furthermore, inspired by the way that petrologists examine photomicrographs and considering the complicated nature of coal, we investigated four popular classification methods to identify the regions with vitrinite. Based on RBF-SVM along with 112 discriminative features, the proposed strategy is able to classify vitrinite properly in over 97.10% cases. For the purpose of enhancing the robustness and reliability of the proposed method, the largest vitrinite within each photomicrograph was selected for estimating MMVR. We split the selected vitrinite region into grid squares with the size of 41×41px. 15 simplified grayscale features were employed to estimate MMVR values based on five intelligent regression models. The random forest provides the most optimal results with R-square of 0.9839. Our results suggest that machine learning-based maceral analysis will be a promising direction in geology.

**Note**: this package requires installing Matlab **R2016b** or latter.

## Usage

1.The software of MMVRML was implemented in Matlab, and could be run on
Windows systems without installing. MMVRML distributions for Windows can be found at 
https://github.com/GuyooGu/MMVRML. We recommend that users can download the latest release. 

2.After downloading, please double-click on the file 'MMVRML.exe' to run the executable file：MMVRML.exe

3.Select an image（such as 'TestImage_Ref_0.7.bmp' in the folder 'testimage' , the last digits '0.7' is the ground truth MMVR）for analysis.

4.Select a calssification method for vitrinite identification, and select the regression method (random forest) for MMVR estimation. This procedure may take several seconds. The segmentation results  is shown in subfigure (b) and the identified vitrinite region is shown in subfigure (c), the estimated MMVR value is shown in subfigure (d).

5.Click on the left or right arrow to change the image to be processed. If we don't change the classification algorithm, the system will adopt the same one in the last time, and all the estimated MMVR value can be saved in an Excel file. 


## Updation

Our software will be updated routinely based on users’suggestions and advice. Thus, your feedback is greatly important for our future upgrading. Please do not hesitate to contact with us if you have any concerns.

## Citation 
We hope you can cite the article if the software has been helpful for your work.                
[1]  Wang, H.; et al., Intelligent estimation of vitrinite reflectance of coal from photomicrographs based on machine learning. Submitted to Minerals, 2019.

## FeedBack 

Any suggestion and problem, please feel free to let us know via Email: liangzou@ece.ubc.ca.  Thanks a lot.

## License 

Released under MIT license

## Reference  

 1. Chen, Y.; Qin, Y.; Li, Z.; Shi, Q.; Wei, C.; Wu, C.; Cao, C.; Qu, Z. Differences in desorption rate and composition of desorbed gases between undeformed and mylonitic coals in the Zhina Coalfield, Southwest China. FUEL 2019, 239, 905-916.
 2. Mählmann, R.F.; Le Bayon, R. Vitrinite and vitrinite like solid bitumen reflectance in thermal maturity studies: Correlations from diagenesis to incipient metamorphism in different geodynamic settings. INT J COAL GEOL 2016, 157, 52-73.
 3. Unsworth, J.F.; Gough, H. Characterization of coals by automated optical image analysis 2. Inertinite reflectance. J MICROSC-OXFORD 2011, 156, 327-342.
 4. Dembicki, J.H. Chapter 3 - Source Rock Evaluation. In Practical Petroleum Geochemistry for Exploration and Production; Dembicki, J. H., Ed Elsevier: 2017; pp. 61-133.
 5. Flores, R.M. Chapter 4 - Coalification, Gasification, and Gas Storage. In Coal and Coalbed Gas; Flores, R. M., Ed Elsevier: Boston, 2014; pp. 167-233.


