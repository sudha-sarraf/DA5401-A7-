### Name: Sudha Sarraf
### Roll Number: ns25z247
# DA5401 – Assignment 7: Model Selection and Evaluation

### Overview
This assignment explores **multi-class model selection** using the UCI **Statlog (Landsat Satellite)** dataset.  
It involves loading and preprocessing the dataset, training multiple classifiers, and evaluating them using diverse performance metrics and visualization techniques.

### Contents
- **Part A – Data Preparation and Baseline:**  
  Load `sat.trn` and `sat.tst`, standardize features, train six classifiers  
  (KNN, Decision Tree, Dummy, Logistic Regression, GaussianNB, SVC),  
  and evaluate with Accuracy and Weighted F1-Score.

- **Part B – ROC Analysis:**  
  Compute One-vs-Rest ROC curves, calculate **macro-averaged AUC**, and plot combined ROC curves.

- **Part C – Precision–Recall Analysis:**  
  Generate **macro-averaged PRC curves**, compute **Average Precision (AP)**,  
  and interpret PRC results for the best and worst models.

- **Part D – Final Recommendation:**  
  Compare rankings based on F1, ROC-AUC, and PRC-AP, discuss trade-offs,  
  and recommend the best overall model.

- **Additional Experiments:**  
  Include **RandomForest** and **XGBoost** models for extended analysis  
  and demonstrate a classifier with **AUC < 0.5** for conceptual understanding.

### Recommended Environment
- Python 3.8+  
- Libraries: `numpy`, `pandas`, `scikit-learn`, `matplotlib`, `xgboost`, `joblib`

### How to Run
1. Place `sat.trn` and `sat.tst` in the same directory as the notebook.  
2. Open `DA5401_A7_Model_Selection.ipynb` in Jupyter.  
3. Run all cells in order (Parts A–D).  
4. Review generated plots and summary tables for interpretation.

### Final Recommendation
**Support Vector Classifier (SVC)** achieved the best balance across all metrics,  
demonstrating strong discrimination, precision–recall trade-off, and robustness.  
**XGBoost** slightly improved AUC/AP but at higher computational cost.

