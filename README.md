# Text Mining with Naïve Bayes and Market Basket Analysis for Fake News Detection


This project integrates Naïve Bayes and Market Basket Analysis (MBA) to improve fake news detection by analyzing word associations.

1) Naïve Bayes for Text Preprocessing:

The text undergoes tokenization, stemming, lemmatization, and stop-word removal, ensuring that only meaningful terms are retained.
This step helps identify frequent and relevant words in both fake and real news articles.

2) Market Basket Analysis for Word Associations

The processed text data is structured into a transactional format, where each article represents a transaction and each word is treated as an item.
A sparse itemMatrix with 44,940 transactions (News) and 81,771 unique words (Items) is created for association rule mining.
The Apriori algorithm is applied to extract frequent itemsets and strong word associations based on support, confidence, and lift.
This approach helps uncover patterns in word co-occurrences, distinguishing linguistic features of fake and real news.


- **Fake News Dataset**: Contains fake news articles labeled as fake.
- **True News Dataset**: Contains true news articles labeled as true.
Fake and True News Dataset Sources: https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset
