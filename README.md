I study machine learning for predicting structural materials, especially concrete and flyashes. This repository is about this code.

The first one is Fly ashes.
=================
This study develops into a three-step model.
* The first model is about "Prediction of Flyashes of Total Amorphous Content(wt. %)". 
  * Data
    * input(7) : XRF results (Al2O3, SiO2, CaO, Fe2O3, MgO, Na2O+0.658K2O, SiO2/Al2O3
    * output(1) : Total Amorphous Content 
  * Model
    * MLPReressor : solver-lbfgs, activation-relu, hidden_layer_sizes=(10,3)
    * Mini-batch gradient descent 
  * Result
    * (Accuracy) R-square : 0.674
    * This model is over-fitting. 


* The second model is about "Prediction of **_Domestic_** Flyashes of Total Amorphous Content(wt. %)". 






* The third model is about "Prediction of Domestic Flyashes of RAl2O3, RSiO2 Content(wt. %)."

The second one is Concrete.
===================
