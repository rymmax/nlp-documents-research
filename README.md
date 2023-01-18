# NLP Documents Research
My personal project of using NLP to classify and summarize quantitative finance research papers

I've developed a research paper classification engine based on weakly supervised NLP technique to build a classifier of finance documents.

# Required packages
First of all, for completing the next tasks you need to install such packages as Pandas, NumPy, Seaborn, Glob (in general they're already pre-built in Anaconda distribution); Gensim & NLTK (for completing NLP tasks) + pdf2txt & arxiv for retrieving and transforming documents we need.

# About this project
I've downloaded approximately two thousand quantitative finance papers and have transformed them into .txt format.</br>
I've developed the word embedding training. The embedding was trained on the entire length of a half of two thousand documents (a half of them was valid)
I've removed numbers, spaces, punctuations & some words that have length == 1.

- Why haven't I removed stopwords?
  - Due to the fact that the word embedding matrix will be used for creating pseudo documents, and they will need the presence of these words.

- Why haven't I used word stemming?
  - It works bad in finance in general cause most of the keywords in finance are already derivative words (trading, equity, fixed income etc.). There are lots of researches showing that performing stemming will distort the original meaning of the word.
