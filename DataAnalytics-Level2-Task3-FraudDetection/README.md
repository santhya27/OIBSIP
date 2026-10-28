# 🛡️ FraudShield — Credit Card Fraud Detection

## Project Overview
FraudShield is a machine learning project designed to identify fraudulent credit card transactions in a highly imbalanced dataset.

**Internship Task:** Level 2 — Task 3  
**Domain:** Data Analytics and Machine Learning

## Objectives
- Analyze fraud and legitimate transaction distributions.
- Explore transaction amounts and elapsed-time patterns.
- Address class imbalance using SMOTE.
- Train and compare Logistic Regression and Decision Tree models.
- Evaluate precision, recall, F1-score, ROC-AUC, and Average Precision.
- Visualize model performance and feature importance.
- Discuss scalability for real-time fraud detection.

## Technologies
- Python
- NumPy
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Python CSV module
- JupyterLab
- SVG visualizations

## Dataset
The project uses the Credit Card Fraud Detection dataset from Kaggle.

Dataset link: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

Download `creditcard.csv` and place it in the `data/` folder before running the notebook. The dataset is not included in this repository.

## Project Structure
- `Fraud_Detection.ipynb` — analysis, training, and evaluation
- `data/README.md` — dataset download instructions
- `outputs/` — generated charts and evaluation results
- `requirements.txt` — Python dependencies

## Models
1. Logistic Regression
2. Decision Tree Classifier

SMOTE is applied only to the training data to avoid test-set leakage.

## Evaluation
The models are compared using precision, recall, F1-score, ROC-AUC, and Average Precision. Accuracy alone is not sufficient for an imbalanced fraud detection problem.

## Limitations
The dataset's `Time` feature represents elapsed seconds, not actual clock time. Its V1–V28 features are anonymized PCA components. Production deployment would require additional testing, monitoring, and throughput validation.

## How to Run
1. Download the dataset from Kaggle.
2. Place `creditcard.csv` in `data/`.
3. Install the dependencies listed in `requirements.txt`.
4. Open `Fraud_Detection.ipynb` in JupyterLab.
5. Run the notebook cells in order.

## Outputs
The notebook generates SVG charts and CSV files for model comparison, predictions, and feature importance.

*Created as part of the OIBSIP Data Analytics internship tasks.*
