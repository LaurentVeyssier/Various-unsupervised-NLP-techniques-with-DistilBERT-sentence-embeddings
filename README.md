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

Two additional notebooks are added. These are introduced and described in this interesting analysis published in [medium](https://medium.com/swlh/semantic-search-with-nlp-86084ca81247). The author explores sentence embeddings using SBERT. SBERT generates embeddings from a pretrained BERT model which is then modified with Siamese and Triplet network structures to generate meaningful Sentence Vectors. SBERT approach is described in this [paper](https://arxiv.org/pdf/1908.10084.pdf). Sentence embedding proves superior for semantic search as opposed to pure lexical matches which would fail at identifying similar meaning from a query. Sentence embedding also performs better than averaging word embeddings from a sentence.
- experiment looking at sentence similarity using the average of BERT embeddings at word level
- experiment looking at sentence similarity using SBERT model leveraging transfer learning from BERT to produce sentence embeddings
These two notebooks run smoothly on google drive.
