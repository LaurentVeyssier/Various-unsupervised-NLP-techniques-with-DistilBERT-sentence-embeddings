# Various unsupervised NLP techniques with DistilBERT
Usage of BERT pre-trained model for unsupervised NLP and text clustering techniques


This notebook illustrates the techniques for text clustering described in [SBERT.net](https://www.sbert.net/examples/applications/computing-embeddings/README.html).
The architecture uses DistilBERT language model and Sentence-Transformers model.
The techniques described in the notebook are:
- Computing sentence embeddings from pretrained BERT model
- Semantic textual similarity
- Semantic search

Both approaches use cosine similarity. In contrast to traditional search, that only finds documents based on lexical matches, semantic search can also find synonyms. These techniques leverage the embedding representation of text to identify the closest element from a semantic view (capture the meaning).

- Text clustering
  - k-means
  - agglomerative clustering
  - fast clustering

Here embeddings are also utilized to cluster based on semantic proximity.


The notebook uses [Quora duplicate questions dataset](http://qim.fs.quoracdn.net/quora_duplicate_questions.tsv).
