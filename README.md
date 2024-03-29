# Laser-Detection-Machine-Learning

<a name="readme-top"></a>
<p float="left">
  <img src="https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue">
  <img src="https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white">
  <img src="https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white">
  <img src="https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white">
  <img src="https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white">
  
</p>

<!-- ABOUT THE PROJECT -->
### About The Project
This machine learning project is a part of my Master's course `Machine Learning` to classify faulty and non-faulty lasers correctly.

### Problem Statement
For the purpose of quality assurance, a manufacturer of medical lasers wants to introduce a system which recognizes defective products. For the lasers produced, a constant lightoutput with a frequency as constant as possible is desired. Certain fluctuations are acceptable; Lasers in which the power fluctuates to an intolerable extent should be sorted out.For this purpose, the intensity of each laser is measured for one minute – one measurement per second.

### Implementation

* four classifiers: `Decision Tree`, `Random Forest`, `SVM(Support Vector Machine)`, `KNN (K Nearest Neighbor)`
* evaluation/permormance metrics: `accuracy`, `recall`, `precision`, `f1-score`, `confusion matrix`, `AUC`, `ROC curve`
* dataset: `laser.mat`

### Justify model's robustness
Following this steps to justify all model's robustness:
* Model training using default parameters
* Generating confusion matrix, classification report and ROC curve
* Applying GridSearchCv for finding best parameters
* Model training using best parameters
* Generating confusion matrix, classification report and ROC curve for comparing with the default parameters

### Conclusion
Among the 4 models, we did not get any improvement after hyper-parameter tuning on the two following models:
* SVM (98%)
* K-Nearest Neighbor (95%)

On the other hand, Following two models showed an improvement after hyper-parameter tuning:
* Decision Tree (from 80% to 90%)
* Random Forest (from 96% to 98%)

Therefore, Random Forest is outperforming all other models.


# Credit Card Default Prediction

<p align="right">(<a href="#readme-top">back to top</a>)</p>
Given data about credit card clients, we try to predict whether a given client will default or not.  

Logistic regression, support vector machine, and neural network models used to make our predictions.  

Data source: https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset
