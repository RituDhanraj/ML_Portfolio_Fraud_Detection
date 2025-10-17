# ML_Portfolio_Fraud_Detection
## Non-technical summary (≈100 words)

This project detects potentially fraudulent card transactions. We trained a machine-learning model on an anonymised public dataset and tuned it to balance “catching fraud” with “avoiding false alarms.” The model first explores patterns in the data, then learns to rank transactions by risk. On our test set it achieved strong ranking performance (ROC-AUC 0.974; PR-AUC 0.756). Because teams act on alerts, we chose a practical decision threshold (0.82) to reduce false positives while keeping a high catch rate (Precision ≈ 0.50, Recall ≈ 0.83). Results, documentation, and how to reproduce them are provided so others can review and reuse this work.

## Results

**Dataset:** Kaggle — Credit Card Fraud Detection  
**Model:** Random Forest (tuned with Bayesian Optimization)

- ROC–AUC: **0.9738**
- PR–AUC: **0.7557**
- Operating threshold: **0.82**
  - Precision **0.503**, Recall **0.827**, F1 **0.626**
  - Confusion matrix: TN=56,784, FP=80, FN=17, TP=81

**Why this threshold?** Highest recall subject to **precision ≥ 0.50** to cut false-positive reviews while catching most fraud.

📄 Artifact: `models/fraud_rf_artifact.json` (best params + threshold)  
📈 PR curve: [docs/pr_curve.png](docs/pr_curve.png)  
👀 View notebook (nbviewer): https://nbviewer.org/github/RituDhanraj/ML_Portfolio_Fraud_Detection/blob/main/notebooks/04_results_and_visualizations.ipynb

“Add Results section with metrics & links”
Add PR curve image, artifact JSON, and README results
