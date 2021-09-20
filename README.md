# Finite Element Human Body Model-based Injury Prediction using Machine Learning
Repositry documenting the work for the master's thesis conducted by *[Yash Niranjan Poojary](https://github.com/yash-n-p) and [Akhil Srinivas](https://github.com/akhil8794)*. This thesis was completed in july 2021.

The contents and results of the thesis are published in [Chalmers ODR](https://odr.chalmers.se/handle/20.500.12380/303774).

Part of this project is also packaged in a python library available for public called [`dynakit`](https://pypi.org/project/dynakit/)

# Thesis abstract
Models of the human body, both physical and virtual, have been vital tools for the design of safer vehicles. Finite element models of the human body are now becoming widely used for evaluating safety systems. With the introduction of future designs like autonomous vehicles that affect the nature of vehicle crashes, HBM will become a necessary tool to assess safety. Detailed human anatomy representation in HBM, however, makes it computationally expensive and consumes a lot of time to simulate crash scenarios. The aim of this thesis was to evaluate machine learning models as computationally inexpensive surrogates for injury metrics from human body models. 

Machine learning was performed on outputs from two types of finite element models, crash test dummy (Hybrid III M50 fast model) and the human body (SAFER model). Different types of model outputs namely kinematics, kinetics, injury metrics, and injury risks used for injury evaluation were studied. Linear regression-based models (Ordinary, Lasso, Ridge) were used as the baseline models. Advanced tree-based methods (Random Forest, Gradient boosted, XGBoost, Histogram-based gradient boost) and Gaussian process regression were used to build additional machine learning models. The machine learning pipeline comprised of data preparation, model validation using the k-Fold cross-validation method, and model optimization using hyperparameter tuning methods such as random search and grid search. In these methods, the number of simulations required to achieve accurate models was evaluated.

This thesis provides representative model learning curves (model accuracy vs number of simulations) for the various HBM outputs. The accuracy of the models was seen to be highly dependent on data transformation if the HBM outputs were skewed. It was also seen that estimation of numerical noise needs to be considered as part of the ML pipeline for HBM data to avoid overfitting in the pursuit of accuracy. For the HBM outputs considered in this study, tree-based boosting methods provided accurate models in most cases.

## Machine learning algorithms used
<p align="center">
  <img src="https://github.com/yash-n-p/FE_HBM_ML/blob/main/docs/models.PNG" alt="Sublime's custom image"/>
</p>
