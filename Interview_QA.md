# Task 4 — Logistic Regression Interview Q&A

**1. How does logistic regression differ from linear regression?**  
- Linear regression predicts continuous values; logistic regression predicts probabilities for binary classification via sigmoid (values between 0 and 1).

**2. What is the sigmoid function?**  
- Maps logit (raw output) to [0,1] probability:  
  sigmoid(z) = 1 / (1 + exp(-z))

**3. What is precision vs recall?**  
- Precision = TP / (TP + FP) — risk of false alarms
- Recall = TP / (TP + FN) — ability to catch all positives

**4. What is the ROC-AUC curve?**  
- Graphs recall (TPR) vs. fall-out (FPR) for all thresholds.
- AUC summarizes the curve (higher=better).

**5. What is the confusion matrix?**  
- Table: TP, FP, TN, FN for model predictions vs truth — visualizes error types.

**6. What if classes are imbalanced?**  
- Metric distortion: accuracy misleading, model may always predict the majority.
- Use metrics like recall, precision, f1, ROC-AUC; possibly oversample/undersample/minority class weighting.

**7. How do you choose the threshold?**  
- By balancing recall/precision for application needs (ex: disease detection prefers high recall).

**8. Can logistic regression be used for multi-class problems?**  
- Yes, via extensions: one-vs-rest, multinomial logistic regression.

**End of Q&A**
