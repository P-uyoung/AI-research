<h2 align="center">Factory Design Research Project _ SK Hynix</h2>

**- `Design and Analysis` of low-vibration structural materials**

**- `Suggesting` cement mixture ratios for the `objectives attainment (cost reduction, strength and stiffness improvement)` using `machine learning`**   

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
- [(Ongoing) Progress Stage](#Progress-Stage)
  - [Literature Survey](#1-Literature-Survey)
  - [Modeling](#2-Modeling)
  - [Experiment Design](#3-Experiment-Design)
  
</b>
<br/>


## **Abstract**
- Korean `compressive strength data` according to the cement mixture were collected through literature survey. First, domestic data were applied to the overseas model of the existing compressive strength prediction study. As a result, Korean data is not applicable to overseas models. (The coefficient of determination was negative.) Therefore, `a Korean model was created using the gradient boosting machine(GBM).`
- Through this model, I would like to propose `Cement Mixture for Reducing Unit Price and Improving Strength of Low Vibration Plant` required by `SK Hynix`. However, since the quality of the data used in the model is different from that of the target data, the `experiment` according to the `six cement mixtures suggested through the ML model` is planned `to verify the objectives attainment`. The experiment will be conducted when the material arrives from the SNNC company.

<!-- ![](https://github.com/P-uyoung/AI-research/blob/master/Concrete/Fig/baseModel_performance.png)
<img src="https://github.com/P-uyoung/AI-research/blob/master/Concrete/Fig/Feature_Importance.png" width="679" height="280"/> -->

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
