# EEG Emotion Classifier

This project explores classification of emotional states (valence/arousal) from EEG signals using machine learning.

## 🧠 Dataset

[Kaggle EEG Emotion Dataset](https://www.kaggle.com/datasets/birdy654/eeg-brainwave-dataset-feeling-emotions)

## Project Summary

This notebook analyzes EEG data to classify emotional states using machine learning. The dataset contains over 2,500 frequency-domain features derived from brainwave activity recorded while subjects listened to emotion-evoking music.

### Key Steps

- Loaded and cleaned the dataset (removed missing values, renamed columns).
- Encoded emotion labels numerically using `LabelEncoder`.
- Split the data into training and test sets (80/20 split).
- Performed 5-fold cross-validation to estimate model generalizability.
- Trained a `RandomForestClassifier` on the full EEG feature set.
- Evaluated performance using accuracy, classification report, and confusion matrix.

### Conclusions

- The model achieved reasonable accuracy given the high-dimensional input space.
- Random Forest performed well without requiring much parameter tuning.
- Cross-validation scores confirmed stable performance across folds.
- The results suggest that EEG signals contain patterns that can be used to classify emotional states.
- Further improvements could include feature selection, dimensionality reduction (e.g., PCA), or trying alternative classifiers.

## 🗂️ Structure

- `/notebooks` – Colab/Jupyter notebooks
- `/data` – Link or instructions for dataset (do **not** upload raw EEG files)
- `/results` – Charts, model outputs, performance summaries
