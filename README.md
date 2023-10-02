# Assignment 1: Train Word2Vec on peS2o Dataset (AllenNLP)

Train a Word2Vec base model for generating sentence embeddings on the peS2o dataset (or the arxiv dataset).

## Requirements:

- **Dataset Source**: Research papers should be collected only from the Computer Science domain.
- **Data Split**: Use a random training set of 3000 documents and a test set of 1000 documents.
- **Linguistic Unit**: The input context matrix's row vector should represent sentences, not words. In other words, embed sentences instead of individual words.
- **Pre-processing**: The input context matrix should undergo the following cleanup:
  1. Remove stopwords
  2. Remove URLs
  3. Remove bullet points
  4. Remove apostrophes
  5. Remove hyphens
  6. Convert enumerations (e.g., like how this list is being enumerated)
  7. Convert numbers to text
  8. Remove punctuations
- **Initialization**: The Context Matrix should be initialized using TF-IDF based vector modeling.

## Evaluation:

Manually evaluate the model's accuracy using your custom evaluation dataset. Alternatively, you can use the benchmark evaluation dataset from [SemEval STS](http://ixa2.si.ehu.eus/stswiki/index.php/STSbenchmark?authuser=0) to compare pairs of similar and dissimilar sentences from research papers.

## Useful Links:

- [peS2o Dataset on GitHub](https://github.com/allenai/peS2o?authuser=0)
- [SemEval STS Benchmark](http://ixa2.si.ehu.eus/stswiki/index.php/STSbenchmark?authuser=0)
