Basic Text vectorization and Embedding Techniques 

Disadvantage of BoW -
Feature values are either 1 or 0 hence it is not possible to determine which word is more important over another words. This is very important in solving problems like sentiment analysis.

This can be solvedd by TF-IDF (Term Frequency - Inverse Document Frequency)

TF-IDF : 

Term Frequency (TF) = No of repetition of words in sentence/ No of words in sentence

Inverse Document Frequency (IDF) = No of sentences/No of sentencts containing words

TF * IDF = Final outcome.
Note: Values are calculated in terms of logs 

Word2Vec :

Word2vec is one of the most popular technique to learn word embeddings using a two-layer neural network. Its input is a text corpus and its output is a set of vectors. Word embedding via word2vec can make natural language computer-readable, then further implementation of mathematical operations on words can be used to detect their similarities. A well-trained set of word vectors will place similar words close to each other in that space.

There are two main training algorithms for word2vec, one is the continuous bag of words(CBOW), another is called skip-gram. The major difference between these two methods is that CBOW is using context to predict a target word while skip-gram is using a word to predict a target context. Generally, the skip-gram method can have a better performance compared with CBOW method, for it can capture two semantics for a single word. 

Problems with BoW and TF-IDF are -
1. Semantic information is not stored
2. Importance is given to uncommon words (TF-IDF)
3. Chances of overfitting 

Word2Vec advantages -
1. Each word is represented as a separate vector of size 32 or more (not a decimal value like in TF-IDF)
2. Semantic info and relation between words is preserved
3. Each word is presented in 2-D vector. Example Man(3,6), Women (3.2,6.2) - This shows "Man" and "Women" are related because dimensionally they are near to each other. 

For Huge dataset - Word2Vec is a better option
Word2Vec implementation - Gensim lib can be used. It creates a 100-d vector for words
<!---
anishsavla2/anishsavla2 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
