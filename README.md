# 🏃‍♂️ Human Activity Recognition Using LSTM Networks

This project focuses on classifying human physical activities (e.g., walking, sitting, climbing stairs) using sensor data from smartphones. We built and compared two LSTM-based neural network models — one trained on engineered features, the other trained directly on raw sensor signals.

---

## 📘 Project Description

Human Activity Recognition (HAR) is crucial in AI, healthcare, and wearable tech. This project explores time-series classification using Recurrent Neural Networks (RNNs), specifically **Long Short-Term Memory (LSTM)** architectures, to process smartphone accelerometer and gyroscope data.

---

## 📊 Dataset

**Source:** [UCI HAR Dataset](https://archive.ics.uci.edu/ml/datasets/human+activity+recognition+using+smartphones)

- **561 Engineered Features:** (`X_train.txt`) – statistical, frequency, and time-domain features.
- **Raw Inertial Signals:** (`Inertial Signals/`) – direct sensor readings across 9 channels and 128 time steps.

---

## 🧠 Models

| Model | Input Type           | Description                                          |
|-------|----------------------|------------------------------------------------------|
| 1     | Extracted Features   | Trained on 561 preprocessed statistical features     |
| 2     | Raw Signals          | Trained on raw accelerometer & gyroscope sequences   |

### Shared Architecture:
- 2-layer **Stacked LSTM**
- **Dropout**: 30%
- **Loss**: Categorical Cross-Entropy
- **Optimizer**: Adam (lr=0.001)

---

## 📈 Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

## 📂 How to Run

1. **Download and unzip** the [UCI HAR Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/00240/UCI%20HAR%20Dataset.zip)
2. Open the notebook:
   - `proj2_YoussefSaraya_320210002.ipynb`
3. Run all cells to:
   - Preprocess and load data
   - Train both LSTM models
   - Evaluate and compare performance

---

## 🔍 Results & Insights

- Model 1 (Extracted Features) slightly outperforms Model 2 in accuracy and F1-Score.
- Model 2 (Raw Signals) performs competitively and is more realistic for real-time applications.
- Future improvements: try hybrid **CNN-LSTM** architectures or **attention mechanisms**.

---

## 💻 Technologies Used

- Python
- TensorFlow / Keras
- NumPy / Pandas
- Matplotlib / Seaborn
- Scikit-learn

---

## 👤 Author

- **Youssef Saraya** 

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 📦 Acknowledgements

- UCI Machine Learning Repository
- TensorFlow/Keras community
