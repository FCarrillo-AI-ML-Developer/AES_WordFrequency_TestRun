# Automated Essay Scoring Using Word Frequency Analysis
Dataset: The Hewlett Foundation - ASAP AES https://www.kaggle.com/competitions/asap-aes/data

## Overview
This project explores the correlation between word frequency and essay scores using Natural Language Processing (NLP) techniques. Our analysis is based on the observation that students with higher essay scores (e.g., 12) tend to use a greater number of common words compared to those with lower scores (e.g., 2). The objective is to determine whether word frequency can serve as a predictive feature for automated essay scoring.

## Methodology
1. **Word Frequency Analysis:**

Extract word frequency distributions from essays to identify commonly used words.
Count the occurrences of these common words in each essay to examine potential correlations with assigned scores.
2. Dataset & Test Sample:

The dataset includes human-scored essays.
A test sample of 18 essays is used, with three essays representing each score category: 12, 10, 8, 6, 4, and 2.
Preprocessing Steps:

3. Convert text to lowercase.
Remove mentions (words starting with @), punctuation, and unnecessary whitespace.
Tokenize text for further processing.
Apply spell-checking to correct common misspellings (e.g., "wouldnt" → "would not", "havent" → "have not", "camputer" → "computer"). Since the grading rubric does not penalize spelling errors, this step ensures consistency in word frequency analysis.
Perform lemmatization after spell correction to group words into their root forms.
Remove stop words to focus on meaningful content and prevent skewed frequency distributions.
## Expected Impact
By refining preprocessing techniques and analyzing word frequency distributions, this project aims to provide insights into how commonly used words influence essay scoring. The findings may contribute to the development of automated scoring models for more efficient and fair grading.
