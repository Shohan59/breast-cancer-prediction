# Breast Cancer Prediction
## Project overview
This project uses Logistic Regression to classify breast tumour records as malignant or benign using the Breast Cancer Wisconsin (Diagnostic) dataset.

## Research question
How accurately can Logistic Regression classify breast tumours as malignant or benign using diagnostic measurements?

## Dataset
- **Name:** Breast Cancer Wisconsin (Diagnostic)
- **Source:** UCI Machine Learning Repository
- **Dataset page:** https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic
- **Observations:** 569
- **Predictor features:** 30 numerical measurements
- **Target:** Diagnosis (malignant or benign)

The notebook loads the dataset through scikit-learn's built-in copy of the UCI dataset. The original dataset description explains that features are computed from digitised fine-needle aspirate images of breast masses.

## Method
1. Load and inspect the dataset.
2. Split the data into training and testing sets using stratification.
3. Standardise features within a scikit-learn pipeline to avoid data leakage.
4. Train a Logistic Regression classifier.
5. Evaluate the model using accuracy, precision, recall, F1-score, a confusion matrix and ROC-AUC.

## Run the project
Open `notebooks/breast_cancer_prediction.ipynb` in Google Colab and select **Runtime → Run all**. Keep the outputs visible, then save/download the completed notebook into this repository.

## Repository structure
```text
.
├── README.md
├── .gitignore
├── proposal.md
├── CONFLICT_NOTES.md
├── data/
│   └── README.md
└── notebooks/
    └── breast_cancer_prediction.ipynb
```

## Important limitation
This is an educational machine learning exercise using a historical public dataset. It is not a clinical diagnostic tool and must not be used to make medical decisions.

## References
- UCI Machine Learning Repository. Breast Cancer Wisconsin (Diagnostic). https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic
- Critical Risk Assessment, Diagnosis, and Survival Analysis of Breast Cancer (2024). https://pmc.ncbi.nlm.nih.gov/articles/PMC11119540/
- Chetry, M. et al. (2025). Early detection and analysis of accurate breast cancer for improved diagnosis using deep supervised learning for enhanced patient outcomes. https://doi.org/10.7717/peerj-cs.2784
