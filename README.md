N-Gram Language Model
Project Overview

For this project, I built a simple N-gram language model using Python. The model uses text data to create unigrams and bigrams and calculate word probabilities.

What I Did
Preprocessed the text by making it lowercase.
Tokenized the text into individual words.
Created unigrams (single words).
Created bigrams (two words next to each other).
Calculated bigram probabilities using Maximum Likelihood Estimation (MLE).
Created a function to predict the most likely next word.
Created a function to calculate the probability of a sentence.
Generated sentences by sampling words from the model.
Compared the unigram and bigram models.
Unigrams and Bigrams

A unigram is one word by itself.

Example:

I, want, to, eat

A bigram is two words that appear next to each other.

Example:

(I, want), (want, to), (to, eat)

The bigram model uses the previous word to help predict what word comes next.

Next-Word Prediction

The model can take a word or phrase and predict the most likely next word based on the probabilities it learned from the text.

Example:

I want

Prediction:

to

Sentence Probability

The bigram model can also calculate the probability of a sentence by using the probabilities of each word based on the word before it.

Text Generation

The model can generate new sentences by starting with <s> and choosing the next word based on the probabilities from the bigram model. It stops when it reaches </s>.

Model Comparison

The bigram model usually produces more realistic text than the unigram model because it considers the word that comes before the next word.

The unigram model only looks at individual word probabilities, so the generated text can be more random and may not make much sense.

One limitation of the unigram model is that it does not understand word order. A limitation of the bigram model is that it only looks at one previous word, so it does not understand longer context.

Reflection
What was the most difficult part of building your language model?

The most difficult part for me was understanding how the bigram probabilities worked and using them to predict the next word. It took some practice to understand how the word counts were used to calculate the probabilities.
