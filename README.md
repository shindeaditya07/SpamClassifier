Email Spam Classifier using Naive Bayes Theorem

The Naive Bayes Theorem operates on the principle of conditional probability. It assumes that the features (words or phrases in the case of emails) are independent of each other, which may not always hold true in reality but simplifies the computational complexity significantly. In the context of an email spam classifier, this theorem calculates the probability that a given email belongs to a particular class (spam or not spam) based on the occurrence of specific words or features within the email.

We use the following steps to implement the naive bayes theorem in python:
1. Import the numpy, pandas packages, import train_test_split from sklearn.model_selection, CountVectorizer from sklearn.feature_extraction.text, MultinomialNB from sklearn.naive_bayes.
2. Import presaved data using pd.read_csv() function.
3. Create a new column "Spam" whose values can be 0 for ham mails, 1 for spam mails.
4. Create train-test-split using train_test_split() function.
5. Find word count using CountVectorizer and store it in a matrix form. xtrain_count = cv.fit_transform(xtrain.values)
6. Train model using MultinomialNB() function.
7. Pre-test a user created ham and spam mail with the model using the cv.transform() function.
8. Find out the accuracy of the model by calculating the score using model.score() function.

The beauty of Naive Bayes lies in its simplicity, efficiency, and effectiveness. Despite its "naive" assumption of feature independence, it often outperforms more complex algorithms in spam classification tasks. This makes it a popular choice for real-time email filtering systems, where quick and accurate decisions are crucial to maintaining a secure and clutter-free inbox.
