# Machine Learning Course

This repository corresponds to the Machine Learning Course (IE675b) at the University of Mannheim.

## Assignment 1: MNIST Dataset

In this assignment, we use a preprocessed variant of the MNIST digits dataset to classify hand-written digits. The dataset comprises classes for each digit (0-9) with features representing scanned images (28×28 pixels, values in {0, 1, …, 255}). It contains approximately 6000 training images per class and 1000 test images per class. More details can be found at [MNIST Dataset](http://yann.lecun.com/exdb/mnist/).

The report focuses on the Naive Bayes classification algorithm, particularly the effects of Laplace smoothing. We trained and evaluated the model using standard metrics such as accuracy, precision, recall, and F1-score. Cross-validation determined the optimal smoothing parameter α, emphasizing its impact on model performance. We also generated digit samples to explore how α influences sample quality and discussed theoretical aspects like handling missing data. The findings highlight the importance of tuning α to balance overfitting and underfitting in classification tasks.

## Assignment 2: Spambase Dataset

This assignment involves a dataset on email spam detection, derived from 4601 emails labeled as no-spam (0) or spam (1). Each email has 57 features, including:

- **48 word features:** Indicating the frequency percentage of specific words in the email (e.g., “business,” “free,” “george”).
- **6 character features:** Reflecting the frequency percentage of certain characters in the email (e.g., `{[}!$#`).
- **3 length statistics features:** Analyzing consecutive uppercase letter lengths, including minimum, maximum, and total lengths.

The dataset is split into a training set (3065 examples) and a test set (1536 examples). We provide code to load the data and access all feature names. More information can be found at [Spambase Dataset](https://archive.ics.uci.edu/ml/datasets/spambase).

This report explores the implementation and evaluation of a logistic regression model utilizing gradient descent (GD) and stochastic gradient descent (SGD) optimization methods on a dataset of emails to classify spam. Through a series of tasks, we analyze feature distributions, assess model performance metrics, and investigate the effects of varying the regularization parameter $\lambda$ on model complexity and weight vector composition. Kernel density estimation (KDE) plots reveal significant patterns and outliers among features, while performance evaluations demonstrate the interplay between accuracy, precision, recall, and AUC scores. A comprehensive examination of weight vectors highlights the trade-offs associated with regularization, emphasizing the importance of selecting an appropriate $\lambda$ to achieve an optimal balance between model fit and generalization. Overall, the findings illustrate the effectiveness of logistic regression in spam classification and provide insights for refining feature selection and model tuning.