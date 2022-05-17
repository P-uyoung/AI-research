I study machine learning for predicting structural materials, especially concrete and flyashes(; the component of concrete). This repository is about this code.

The first one is Fly ashes.
=================
This study develops into a three-step model.
* The first model is about "Prediction of Amorphous Aluminosilicate of Grobal Fly ashes(wt.%)". 
  * Data
    * input(6) : XRF results (Al2O3, SiO2, CaO, Fe2O3, MgO, Na2O+0.658K2O)
    * output(1) : QXRD results (Sum of amorphous aluminosilicate)
  * Model
    * Sampling : Stratified Sampling
    * (alg) MLPRegressor : solver-lbfgs, activation-relu, hidden_layer_sizes=(10,3)
    * Mini-batch gradient descent 
  * Result
    * (Accuracy) R-square : 0.774
    * ---This model is over-fitting.---


* The second model is about "Prediction of Amorphous Aluminosilicate of **_Domestic_** Fly ashes(wt.%)". 
  * Data
    * input(6) : XRF results (Al2O3, SiO2, CaO, Fe2O3, MgO, Na2O+0.658K2O)
    * output(1) : QXRD results (Sum of amorphous aluminosilicate)
  * Model
    * Sampling : Stratified Sampling
    * (alg) Ensemble Technique : GradientBoosing + RandomForest
  * Result
    * (Accuracy) R-square : 0.492
    * --- Accuracy is bad, some of fly ashes are not predictable. So, next model is trained without these fly ash samples. ---
    

* The third model is about "Prediction of Amorphous Aluminosilicate of **_Selected Domestic_**  Fly ashes(wt.%)."
  * Data
    * input(6) : XRF results (Al2O3, SiO2, CaO, Fe2O3, MgO, Na2O+0.658K2O)
    * output(1) : QXRD results (Sum of amorphous aluminosilicate)
  * Model
    * Sampling : Stratified Sampling
    * (alg) GradientBoosing : warm_start=True, learning_rate=1, n_estimator=8
  * Result
    * (Accuracy) R-square : 0.802
    * --- Accuracy is bad, some of fly ashes are not predictable. So, next model is trained without these fly ash samples. ---




The second one is Concrete.
===================
