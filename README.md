# compdisteval-ellipsis
This repository links to the datasets, models and code for evaluating composition models for VP-elliptical sentences, as described in the article

Gijs Wijnholds and Mehrnoosh Sadrzadeh. *Evaluating Composition Models for Verb Phrase Elliptical Sentence Embeddings.* NAACL-HLT 2019.

If you find any of this useful, please consider citing our paper as

```
@inproceedings{wijnholds2019evaluating,
  title = "Evaluating Composition Models for Verb Phrase Elliptical Sentence Embeddings",
  author = "Gijs Wijnholds and Mehrnoosh Sadrzadeh",
  year = "2019",
  booktitle={Proceedings of the 2019 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long Papers)},
  publisher={Association for Computational Linguistics}
}
```


## Datasets
We provide two new datasets, extending the verb disambiguation dataset of Grefenstette & Sadrzadeh 2011 and the transitive sentence similarity dataset of Kartsaklis & Sadrzadeh 2013.

### ELLDIS

### ELLSIM


## Models

We provide four trained vector spaces, following several popular embedding methods. For each of the vector spaces, we also provide a separate *tensor space*, containing learned matrices for 85 verbs that occur in the evaluation datasets.

word2vec: [Vectors][word2vec_vectors] [Tensors][word2vec_tensors]

## Code

We provide some code for evaluating the vector space models on the new datasets.

[word2vec_vectors]: https://ln.sync.com/dl/9189b10d0/v4p9qtvg-6a4zhhiv-dt4am2cq-vv32h7j8
[word2vec_tensors]: https://ln.sync.com/dl/83dce9040/wap786ba-w55pxysy-tsebqz3u-isf5bisu
