<h2 align="center">탄소나노튜브 (carbon nanotubes, CNTs)</h2>

**- Computer Vision-based `Quality Evaluation(품질 평가)` of Carbon Nanotubes**

**- Quality Evaluation : (1) Whether or not dispersion processing, (2) Content of CNT**   

**- Model Performance is `0.90 and 0.89 accuracy`, respectively**

- **Data : Optical microscopy(광학 현미경) image**

- **Paper** : *preparing to the manuscript*

<br/>

## **Table of Contents** 
<b>

- [Abstract](#Abstract)
- [Tech and Tools](#Tech-and-Tools)
- [Code Implementation](#Code-Implementation)
  - [a. Data Analysis](#a.-Data-Analysis)
  - [b. Model Selection](#b.-Model-Selection)
  - [c. Model Evaluation](#c.-Model-Evaluation)
  
</b>
<br/>

## **Abstract**
- Although it is recognized as the next-generation new material for CNTs, there is no research on quality evaluation when used in construction materials.

- Optical microscope images of experimental samples are used as data.

- (1) Data Collections:  `binarize(greyscale)` the images and `augment` data

- (2) Data Pre-processing: `histogram stretching` to increase constant ratio(명암비)

- (3) Train Model: 1D-CNN with dual convolutional layers

- (4) Test Model: show confusion matrix
![]()
<br/>

## **Tech and Tools**
  <span><img src="https://img.shields.io/badge/Python-05122A?style=flat-square&logo=python"/></span>
  <span><img src="https://img.shields.io/badge/ScikitLearn-F7931E?style=flat-square&logo=ScikitLearn&logoColor=white"></span>
  
<br/>

## **Code Implementation**
<details>
<summary><b>Show Detailed Implementation</b></summary>
<div markdown="1">

### a. Data Analysis  
  **"Check (1) Distplot, (2) Outlier, (3) Clustering"**   
  
### b. Model Selection
**I used the following 5 models. So, combining these models, I useed the stakcing model as the final model. **
- Lasso(poly_degree=2)
- SVM
- GBM
- XGBoost
- RF
  
**The final model(stacking)'s `R^2 is 0.92`.** 

### c. Model Evaluation
- R^2 (main)
- R^2_adj
- MAPE
  
</div>
</details>





