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

This dataset extends the verb disambiguation dataset of Grefenstette & Sadrzadeh 2011 to VP-elliptical settings.
[Link](https://github.com/gijswijnholds/compdisteval-ellipsis/blob/master/datasets/ELLDIS.txt)

### ELLSIM

This dataset extends the verb disambiguation dataset of Kartsaklis & Sadrzadeh 2013 to VP-elliptical settings.
[Link](https://github.com/gijswijnholds/compdisteval-ellipsis/blob/master/datasets/ELLSIM.txt)

## Models

We provide four trained vector spaces, following several popular embedding methods. For each of the vector spaces, we also provide a separate *tensor space*, containing learned matrices for 85 verbs that occur in the evaluation datasets. The tensors are presented in a flattened format, so they need to be reshaped to size *(d, d)* for *d* the dimension of the corresponding vector space.

| Model Name    | Dimensions | Vectors                  | Tensors                  |
| ------------- |:----------:| :----------------------: | :----------------------: |
| count         | 2000       | [link][count_vectors]    | [link][count_tensors]    |
| word2vec      | 300        | [link][word2vec_vectors] | [link][word2vec_tensors] |
| glove         | 300        | [link][glove_vectors]    | [link][glove_tensors]    |
| fasttext      | 300        | [link][fasttext_vectors] | [link][fasttext_tensors] |


## Code

We provide some code for evaluating the vector space models on the new datasets.

[count_vectors]: https://ln.sync.com/dl/eaccaea00/4sqgam5y-dj8fgyuv-8fhxien5-jct4htqi
[count_tensors]: https://ln.sync.com/dl/4518d95f0/j8sq4n8d-mmi4iiin-2stkr92r-b7my3s6m
[word2vec_vectors]: https://ln.sync.com/dl/9189b10d0/v4p9qtvg-6a4zhhiv-dt4am2cq-vv32h7j8
[word2vec_tensors]: https://ln.sync.com/dl/83dce9040/wap786ba-w55pxysy-tsebqz3u-isf5bisu
[glove_vectors]: https://ln.sync.com/dl/c66e50cc0/bf7nnmm3-rwde43an-gw6q8raq-vfdr6jy6
[glove_tensors]: https://ln.sync.com/dl/2b21bc080/3u4kby9s-z8uks3ns-m4hfg5pu-jm8edb5u
[fasttext_vectors]: https://ln.sync.com/dl/2ef558dc0/2mdzq2er-kuvf8yk8-f7zbgsxx-ymmbvx38
[fasttext_tensors]: https://ln.sync.com/dl/44be89600/v45je9ek-nzfqzahx-uvyjdvwb-df82qkmq

