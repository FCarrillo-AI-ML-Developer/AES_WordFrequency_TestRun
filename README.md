# Kaggle - The Hewlett Foundation: Automated Essay Scoring
Dataset found on https://www.kaggle.com/competitions/asap-aes/data

Word Frequency Preprocessing Feature Using NLP

Students with low scores, such as a 2, use fewer common words in their essays, while students with a score of 12 use more common words in their essays. Based on this observation, the more common words students write in their essays, the more positive the effect on their essay scores.
- First identify the frequency of words mentioned in every essay and then identify the common words. Finally count how many common words are in each essay to identify if there is a correlation on the score and the common words.
- Test Run focuses on a small sample that contains eighteen human scored essays. From the eighteen essays there is three essays for each score: 12, 10, 8, 6, 4, 2.
- To narrow down the common words text of the essays will be turned to lowercase, any words that start with @___ will be removed, punctuctuation will be removed, white spaces will be removed, and then each word will be turned into a token. In the 8th grade essays there is a lot of mispelling and the rubric does not seem to penalize for mispelling. Hence the tokens will be go through spell cheker to autocorrect any mispellings such as: "wouldnt" to "would not", "havent" to "have not", or "camputer" to "computer". This move will help identify stop words and add group words for frequency. Furthermore, spellchecking before lemmatization will help mispelled words into their rootform. Finally, stop words will be removed as they take away focus from meaniful words and skew results when finding the most frequent words.
