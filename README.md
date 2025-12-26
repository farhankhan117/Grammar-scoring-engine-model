# 🗣️ Grammar Scoring Engine – SHL Kaggle Competition

## 🎯 Objective
Developed a **machine learning–based grammar scoring engine** to predict grammar proficiency scores (0–5) from spoken English audio samples using **MFCC feature extraction** and **regression modeling**.

---

## 🧠 Problem Statement
Manual evaluation of spoken grammar proficiency is time-consuming and subjective.  
This project aims to **automate grammar scoring** by analyzing speech audio and predicting grammar scores accurately using machine learning techniques.

---

## 🛠 Tools & Libraries
- Python
- Librosa
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

---

## 🔍 Methodology
### 1. Data Preparation
- Audio samples provided in `.wav` format
- Training and testing data referenced via CSV files

### 2. Feature Extraction
- Extracted **MFCC (Mel-Frequency Cepstral Coefficients)** from each audio file
- Aggregated MFCC statistics (mean, variance) for model input

### 3. Model Training
- Trained a **Random Forest Regressor** on labeled grammar scores
- Tuned model parameters for better performance

### 4. Model Evaluation
- Evaluated performance using:
  - **RMSE (Root Mean Squared Error)**
  - **Pearson Correlation Coefficient**

### 5. Prediction & Submission
- Generated grammar score predictions for test samples
- Created final `submission.csv` file for Kaggle submission

---

## 📊 Results & Visualization
- Achieved strong training performance
- Visualized **actual vs predicted grammar scores** using scatter plots
- Observed a positive correlation between predictions and true labels

---

## ✅ Conclusion
Successfully built a **grammar scoring engine** capable of processing spoken English audio and predicting grammar proficiency scores effectively.  
This solution demonstrates the potential of **audio feature extraction and regression models** for automated language assessment tasks.

---

## 📁 Project Files
- `train.csv` – Training audio references and labels  
- `test.csv` – Test audio references  
- `grammar_scoring_engine.ipynb` – Feature extraction and model training  
- `submission.csv` – Final predictions for Kaggle  

---

## 🚀 Future Improvements
- Experiment with deep learning models (CNN/LSTM on spectrograms)
- Use additional audio features (Chroma, Spectral Contrast)
- Apply cross-validation for robustness
- Fine-tune hyperparameters




---
