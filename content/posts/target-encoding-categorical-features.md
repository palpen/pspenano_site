---
title: "Target Encoding Categorical Features"
date: 2020-01-25T11:50:01-05:00
draft: false
---

## What is target encoding?
Replace categorical value with the mean of the target among all records with the given category

## When to use target encoding?
In cases when the cardinality of a categorical feature is huge and one-hot is infeasible or when label encoding is inappropriate

## What type of categorical features does it apply to?
* ordinal, nominal, binary

## What are the issues with target encoding?
* Can cause overfitting when distribution of target among cateogiries in training set is different from test set (how ???)

## Intuition for K-fold CV target encoding
Taking mean of target for category value that have very few records may result in biased estimates in the distribution of the target. If the category is say 'cat', but there are only 5 records associated with that category, then the mean of the target may not represent the true distribution of cat in the test set. To avoid this, instead of taking the mean of the target across all the records in the training dataset for each cateogory, take the mean of the target for each cateogry value only on the k-1 folds and use the mean for that target on the kth fold. This introduces some noise in the target encoding, reducing the chance of overfitting.

Without k-fold CV, a given value in a cateogircal feature will only have the mean of the target for the entire training set. With k-fold CV, the cateogry value, say 'cat', will have a different target encoding across records, among the different k folds.



# References
* [K-Fold Target Encoding](https://medium.com/@pouryaayria/k-fold-target-encoding-dfe9a594874b)
* [Comprehensive study on mean encoding for categorical variables](https://www.kaggle.com/vprokopev/mean-likelihood-encodings-a-comprehensive-study)
