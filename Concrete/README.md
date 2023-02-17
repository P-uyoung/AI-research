<h2 align="center">Prediction Concrete Compressive Strength</h2>

**- ML모델 `(Lasso, SVM, XGBoost, GBR, RF, Stacking_ensemble)`을 사용하여 콘크리트 압축강도 예측 성능 향상**

**- (토이 프로젝트) 기존 연구 및 코드를 공부하여, 예측 성능 향상시킴**

**- 다음 논문 및 코드를 기반으로 공부하여, 재모델링 해봄.**

> **데이터 : [UC Irvine Machine Learning repository](https://archive.ics.uci.edu/ml/datasets/concrete+compressive+strength)**

> **참고논문 : [IC. Yeh. 1998](https://www.sciencedirect.com/science/article/pii/S0008884698001653),   [P.G. Asteris. 2021](https://www.sciencedirect.com/science/article/pii/S0008884621000983)**

> **참고코드 : [github.com_Pranov1984](https://github.com/Pranov1984/Prediction-of-cement-compressive-strength-using-stacked-ensemble-modelling/blob/master/Concrete%20Compressive%20Strength%20Prediction-V3.ipynb)**

<br/>

## **목차** 
<b>

- [요약](#요약)
- [기술 및 도구](#기술-및-도구)
- [구현](#구현)
  - [프로세스](#1-프로세스)
  - [데이터](#2-데이터)
  - [모델링](#3-모델링)
- [트러블 슈팅](#트러블-슈팅)
</b>
<br/>


## **요약**
- (1)Lasso, (2)SVM, (3)XGBoost, (4)GBR, (5)RF, (6)Stacking 모델의 예측 성능이 결정계수 0.78~0.92임.   
![](https://github.com/P-uyoung/AI-research/tree/master/Concrete/Fig/graph_base model performance.png)   

- (1)~(6)모델을 기반모델을 사용하여, Stacking 모델을 만들었으며, 모델의 `결정계수는 0.92`로 가장 높은 정확도를 보임.   
![](https://github.com/P-uyoung/AI-research/tree/master/Concrete/Fig/graph_base model performance.png)   

- `(타겟특성)압축강도` 예측에 영향이 높은 입력변수`(Feature Importance)는 '재령일 > 시멘트양 > 물의양 > 슬래그양 > SP양 > 잔골재' 순`임.   
![](https://github.com/P-uyoung/AI-research/blob/master/Concrete/Fig/Feature%20Importance.png)   

<br/>
<!-- 
## **기술 및 도구**
  <span><img src="https://img.shields.io/badge/Python-05122A?style=flat-square&logo=python"/></span>
  <span><img src="https://img.shields.io/badge/Pytorch-EE4C2C?style=flat-square&logo=PyTorch&logoColor=white"></span>
  <span><img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=TensorFlow&logoColor=white"></span>
  <span><img src="https://img.shields.io/badge/TensorFlowLite-41454A?style=flat-square&logo=TensorFlowLite&logoColor=white"></span>
  <span><img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=Linux&logoColor=white"></span>
  
<br/>


