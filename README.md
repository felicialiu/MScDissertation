# MSc Dissertation
Electronic copy of my dissertation and summarising presentation.

# Abstract
The purpose of this study is to investigate different kinds of word embeddings to use for unsu- pervised part-of-speech tagging, which is tagging words with labels that denote their syntactical function given their context. Unsupervised models for NLP are needed to make use of the abun- dance of raw online textual data and to create systems that work with low-resource languages. This thesis will compare and contrast various neural network embedding models, in order to identify word embeddings that are well-suited for extracting relevant features on local word order, context, meaning, and morphology. Word-level embeddings have been trained with a context window of size 1 with different dimensions. The character-level embeddings have been extracted from a language model with a convolutional layer over characters. A Gaussian HMM is used as POS induction system. The findings were that models where a word is predicted from its context works better than embeddings where the context is predicted from a word. This means that CBOW and cwindow outperform the (structured) skipgram, and since cwindow is sensitive to word-order, it outperforms CBOW. On average the character-level embeddings performed around the level of GloVe and skipgram, which was good but not exceptional. In order to investigate the quality of the word embeddings trained for this project, we inspect the nearest neighbours and a 2D visualisation of the embedding space. This showed that word- level prediction-based embeddings have clusters of semantic similarity, whereas character-level embeddings have clusters of morphological similarity. Combining word- and character-level embeddings did very well in POS tagging. Further experiments included accounting for out- of-vocabulary words and performing tokenisation similar to the GHMM training data, where especially the latter showed significant improvement in POS tagging. On the basis of the results of this research it can be concluded that proper tokenisation and taking local word order into account can definitely improve embeddings for POS tagging. Furthermore, character-level em- beddings are able to represent words in a completely different manner than regular embeddings that encode semantic information, which can be useful if combined with semantic features. It is worth researching other ways of creating character-level embeddings, either for part-of-speech tagging or for better word representation.
