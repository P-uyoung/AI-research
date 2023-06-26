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
-The prediction performances of (1)Lasso, (2)SVM, (3)XGBoost, (4)GBR, (5)RF models fall `between 0.78 and 0.92 of R^2` (Coefficient of Determination).   
![](https://github.com/P-uyoung/AI-research/blob/master/Concrete/Fig/baseModel_performance.png)

-A stacking model was created using the (1)~(5) models as the base models, and the `R^2 of model is 0.92`, showing the highest accuracy.   
      <img src="https://github.com/P-uyoung/AI-research/blob/master/Concrete/Fig/metaModel_performance.png" width="250" height="250"/>  

-The input features that has a high `influence` on the prediction of (target feature)compressive strength is `in the order of age > cement amount > water amount > slag amount > SP amount > coarse aggregate(CA) amount`.
      <img src="https://github.com/P-uyoung/AI-research/blob/master/Concrete/Fig/Feature_Importance.png" width="679" height="280"/>

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





