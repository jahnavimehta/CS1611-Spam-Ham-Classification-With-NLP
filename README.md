# Spam-Ham-Classification-With-NLP

## Table of contents

- [Project description](#project-description)
- [Tech stack](#tech-stack)
- [NLP text vectorization](#nlp-text-vectorization)
- [Dataset](#dataset)
- [Installation and usage](#installation-and-usage)

## Project description

In today’s digital age, SMS spam poses a significant challenge, flooding inboxes with unwanted messages. Overwhelming users with fraudulent and promotional messages posing security risks, such as phishing attempts and financial fraud. This project tackles the problem by leveraging NLP text vectorization techniques (BoW and TF-IDF) and ML models (Multinomial naive bayes or MultinomialNB) to classify SMS messages as spam or ham (legitimate).

## Tech stack

- Programming Language: Python  
- Libraries & Frameworks:
  1. NLTK - text processing.
  2. Pandas and NumPy - data manipulation and numerical computations.
  3. Regex (re) - pattern matching and text cleaning.
  4. Scikit-learn - dataset splitting, ML model, feature extraction (BoW, TF-IDF), and evaluation metrics.

## NLP text vectorization

  1. Bag of Words (BoW)
  - Represents text as a frequency-based numerical vector.
  - Counts the occurrences of each word in the document, ignoring order.
  - Creates a sparse matrix where each row is a document, and each column is a word.
  - Treats all words equally, which can lead to overemphasizing common words.
  - Suitable for simple text classification tasks but may struggle with semantic meaning.
  
  2. Term Frequency-Inverse Document Frequency (TF-IDF)
  - Assigns a weight to each word based on its importance in a document.
  - Term frequency (TF): measures how often a word appears in a document.
  - Inverse document frequency (IDF): reduces the importance of commonly occurring words across all documents.
  - Helps highlight important but unique words, making it better for distinguishing documents.
  - More effective than BoW in capturing meaningful terms and reducing the impact of stopwords.

BoW focuses on word count, while TF-IDF adjusts the importance of words based on how common they are across all documents.


## Dataset

- This dataset is the SMS Spam Collection, a well-known dataset used for spam detection research.
- It consists of labeled SMS messages, where:
  1. "ham" denotes legitimate messages.
  2. "spam" denotes unwanted or fraudulent messages.
- The dataset was originally collected by Tiago A. Almeida and José María Gómez Hidalgo and is commonly used for training spam classifiers.
- It is publicly available on platforms like Kaggle and the UCI Machine Learning Repository.


## Installation and usage

1. Clone the repository
  - `git clone [https://github.com/jahnavimehta/Spam-Ham-Classification-With-NLP.git](https://github.com/jahnavimehta/Spam-Ham-Classification-With-NLP.git)`
  - `cd  Spam-Ham-Classification-With-NLP`
2. Create a virtual environment and install dependencies.
  - `python -m venv venv`
  - `venv\Scripts\activate`
  - `pip install -r requirements.txt`
3. Execute the jupyter notebook.
