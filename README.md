# Grammar Scoring Engine – SHL Kaggle Competition

##  Objective
Built a machine learning model to predict grammar scores (0–5) from spoken English audio samples using MFCC features and regression modeling.

##  Tools & Libraries
- Python
- Librosa
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

##  Summary of Steps
- Extracted MFCC features from `.wav` audio files
- Trained a Random Forest Regressor on labeled grammar scores
- Evaluated model using RMSE and Pearson correlation
- Predicted scores for test set and created `submission.csv`
- Visualized predicted vs actual scores using scatter plots

##  Conclusion
Successfully developed a grammar scoring engine with strong training accuracy. The model processes audio input and predicts grammar proficiency effectively.

##  Project Files
- `train.csv`, `test.csv` – Audio file references and labels
- `grammar_scoring_engine.ipynb` – Feature extraction and model training code
- `submission.csv` – Final predictions file for Kaggle
