ENRON Email Spam Classifier
Project Overview

This project classifies emails as spam or ham (not spam) using a Decision Tree Classifier trained on the ENRON email dataset. The goal is to demonstrate email classification with natural language processing and machine learning.

Dataset

Source: ENRON Spam Dataset

Content: 6,744 emails labeled as spam or ham

Features: Email text content

Target: Label (0 = ham, 1 = spam)

Libraries

Python 3.13

NumPy, Pandas, scikit-learn, datasets

Model

Algorithm: Decision Tree Classifier (max_depth=10)

Text Representation: TF-IDF Vectorizer (unigrams & bigrams)

Results

Accuracy: 0.915

Classification Report:

Class	Precision	Recall	F1-score
HAM	0.98	0.84	0.91
SPAM	0.87	0.98	0.92

Confusion Matrix:

[[2796  513]
 [  57 3378]]

Sample Predictions
Email	Predicted Label
"Free money!!! Claim your prize now by clicking the link"	SPAM
"Hi team, please see the attached meeting agenda for tomorrow"	HAM
"URGENT! Your account has been suspended. Verify immediately"	SPAM
"Lunch at 1pm? Let me know if you're free"	HAM
Usage

Clone the repo:

git clone https://github.com/AshleyMamakoko/email-spam-classifier-enron.git


Install dependencies:

pip install -r requirements.txt


Run the notebook classifying_Emails.ipynb

Notes

Emails are stored as lists (e.g., ['Subject: ...']). TF-IDF converts lists to strings automatically.

Decision Tree text is truncated for readability.
