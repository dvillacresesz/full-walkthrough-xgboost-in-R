### A full walkthrough (I hope) of XGBoost in R

As in my recent experience I didn't found a full tutorial, walkthrough or example of how to perform a step by step "personalized" XGBoost in R, I decided to upload this. Hope the code will be useful to someone.

What I mean by "personalized"? I mean that you could use any loss-function (evaluation metric, gain function...) to perform a fully parallelized Hyperparameter Tuning and then use XGBoost with those hyperparameters for whatever you want: prediction, feature selection, support for descriptive or causality analysis and so on. In `xgboost_tutorial_dv.R` I leave a tutorial to:

* Hyperparameter Tuning XGBoost using any evaluation metric you want with parallelized computation.
  * With some recommendations about the Hyperparameter Space 
* Optimal iteration for XGBoost (partially parallelized).
* Personalized Cross-Validation to be sure and to explore more about predicting power of the model (fully parallelized).
* Feature importance computation from where you can easily perform Feature Selection.
* Computation of an "interpretable model" from our XGBoost (thanks to [`AppliedDataSciencePartners/xgboostExplainer`](https://github.com/AppliedDataSciencePartners/xgboostExplainer)) 

Also I uploaded `Health Survey Ecuador - 2018 - as presented by publisher.rar`, databases you could use to reproduce my results if you want. Those are bases from the National Health Survey from Ecuador, survey conducted by the [National Statistical Office](https://www.ecuadorencifras.gob.ec/salud-salud-reproductiva-y-nutricion/).
