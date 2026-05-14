# News Classification using NLP & Deep Learning

## Overview

This project focuses on automatic news article classification using Natural Language Processing (NLP) and Deep Learning techniques. The system processes textual news data, performs preprocessing and feature extraction using TF-IDF Vectorization, and classifies news articles into predefined categories using a Neural Network model built with TensorFlow/Keras.

The project demonstrates a complete NLP pipeline including:

- Data preprocessing
- Text cleaning
- Feature engineering
- TF-IDF vectorization
- Multi-class classification
- Deep learning model training
- Model persistence and inference

---

# Problem Statement

With the rapid growth of digital media, manually organizing and categorizing news articles becomes inefficient and time-consuming.

This project aims to automate the classification of news articles into different categories using machine learning and deep learning techniques.

---

# Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
- SpaCy
- LangDetect
- Matplotlib
- Seaborn
- Jupyter Notebook

---

# Dataset Information

Dataset Used:
**News_Category_Dataset_v3.csv**

The dataset contains:

- News headlines
- Short descriptions
- News categories
- Additional metadata such as authors, links, and dates

A subset of the dataset was used for efficient model training and evaluation.

---

# Project Workflow

## 1. Data Loading
The dataset is loaded using Pandas.

## 2. Data Cleaning
Unnecessary columns were removed and missing values were handled.

## 3. Text Preprocessing
The preprocessing pipeline includes:

- Lowercasing
- URL removal
- Mention removal
- Special character removal
- Whitespace cleanup
- Language detection
- NLP processing using SpaCy

## 4. Feature Engineering
Text data is converted into numerical vectors using TF-IDF Vectorization.

## 5. Label Encoding
News categories are transformed into numerical labels using LabelEncoder.

## 6. Model Training
A Neural Network model is trained using TensorFlow/Keras for multi-class classification.

## 7. Prediction Pipeline
The trained model predicts the category of custom news text input.

---

# Deep Learning Model Architecture

The project uses a Sequential Neural Network architecture with:

- Dense layers
- ReLU activation
- Dropout layers for regularization
- Softmax output layer for classification

---

# Saved Models

The project includes:

- `news_classifier.keras` → Trained Neural Network model
- `tfidf_vectorizer.pkl` → TF-IDF Vectorizer
- `label_encoder.pkl` → Label Encoder

These files can be used directly for inference and deployment.

---

# Project Structure

```text
news-classification-nlp/
│
├── data/
│   └── News_Category_Dataset_v3.csv
│
├── notebooks/
│   └── news_classification_nlp.ipynb
│
├── models/
│   ├── news_classifier.keras
│   ├── tfidf_vectorizer.pkl
│   └── label_encoder.pkl
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

# Installation

## Clone Repository

```bash
git clone https://github.com/your-username/news-classification-nlp.git
```

## Navigate to Project Folder

```bash
cd news-classification-nlp
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Example Prediction

```python
sample_text = ["India wins the cricket world cup final"]

sample_tfidf = vectorizer.transform(sample_text).toarray()

prediction = model.predict(sample_tfidf)
```

The predicted category is decoded using the saved label encoder.

---

# Future Improvements

Potential enhancements include:

- Streamlit or Flask deployment
- Real-time news classification
- Transformer-based NLP models (BERT)
- Docker deployment
- Hyperparameter tuning
- Advanced NLP preprocessing

---

# Learning Outcomes

This project helped in understanding:

- Natural Language Processing
- Text preprocessing techniques
- TF-IDF Vectorization
- Deep Learning for NLP
- Multi-class classification
- TensorFlow/Keras workflows
- Model serialization and inference

---

# Conclusion

This project demonstrates how NLP and Deep Learning can be combined to automate news categorization efficiently. It showcases practical implementation of text preprocessing, feature engineering, neural network design, and predictive inference using real-world news data.