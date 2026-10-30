# Research Proposal

## Title

Machine Learning-Based Breast Cancer Classification Using Logistic Regression

## 1\. Background

Breast cancer diagnosis can involve examining characteristics of cells obtained from a breast mass. The Breast Cancer Wisconsin (Diagnostic) dataset contains numerical measurements calculated from digitised fine-needle aspirate images. These measurements provide an opportunity to study a supervised machine learning classification method using a public dataset.

## 2\. Research question

How accurately can Logistic Regression classify breast tumours as malignant or benign using diagnostic measurements?

## 3\. Aim and objectives

**Aim:** To develop and evaluate a Logistic Regression model for classifying records in the Breast Cancer Wisconsin (Diagnostic) dataset.

**Objectives:**

1. Explore the dataset and its 30 numerical predictor features.
2. Prepare the data and divide it into training and testing sets.
3. Train a Logistic Regression classifier using standardised features.
4. Evaluate its performance using accuracy, precision, recall, F1-score, a confusion matrix and ROC-AUC.

## 4\. Dataset and source

The project will use the Breast Cancer Wisconsin (Diagnostic) dataset from the UCI Machine Learning Repository: https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic

The dataset contains 569 observations and 30 continuous predictor features. The target variable identifies each record as malignant or benign. The features describe characteristics of cell nuclei measured from digitised fine-needle aspirate images. The notebook will load the dataset using `sklearn.datasets.load\\\_breast\\\_cancer`, which provides a convenient copy of this established dataset.

## 5\. Proposed method

This is a supervised binary classification task. The data will be divided into training and testing subsets using a stratified split so that both subsets retain a similar class distribution. A pipeline will standardise the numerical features and fit a Logistic Regression classifier. The pipeline ensures that scaling parameters are learned from the training data only. Model performance will be assessed on the held-out test set using accuracy, precision, recall, F1-score, a confusion matrix and ROC-AUC. Results will be interpreted as a classroom exercise rather than evidence of clinical usefulness.

## 6\. Two-source scan of existing work

### Source 1: Critical Risk Assessment, Diagnosis, and Survival Analysis of Breast Cancer (2024)

This study examines breast cancer risk assessment and classification approaches, including Logistic Regression, using the Wisconsin diagnostic dataset. Its reported results provide a useful point of comparison for evaluating a Logistic Regression model. The study also illustrates why classification performance should be assessed using more than accuracy alone, including sensitivity and specificity.

Link: https://pmc.ncbi.nlm.nih.gov/articles/PMC11119540/

### Source 2: Chetry et al. (2025)

The study, *Early Detection and Analysis of Accurate Breast Cancer for Improved Diagnosis Using Deep Supervised Learning for Enhanced Patient Outcomes*, compares several machine learning approaches, including Logistic Regression, on breast cancer datasets. It provides recent context for the use of conventional machine learning alongside more complex methods. This project is narrower: it focuses on one interpretable baseline classifier and one diagnostic dataset.

Link: https://doi.org/10.7717/peerj-cs.2784

## 7\. Expected outcome

The expected outcome is a trained Logistic Regression model and a transparent evaluation of its classification performance on held-out data. The project will identify strengths and limitations using several evaluation metrics. No particular accuracy level is assumed in advance.

## References

* UCI Machine Learning Repository. (n.d.). *Breast Cancer Wisconsin (Diagnostic).* https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic
* *Critical Risk Assessment, Diagnosis, and Survival Analysis of Breast Cancer.* (2024). https://pmc.ncbi.nlm.nih.gov/articles/PMC11119540/
* Chetry, M., et al. (2025). *Early detection and analysis of accurate breast cancer for improved diagnosis using deep supervised learning for enhanced patient outcomes.* PeerJ Computer Science. https://doi.org/10.7717/peerj-cs.2784

The project will use a training and testing split to evaluate the classification model. Model performance will be assessed using accuracy, precision, recall, F1-score, and a confusion matrix.

