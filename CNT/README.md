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
- [Visualize Model](#Visualize-Model)
  - [a. ModelA](#a.-ModelA)
  - [b. ModelB](#b.-ModelB)
  
</b>
<br/>

## **Abstract**

![](https://github.com/P-uyoung/AI-research/blob/master/CNT/Fig/Overview.png)

- Although it is recognized as the next-generation new material for CNTs, there is no research on quality evaluation when used in construction materials.

- Optical microscope images of experimental samples are used as data.

- (1) Data Collections:  `binarize(greyscale)` the images and `augment` data

- (2) Data Pre-processing: `histogram stretching` to increase constant ratio(명암비)

- (3) Train Model: 1D-CNN with dual convolutional layers

- (4) Test Model: show confusion matrix

<br/>

## **Tech and Tools**
  <span><img src="https://img.shields.io/badge/Python-05122A?style=flat-square&logo=python"/></span>
  <span><img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=TensorFlow&logoColor=white"></span>
  <span><img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=Docker&logoColor=white"></span>
  <span><img src="https://img.shields.io/badge/REST%20API-05122A?style=flat-square"></span>
  
<br/>

## **Visualize Model**
<details>
<summary><b>Show detailed things</b></summary>
<div markdown="1">

### a. ModelA
**Whether or not dispersion processing module**
![](https://github.com/P-uyoung/AI-research/blob/master/CNT/Fig/module1.png)
![](https://github.com/P-uyoung/AI-research/blob/master/CNT/Fig/module1-1.png)
  
### b. ModelB
**Content of CNT: 0.05, 0.1, 0.2, 0.4 wt%**
![](https://github.com/P-uyoung/AI-research/blob/master/CNT/Fig/module2.png)
![](https://github.com/P-uyoung/AI-research/blob/master/CNT/Fig/module1-2.png)

</div>
</details>





