# EEG Emotion Classifier

This project explores classification of emotional states (valence/arousal) from EEG signals using machine learning.

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

## Structure

- `/notebooks` – Colab/Jupyter notebooks
- `/data` – Not uploaded here - to find on Kaggle s below
- `/results` – Charts, model outputs, performance summaries

## Dataset Description and Citation

This project uses the **EEG Brainwave Emotion Dataset** available on [Kaggle](https://www.kaggle.com/datasets/birdy654/eeg-brainwave-dataset-feeling-emotions).

The dataset consists of EEG recordings from two individuals (1 male, 1 female) collected using a Muse headband, which records from TP9, AF7, AF8, and TP10 placements using dry electrodes. Data was collected for 3 minutes per emotional state (positive, neutral, negative), with an additional 6 minutes of resting (neutral) baseline. The EEG signals were preprocessed using a statistical extraction strategy described in the linked publications.

Citation sources as suggested:

- [Mental Emotional Sentiment Classification with an EEG-based Brain-machine Interface](https://www.researchgate.net/publication/329403546_Mental_Emotional_Sentiment_Classification_with_an_EEG-based_Brain-machine_Interface)
- [A Deep Evolutionary Approach to Bioinspired Classifier Optimisation for Brain-Machine Interaction](https://www.researchgate.net/publication/335173767_A_Deep_Evolutionary_Approach_to_Bioinspired_Classifier_Optimisation_for_Brain-Machine_Interaction)
