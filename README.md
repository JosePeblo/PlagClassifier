# PlagClassifier

**PlagClassifier** is a machine learning-based plagiarism detection tool for Java source code. It leverages BERT to generate sequence embeddings, enabling the model to assess code similarity effectively.

---

## Overview

This repository demonstrates the data preparation, model training, and evaluation process for a Java code plagiarism classifier. The model is designed to identify pairs of code files that are either plagiarized or original.

## Datasets

We used a combination of the **ConPlag v2** and **IR Plag** datasets for training and evaluation. Details on how the datasets were pre-processed and merged can be found in:

- `src/DataPreparation.ipynb`

## Model Architecture

The model is a binary classifier that uses dense layers fed with embeddings of two code sequences. These embeddings are generated using a pre-trained BERT model.

Training achieved an accuracy of **82.9%** on the validation set.

You can find the full model training workflow in:

- `src/Bert.ipynb`

