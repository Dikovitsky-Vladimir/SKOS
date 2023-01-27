# SKOS relation classifier 
Neural network classification of SKOS-ontology relations using the cosine distance between word vectors (GloVe) and the syntactic features of the context. 

# Data description: 
Train data:
1. DET_relations_with_vectors_and_similarity.csv  
2. DET_SKOS_with_text.csv

Training datasets for SKOS relation are compiled from DBpedia[https://dbpedia.org/page/Simple_Knowledge_Organization_System] with GloVe model glove.6B.300d.bin [https://nlp.stanford.edu/projects/glove/] and SpaCY[https://spacy.io/]
