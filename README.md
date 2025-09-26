# A Comparative Analysis of kNN and Decision Tree for Multi-Class Classification

This repository contains my CM3015 Machine Learning and Neural Networks midterm project, where I compare the performance of two supervised learning algorithms: k-Nearest Neighbors (kNN) and Decision Trees on the classic Wine dataset.

## Project Overview
This project is a comparative study of two classic machine learning algorithms: k-Nearest Neighbors (kNN) and Decision Trees, applied to a multi-class classification problem using the Wine dataset from scikit-learn.

The aim is to evaluate the performance, strengths, and weaknesses of both algorithms when applied to the same dataset, and to reflect on their suitability for multi-class classification tasks.

## Problem Statement
The project involved implementing at least two machine learning algorithms studied in the module, applying them to a dataset of choice, and comparing their performance. One of the algorithms had to be implemented from scratch in Python, while standard libraries could be used for the other.

In this project, I:  
- Implemented k-Nearest Neighbors (kNN) from scratch.  
- Applied a Decision Tree classifier using scikit-learn.  
- Compared their performance using evaluation metrics such as accuracy, precision, and cross-validation results.  

## Dataset
- Wine dataset (scikit-learn built-in).  
- 178 samples of wines produced by three cultivars in Italy.  
- 13 numerical features (for example, alcohol, flavanoids, magnesium, proline).  
- 3 target classes.  
- Challenges: small dataset size, correlated features, and presence of outliers.  

## Methodology
1. **Preprocessing**  
   - Outlier removal using IQR with an adjusted threshold of 1.2.  
   - Train-test split with an 80:20 ratio.  
   - Min-Max scaling for distance-based kNN.  
   - PCA to reduce correlated features.  

2. **Model Training**  
   - **kNN**: Implemented from scratch, with optimal k=3 found through cross-validation.  
   - **Decision Tree**: Trained with scikit-learn’s `DecisionTreeClassifier`, optimal max_depth=2.  

3. **Evaluation Metrics**  
   - Test Accuracy  
   - Cross-Validation Accuracy  
   - Precision (macro-average)  

## Results
- **kNN**  
  - Test Accuracy: 96.43%  
  - Cross-Validation Accuracy: 98.18%  
  - Precision: 96.97%  

- **Decision Tree**  
  - Test Accuracy: 89.29%  
  - Precision: 90.28%  
  - Cross-Validation Accuracy: 93.64%  

**Summary:** kNN achieved higher scores across all metrics, while Decision Trees offered greater interpretability but were more prone to overfitting.  

## Files in This Repository
- `knn_vs_decision_tree.html` – Jupyter Notebook exported as HTML (contains code, analysis, and visualizations).
- `knn_vs_decision_tree.ipynb` – Raw Jupyter Notebook for reproducibility and re-running the code.  
- `Report.pdf` – Formal write-up of the project, including background, methodology, results, and evaluation.  
- `README.md` – Project overview and instructions (this file).  

## How to Use
- Open `knn_vs_decision_tree.html` in a browser to view the complete analysis.  
- Read `Report.pdf` for the formal write-up with detailed methodology and discussion.
- Open `knn_vs_decision_tree.ipynb` in Jupyter or Colab to re-run or extend the code.  

## View Online
You can also view the rendered notebook directly through GitHub Pages here:  
👉 [kNN vs Decision Tree Notebook](https://ellenfaustine.github.io/knn-vs-decision-tree/knn_vs_decision_tree.html)
