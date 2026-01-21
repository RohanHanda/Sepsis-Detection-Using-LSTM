# 🩺 Early Sepsis Risk Prediction using Deep Learning

## 📌 Overview
Early identification of high-risk patients is a critical challenge in healthcare due to noisy physiological signals, delayed labels, and extreme class imbalance.  
This project presents an **end-to-end deep learning pipeline** for **early disease risk prediction** using multivariate patient time-series data.

The system is designed as a **clinical decision-support prototype**, not a diagnostic tool, with a strong emphasis on:
- Temporal modeling
- Interpretability
- Clinically meaningful evaluation metrics
- Ethical AI practices

---

## 🚀 Key Features
- Bilateral LSTM-based temporal sequence modeling
- Attention mechanism for time-step interpretability
- Cost-sensitive learning for extreme class imbalance
- Precision–Recall–based threshold optimization
- Robust evaluation using PR-AUC and sensitivity–specificity trade-offs and custom metrics

---

## 🧠 Model Architecture
- Input: Multivariate patient time-series data
- Multiple Bilateral LSTM layers for temporal feature extraction
- Attention layer to highlight important time steps
- Fully connected output layer with sigmoid activation
- Optimized decision threshold selected using validation data

---

## 📊 Final Results (Test Set)

| Metric | Value |
|------|------|
| ROC-AUC | **0.995** |
| PR-AUC | **0.963** |
| Sensitivity (Recall) | **92.7%** |
| Specificity | **99.8%** |
| Precision (Positive class) | **92.3%** |
| F1-score (Positive class) | **92.5%** |
| Accuracy | **99.6%** |

### Confusion Matrix
- True Positives (TP): 3012  
- False Negatives (FN): 238  
- False Positives (FP): 251  
- True Negatives (TN): 125,436  

These results demonstrate strong early risk detection performance despite severe class imbalance.

---


## 📁 Repository Structure
Sepsis-Detection-using-LSTM/
│

├── dataset/ # Dataset

├── notebook/ # EDA, preprocessing, training, evaluation

├── model/ # Saved model

└── README.md

---

## 🧪 Technologies Used
- Python
- TensorFlow / Keras
- NumPy, Pandas
- Scikit-learn
- Matplotlib, Seaborn

---

## ⚠️ Ethical Considerations
- This system is **not intended for clinical diagnosis**
- Designed strictly for **decision support**
- Must be used with human oversight
- False positives and false negatives are explicitly analyzed

---

## 📌 Limitations
- Retrospective dataset
- Single-dataset evaluation
- Label noise inherent to clinical data
- Performance may vary across institutions

---

## 📜 Disclaimer
This project is for **educational and research purposes only** and must not be used for real-world clinical decision-making or patient care.

---

## 📬 Contact
If you have questions, feedback, or suggestions, feel free to open an issue or reach out via LinkedIn.
