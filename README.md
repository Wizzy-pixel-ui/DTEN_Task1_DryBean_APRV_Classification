# DTEN Task 1: Dry Bean Classification with APRV

This project was developed as part of the **Daryl Tech & Educational Network AI and Machine Learning Internship**.

The project focuses on classifying seven varieties of dry beans using morphological and geometric features from the [Kaggle Dry Bean Dataset](https://www.kaggle.com/datasets/muratkokludataset/dry-bean-dataset).

## Project overview

A project-specific classification algorithm called **Adaptive Prototype–Residual Voting (APRV)** was developed. APRV combines robust median and interquartile-range preprocessing, class-based prototypes, feature-reliability weighting, residual-distance analysis, adaptive local voting, class-prior correction, and explainable prediction analysis.

The model is evaluated using accuracy, precision, recall, F1-score, and a confusion matrix.

## Dataset

The dataset contains numerical features describing the shape and morphology of dry beans. The target variable represents seven bean varieties:

- Seker
- Barbunya
- Bombay
- Cali
- Dermosan
- Horoz
- Sira

Dataset source: [Kaggle Dry Bean Dataset](https://www.kaggle.com/datasets/muratkokludataset/dry-bean-dataset)

## Algorithm

APRV uses the following workflow:

1. Robustly scale numerical features using the training median and interquartile range.
2. Build one median prototype for each bean variety.
3. Estimate feature reliability from class separation and within-class stability.
4. Calculate weighted residual distances between new observations and class prototypes.
5. Add an adaptive local vote from nearby training observations.
6. Reduce local-vote influence for isolated observations.
7. Apply a small class-prior correction.
8. Produce an explainable class prediction.

APRV is presented as an original project-specific heuristic design. It is not claimed to be a completely unprecedented research algorithm.

## Tools and technologies

- Python
- Google Colab
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- KaggleHub

## How to run

1. Open the notebook in Google Colab.
2. Run the cells from top to bottom.
3. Allow the notebook to download the Kaggle dataset.
4. Review the accuracy, precision, recall, macro-F1 score, classification report, and confusion matrix.
5. Download the generated CSV evaluation files if needed.

## Repository contents

- `Wisdom_Kekeli_APRV_Task.ipynb` — complete Google Colab notebook.
- `README.md` — project overview, methodology, dataset source, and run instructions.

## Internship task

This repository fulfills **Task 1: Classification Model on a Standard Dataset** from the Daryl Tech & Educational Network AI and Machine Learning internship. The task requires dataset selection, preprocessing, model training, evaluation with accuracy, precision, recall, and a confusion matrix, followed by a short explanation of the model and results.

## Author

Wisdom Kekeli

## Internship organization

Daryl Tech & Educational Network
