# Speaker Age Prediction from Speech 🎤📊

This project aims to estimate a speaker’s age based solely on speech characteristics. Leveraging acoustic and linguistic metadata extracted from controlled speech recordings, we built a regression pipeline to predict the speaker's age. The project was completed as part of the Data Science Lab Winter Call (A.Y. 2024/2025) at Politecnico di Torino.

## 🚀 Project Overview

- **Goal:** Predict speaker age using speech signal metadata and acoustic features.
- **Dataset Size:** 3,624 samples (2,933 for training, 691 for evaluation).
- **Features Used:** pitch (min/max/mean), jitter, shimmer, ZCR, tempo, energy, formants, and more.
- **Metric:** Root Mean Square Error (RMSE)

## 📁 Dataset Structure

The dataset contains:
- `development.csv`: 2,933 samples with features and target age.
- `evaluation.csv`: 691 samples for final predictions (no target).
- `audio_development/`: Audio files for training samples.
- `audio_evaluation/`: Audio files for testing samples.
- `sample_submission.csv`: Format reference for evaluation.

**Note:** External datasets or pre-trained models were strictly prohibited.

## 🛠️ Workflow

1. **Data Preprocessing**
   - Checked for nulls, outliers, and cleaned features.
   - Normalized features and handled categorical variables (e.g., gender, ethnicity).

2. **Feature Engineering**
   - Used both existing and derived acoustic features.
   - Ensured no data leakage between training and evaluation.

3. **Model Training**
   - Tried multiple regression models: Linear Regression, Random Forest, XGBoost.
   - Used cross-validation and hyperparameter tuning.
   - Selected the best model based on RMSE.

4. **Evaluation and Submission**
   - Generated predictions for the evaluation set.
   - Formatted CSV submission as per DSLE requirements.
   - Submitted using the student key on the DSLE platform.

## 📊 Results

- **Best RMSE:** _9.36_
- Successfully submitted results via the DSLE competition portal.


## 🧠 LLM Usage

Large Language Models (LLMs) such as ChatGPT were used **only** for generating the final project report and documentation. No LLM-generated code was used in the pipeline, in accordance with the project guidelines.

## 📬 Contact

For any queries related to this project, feel free to reach out via GitHub Issues or email (if public).

---


