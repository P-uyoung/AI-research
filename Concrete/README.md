<h2 align="center">Prediction of Concrete Compressive Strength</h2>

**- Improved the prediction performance of compressive strength of concrete using `ML model(Lasso, SVM, XGBoost, GBR, RF, Stacking)`**

**- `3% (0.89 -> 0.92 R^2)` performance improvement**   

**- (Toy Project) To improve model performance, I studied existing research and code**

**- `Studied` based on the following papers and code, and `remodeled` them.**

> **Data : [UC Irvine Machine Learning repository](https://archive.ics.uci.edu/ml/datasets/concrete+compressive+strength)**

> **Reference Papers : (1) [IC. Yeh. 1998](https://www.sciencedirect.com/science/article/pii/S0008884698001653),  (2) [P.G. Asteris. 2021](https://www.sciencedirect.com/science/article/pii/S0008884621000983)**

> **Reference Code : [github.com_Pranov1984](https://github.com/Pranov1984/Prediction-of-cement-compressive-strength-using-stacked-ensemble-modelling/blob/master/Concrete%20Compressive%20Strength%20Prediction-V3.ipynb)**

<br/>

## **Table of Contents** 
<b>

- [Abstract](#Abstract)
- [Tech and Tools](#Tech-and-Tools)
- [Code Implementation](#Code-Implementation)
  - [a. Data Analysis](#1-Data-Analysis)
  - [b. Model Selection](#2-Model-Selection)
  - [c. Model Evaluation](#3-Model-Evaluation)
  
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

### A. Data Analysis  
  **"Check (1) Distplot, (2) Outlier, (3) Clustering"**   
  
### B. Data Proprocessing 
**I used the following 5 models, and XGBoost is the final model. The model's `R^2 is 0.74`.**
  
- SVM
- GBM
- XGBoost
- RF
- Stacking
  
<br/>




