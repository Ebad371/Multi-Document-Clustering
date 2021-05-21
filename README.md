# Multi-Document-Clustering
A multi-document clustering algorithm to cluster research papers of mainly nlp domain


This is a really extensive project. What it does:

1. Takes research papers as input (whether in a csv file or as a pdf through google drive)
2. Extracts the titles and abstracts if pdf is given as input
3. Cleans the abstracts using BeatifulSoup, Regex, Tokenization, Lemmatization 
4. Finds out the embeddings for the abstracts using SBERT
5. Now we have to find out that which papers can our KMeans algorithm can cluster and which it cannot (because the training set on which the KMeans was trained was limited to some topics only)
6. It was my own hand written code to do this. The code contains several lines which mainly uses cosine similarity in order to compare every paper with each other and then finding the new clusters
7. So, there are 2 programs to produce the clusters; 1 is the KMeans and the other is my code to produce NEW clusters
8. At the end we combine the output for these two programs and also find out the most semantically excessive keywords just for a good user experience
9. Also we produce a graph using the graphviz library for a more better user experience
