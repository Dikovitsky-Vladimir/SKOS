# SKOS relation classifier
Neural network classification of SKOS-ontology relations using the cosine distance between word vectors (GloVe) and the syntactic features of the context.

# Data description:
Train dataset DET_relations_with_vectors_and_similarity.csv contain concepts, relation(related,broader,narrower), word vectors and cosine distance.
Dataset DET_SKOS_with_text.csv was extended by sentences, which contain this word pair. Training datasets for SKOS relation are compiled from DBpedia[https://dbpedia.org/page/Simple_Knowledge_Organization_System] with GloVe model glove.6B.300d.bin [https://nlp.stanford.edu/projects/glove/] and SpaCY[https://spacy.io/]

# Structure:
'SKOS-classification-with-NN.ipynb'  contain creation doc2vec model for sentences using model glove.6B.300d.bin, train process, adding syntactic features to the training vectors, SKOS ontology creation process from text 'motor.txt' [https://en.wikipedia.org/wiki/Hydraulic_motor]

'Semeval.ipynb' run validation on gold stanford taxonomy SemEval[https://alt.qcri.org/semeval2016/task13/index.php] which contain two groups of pairs related to "food" and "science". Pairs connected in list and 1st word was replaced to "food"(all900food.csv) and "science"(all900science.csv). 

In 'bert-classification.ipynb' BERT binary classifier used for broader relation prediction.
