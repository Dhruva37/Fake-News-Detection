# Fake-News-Detection #
Fake News Detection system using NLP and Machine Learning with TF-IDF and Logistic Regression.

## Overview
This project implements a Fake News Detection system using Natural Language Processing (NLP) and Machine Learning techniques in Python. The goal is to classify news statements as **Real** or **Fake** based on textual patterns learned from data.

## Dataset
The dataset used in this project is derived from the **LIAR benchmark dataset**, which contains labeled political and public statements. The original multi-class labels were converted into binary classes for simplicity:
- True → Real News
- False → Fake News

The dataset is split into training, testing, and validation sets.

## Approach
- Performed text preprocessing including cleaning, lowercasing, stopword removal, and lemmatization  
- Extracted textual features using **TF-IDF vectorization with n-grams**  
- Trained a **Logistic Regression** classifier for binary classification  
- Evaluated the model using **Accuracy, F1-score, Confusion Matrix, and K-Fold Cross Validation**

## Results
The model achieved an F1-score of approximately **0.70**, demonstrating reasonable performance for a classical NLP-based fake news detection system.

## Features
- End-to-end NLP pipeline  
- Binary classification (Real / Fake)  
- Supports custom text input for prediction  
- Clear evaluation and performance analysis  

## Limitations
- The model is pattern-based and does not verify real-world facts  
- Some true statements may be misclassified due to dataset bias  
- Performance depends on the quality and size of training data  

## Future Improvements
- Use deep learning models such as LSTM or BERT  
- Incorporate source credibility and metadata  
- Expand training data for improved accuracy  

## Technologies Used
- Python  
- Pandas, NumPy  
- Scikit-learn  
- NLTK  
