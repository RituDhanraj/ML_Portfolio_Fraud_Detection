# ML_Portfolio_Fraud_Detection
## Non-technical summary (≈100 words)

This project detects potentially fraudulent card transactions. We trained a machine-learning model on an anonymised public dataset and tuned it to balance “catching fraud” with “avoiding false alarms.” The model first explores patterns in the data, then learns to rank transactions by risk. On our test set it achieved strong ranking performance (ROC-AUC 0.974; PR-AUC 0.756). Because teams act on alerts, we chose a practical decision threshold (0.82) to reduce false positives while keeping a high catch rate (Precision ≈ 0.50, Recall ≈ 0.83). Results, documentation, and how to reproduce them are provided so others can review and reuse this work.

