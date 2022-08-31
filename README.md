# Vector Space Semantics for Similarity between Eastenders Characters

A vector representation is created of a document (Eastenders script data). Then that representation is improved in such a way that each character vector is maximially distinguished from the other character documents. This distinction is measured by how well a simple information retrieval classification method can select documents from validation and test data as belonging to the correct class of document (i.e. deciding which character spoke the lines by measuring the similarity of those document vectors to those built in training).

The following tasks have been performed here:
* Pre-processing is preformed by converting the tokens into lowercase. Then, lemmatizing and stemming the tokens consecutively. Finally, the stopwords have been removed.
* Feature extraction have been used by extracting n-grams of different lengths and including their POS-tags.
* Added dialogue context data and features so that the data incorporates the context of the line spoken by the characters in terms of the lines spoken by other characters in the same scene (immediately before and after).
* Matrix transformation technique has been used, here TF-IDF tranformer.