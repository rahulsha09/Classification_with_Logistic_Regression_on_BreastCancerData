# Classification with Logistic Regression on Breast Cancer Wisconsin Dataset.

## Overview

Hey this is new repo on GitHub where working on Breast Cancer Wisconsin Dataset in which project builds a binary classifier to detect breast cancer (malignant vs benign) using logistic regression, Choose a binary classification dataset, Train/test split and standardize features, Fit a Logistic Regression model, Evaluate with confusion matrix, precision, recall, ROC-AUC and Tune threshold and explain sigmoid function.

## Approach

- Loads and inspects the provided dataset (`data.csv`)
- Encodes labels, splits data into train/test sets
- Scales features for model compatibility
- Trains a logistic regression model, evaluates with confusion matrix, precision, recall, ROC-AUC
- Visualizes ROC curve and sigmoid function
- Demonstrates threshold tuning and explains model theory

## Step-by-Step Explanation
1. Load and Preview Data
Reads the provided CSV.

Drops the 'id' column (not a feature for ML).

2. Encode Target
Converts diagnosis labels into binary: Malignant=1, Benign=0.

3. Split Features/Target
X: all columns except the target (diagnosis)

y: target column.

4. Train/Test Split
Uses stratify for class balance.

80/20 split for best utility/testing.

5. Standardization
Features scaled to mean=0, std=1 (required by LR for optimal results).

6. Train Logistic Regression
Fits model to training data.

7. Predict and Evaluate
Calculates predictions, probabilities for ROC.

Evaluation metrics: Confusion matrix, Precision, Recall, ROC-AUC.

8. Plot ROC Curve
Visualizes true/false positive tradeoff & ROC-AUC score.

9. Tune Threshold
Shows how a lower threshold (e.g. 0.3 instead of 0.5) can change precision/recall.

10. Sigmoid Function Plot
Demonstrates the core concept — mapping logit (raw model output) to probability.

## Files

- `Classification_with_Logistic_Regression_on_BreastCancer_Data.ipynb` — Complete code with stepwise comments
- `data.csv` — Dataset
- Plots: `roc_curve.png`, `sigmoid_curve.png`
- `Interview_QA.md` — Key Interview Questions & Answers
