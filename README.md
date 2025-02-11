# Text Mining with Naïve Bayes and Market Basket Analysis for Fake News Detection


# Fake News Detection Using Naïve Bayes and Market Basket Analysis

This project integrates **Naïve Bayes** and **Market Basket Analysis (MBA)** to improve fake news detection by analyzing word associations.

## Naïve Bayes for Text Preprocessing
The text undergoes the following preprocessing steps:
- **Tokenization**: Breaking text into individual terms.
- **Stemming & Lemmatization**: Reducing words to their root forms.
- **Stop-word Removal**: Removing common, unimportant words.

These steps ensure that only meaningful terms are retained, helping to identify frequent and relevant words in both fake and real news.

## Market Basket Analysis for Word Associations
The processed text data is structured into a **transactional format**, where:
- Each News represents a **transaction**.
- Each word is treated as an **item**.

A sparse **itemMatrix** is created with:
- 44,940 transactions (News)
- 81,771 unique words (Items)

The **Apriori algorithm** is applied to extract frequent itemsets and strong word associations based on support, confidence, and lift. This approach uncovers patterns in word co-occurrences, helping to distinguish linguistic features of fake and real news.



- **Fake News Dataset**: Contains fake news articles labeled as fake.
- **True News Dataset**: Contains true news articles labeled as true.
Fake and True News Dataset Sources: https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset
