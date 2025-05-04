# Grammar-scoring-engine-model
 Objective
The goal of this project is to develop a Grammar Scoring Engine that evaluates spoken English audio samples and assigns a grammar score ranging from 0 to 5 based on the MOS Likert scale. The model is trained to predict these continuous scores by learning from labeled audio data.

📁 Dataset Description
The dataset includes audio files in .wav format and three CSV files:

train.csv: Contains filenames and corresponding grammar scores.

test.csv: Contains filenames without labels (used for predictions).

sample_submission.csv: Template for valid submission format.

Training samples: 444

Testing samples: 195

Audio length: 45–60 seconds each

📊 Grammar Score Rubric
Score	Description
1	Poor grammar, frequent errors, limited sentence structure
2	Simple sentences, consistent grammatical mistakes
3	Decent grammar, some syntax or structure errors
4	Good control, few minor grammar issues
5	Strong grammar, rarely makes errors, uses complex structures

🧠 Approach
Audio Preprocessing

Extracted MFCC (Mel-frequency cepstral coefficients) features from each audio file using Librosa.

Applied mean pooling to convert variable-length audio into fixed-size feature vectors.

Model Training

Used a Random Forest Regressor to predict grammar scores.

Trained on MFCC features with corresponding labels from train.csv.

Evaluation Metrics

Calculated Root Mean Squared Error (RMSE) on training data.

Computed Pearson Correlation to assess model consistency.

Prediction & Submission

Extracted features from test-audio/ and predicted scores.

Created a valid submission.csv file for evaluation.

Visualization

Used scatter plot to compare predicted vs true grammar scores on training data.

✅ Results
Train RMSE: (value printed in notebook)

Pearson Correlation: (value printed in notebook)

A submission.csv file is generated in the correct format.

📦 Requirements
Python

pandas

numpy

librosa

scikit-learn

matplotlib

seaborn

tqdm
