<h2 align="center">Factory Design Research Project _ SK Hynix</h2>

**- `Design and Analysis` of low-vibration structural materials**

**- `Suggesting` cement mixture ratios for the objectives attainment`(cost reduction, strength and stiffness improvement)` using `machine learning`**   

**- Based on the existing [concrete compressive strength prediction study](https://github.com/P-uyoung/AI-research/tree/master/Concrete), the mixing ratio will be proposed.**

**- Studied the paper and code below, and attempted to reconstruct them as a Korean model.**

> **Data : [UC Irvine Machine Learning repository](https://archive.ics.uci.edu/ml/datasets/concrete+compressive+strength)**

> **Referenc Papers : (1) [IC. Yeh. 1998](https://www.sciencedirect.com/science/article/pii/S0008884698001653),  (2) [P.G. Asteris. 2021](https://www.sciencedirect.com/science/article/pii/S0008884621000983)**

> **Reference Code : [github.com_Pranov1984](https://github.com/Pranov1984/Prediction-of-cement-compressive-strength-using-stacked-ensemble-modelling/blob/master/Concrete%20Compressive%20Strength%20Prediction-V3.ipynb)**

<br/>

## **Table of Contents** 
<b>

- [Abstract](#Abstract)
- [Tech and Tools](#Tech-and-Tools)
- [Progress Stage](#Progress-Stage)
  - [Literature Survey](#1-Literature-Survey)
  - [Modeling](#2-Modeling)
  - [Experiment Design](#3-Experiment-Design)
  
</b>
<br/>


## **Abstract**
- (1)Lasso, (2)SVM, (3)XGBoost, (4)GBR, (5)RF, (6)Stacking 모델의 예측 성능이 결정계수 0.78~0.92임.   
![](https://github.com/P-uyoung/AI-research/blob/master/Concrete/Fig/baseModel_performance.png)

- (1)~(6)모델을 기반모델을 사용하여, Stacking 모델을 만들었으며, 모델의 `결정계수는 0.92`로 가장 높은 정확도를 보임.   
      <img src="https://github.com/P-uyoung/AI-research/blob/master/Concrete/Fig/metaModel_performance.png" width="250" height="250"/>  

- `(타겟특성)압축강도` 예측에 영향이 높은 입력변수`(Feature Importance)는 '재령일 > 시멘트양 > 물의양 > 슬래그양 > SP양 > 잔골재' 순`임.   
      <img src="https://github.com/P-uyoung/AI-research/blob/master/Concrete/Fig/Feature_Importance.png" width="679" height="280"/>

<br/>

## **Tech and Tools**
  <span><img src="https://img.shields.io/badge/Python-05122A?style=flat-square&logo=python"/></span>
  <span><img src="https://img.shields.io/badge/ScikitLearn-F7931E?style=flat-square&logo=ScikitLearn&logoColor=white"></span>
  
<br/>

## **Progress Stage**
<details>
<summary><b>구현 설명 펼치기</b></summary>
<div markdown="1">

</div>
</details>

<br/>
