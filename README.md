# NLP Sentiment Analysis Engine

A comprehensive **Natural Language Processing (NLP)** project developed using **Python**, **NLTK**, and **Scikit-learn**. This project builds an end-to-end sentiment analysis pipeline that preprocesses text, extracts TF-IDF features, trains a Naive Bayes classifier, and predicts the sentiment of unseen product reviews.

---

## Project Overview

Sentiment analysis is one of the most common applications of Natural Language Processing (NLP). This project demonstrates a complete NLP workflow by cleaning text, performing linguistic preprocessing, converting text into numerical features, training a machine learning model, and predicting whether customer reviews express **positive** or **negative** sentiment.

The project is designed as a complete sentiment analysis engine suitable for educational purposes and introductory NLP applications.

---

## Project Objectives

* Build an end-to-end NLP pipeline.
* Clean and preprocess textual data.
* Preserve important negation words for sentiment analysis.
* Apply tokenization, stop-word removal, POS tagging, and lemmatization.
* Convert text into numerical vectors using TF-IDF.
* Train a Naive Bayes classifier.
* Predict sentiment for new customer reviews.
* Display prediction confidence scores.

---

## Repository Structure

```text
DecodeLabs_Project-4/
│
├── DecodeLabs_Project_4.ipynb
├── README.md
└── requirements.txt
```

---

## Technologies Used

* Python 3
* NLTK
* NumPy
* Scikit-learn

---

## Project Workflow

The project follows a complete NLP pipeline consisting of the following stages:

### 1. Text Preprocessing

The preprocessing pipeline includes:

* Text cleaning
* Lowercase conversion
* Tokenization
* Stop-word removal
* Preservation of negation words (e.g., *not*, *never*)
* Part-of-Speech (POS) tagging
* Word lemmatization

These steps improve text quality before feature extraction.

---

### 2. Dataset Preparation

The notebook contains a sample dataset of labeled product reviews.

Each review is assigned one of two sentiment labels:

* **Positive (1)**
* **Negative (0)**

This dataset is used to train and evaluate the sentiment classifier.

---

### 3. Feature Extraction

The project converts text into numerical features using **TF-IDF (Term Frequency–Inverse Document Frequency)**.

Features include:

* Unigrams
* Bigrams
* Sublinear TF weighting
* Vocabulary filtering using `min_df`

This representation captures important words and phrases for sentiment classification.

---

### 4. Model Training

A Naive Bayes classifier is trained on the processed data.

Depending on class balance, the project automatically selects:

* **Multinomial Naive Bayes** (for balanced datasets)
* **Complement Naive Bayes** (for imbalanced datasets)

This improves model robustness across different datasets.

---

### 5. Sentiment Prediction

The trained model predicts sentiment for new, unseen reviews and provides:

* Predicted sentiment
* Prediction probabilities
* Confidence scores

This demonstrates how the trained classifier can be applied to real-world customer feedback.

---

## Features

* Automated NLP preprocessing pipeline
* TF-IDF feature extraction
* POS-guided lemmatization
* Negation-aware preprocessing
* Automatic classifier selection
* Sentiment prediction with confidence scores
* Modular and reusable functions

---

## How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/AishaDataScientist/DecodeLabs_Project-4.git
```

### 2. Navigate to the Project Folder

```bash
cd DecodeLabs_Project-4
```

### 3. Install Required Libraries

```bash
pip install numpy nltk scikit-learn
```

Or install using:

```bash
pip install -r requirements.txt
```

### 4. Run the Notebook

Open and execute all cells in:

```text
DecodeLabs_Project_4.ipynb
```

---

## Required Libraries

```text
numpy
nltk
scikit-learn
```

---

## Learning Outcomes

This project demonstrates:

* Natural Language Processing (NLP)
* Text Cleaning
* Tokenization
* Stop-word Removal
* Part-of-Speech (POS) Tagging
* Lemmatization
* TF-IDF Vectorization
* Feature Engineering for Text
* Naive Bayes Classification
* Sentiment Analysis
* Machine Learning Workflow

---

## Future Improvements

* Train on larger real-world datasets.
* Support multi-class sentiment (Positive, Neutral, Negative).
* Add confusion matrix and classification report.
* Compare Naive Bayes with Logistic Regression and Support Vector Machines (SVM).
* Build a web application using Streamlit or Flask.
* Deploy the trained model using a REST API.

---

## Author

**Aisha Arif**

GitHub: https://github.com/AishaDataScientist

---
 If you found this project useful, consider giving it a star on GitHub!
