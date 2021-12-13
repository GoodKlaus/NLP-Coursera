## 1. Stemming vs. Lemmatization
- A model without stemming/lemmatization can be the best
- Stemming can be done with heuristic rules
- Lemmatization needs more storage than stemming to work
- Lemmatization usually provides higher precision for query, comparing with stemming
- Stemming normally provides higher recall for query, comparing with lemmatization, because stemming is more likely to find all TPs

## 2. Bag-of-Words (N-gram) Features
- Sparse storage is preferred for bag-of-words features
- Classical bag-of-word vectorizer needs an amount of RAM at least proportional to T, which is the number of unique tokens in the dataset
- Applicable models: Logistic regression; Naive Bayes; SVM
