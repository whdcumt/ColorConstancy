
# MISC

## Introduction

The proposed mean maximum vitrinite reflectance (MMVR) measurement based on machine learning approach, MMVRML, based on adaptive image segmentation,vitrinite identification 
and MMVR estimation makes it possible to estimate MMVR automatically and intelligently.
We integrated image segmentation algorithm based on adaptive K-means clustering, various classification algorithms and random forest algorithm for regression  
described in the following paper:
"Intelligent estimation of vitrinite reflectance of coal from photomicrographs based on machine learning" submitted to Minerals.

**Note**: this package requires installing Matlab **R2016b** or latter.

## Usage

1. The software of MMVRML was implemented in Matlab, and could be run on
Windows systems without installing. MMVRML distributions for Windows can be found at 
https://github.com/GuyooGu/MMVRML. We recommend that users can download the latest release. 

2.After downloading, please double-click on the file 'MMVRML.exe' to run the executable file：MMVRML.exe

3.Select an image（such as 'TestImage_Ref_0.7.bmp' in the folder 'testimage' ） for analysis.

4.Select a calssification method for vitrinite identification, and this procedure may take several seconds, after we get the segmentation results (subfigure b)and the identified 
vitrinite region （subfigure c）,select the regression method(random forest)for MMVR estimation,the estimated MMVR value is shown in subfigure(d).

5.Click on the left or right arrow to change the image to be processed, and all the estimated MMVR value can be saved in a Excel file,in addition, the results of segmentation and classification
can be saved too.

## FeedBack 

Any suggestion and problem, please feel free to let us know via Email: liangzou@ece.ubc.ca.

## License 

Released under MIT license




