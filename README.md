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

We provide some code for evaluating the vector space models on the new datasets. This can be found in my main code repository for evaluation of compositional distributional semantics [here](https://github.com/gijswijnholds/compdisteval)


[count_vectors]: https://ln.sync.com/dl/b533b03c0/ertje7d2-vq66ivey-fevjp8g8-asai3pz7
[count_tensors]: https://ln.sync.com/dl/a5e144f80/86cjd786-6mu265q8-hqsvr5ms-t9kprjp4
[word2vec_vectors]: https://ln.sync.com/dl/e93a0a060/xm5njmyd-hqvbgw5d-cdmviv9q-6ye8yrsb
[word2vec_tensors]: https://ln.sync.com/dl/88a20c1c0/uh9friau-7tvb4mmu-nukuty3f-yzw92yuh
[glove_vectors]: https://ln.sync.com/dl/a6f296b30/2z7yvyvt-63m7qyi2-8zd4j6zc-xygvr2ke
[glove_tensors]: https://ln.sync.com/dl/524f8a0c0/5s4rruv7-iyg2fu7e-vvjgk2fy-d2wha4ja
[fasttext_vectors]: https://ln.sync.com/dl/54a3bfb80/yn7hfrxn-nxkue223-273ynmfq-ma6j4zy4
[fasttext_tensors]: https://ln.sync.com/dl/288e9e450/vfpxzacp-2awa4ikp-6cu3f6vy-a75jvd9p

