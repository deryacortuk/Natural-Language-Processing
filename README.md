• Understanding business problems
• Data collection from open source
• Understanding data and creating a separate data frame
• Text preprocessing
• Feature engineering techniques like count vectorizer, word-level TFIDF, word embeddings
• At the model-building phase, k-means unsupervised learning approach
• Considered three methods: elbow, silhouette score, and dendrogram to define the number of clusters
• Clusters are visualized through monogram word cloud to get more sense out of it and for cluster interpretation
• Topic extraction from each cluster using LDA techniques to further enhance the cluster interpretation
• Each topic model for clusters is visualized separately by using pyLDAvis
• Insights are drawn from word clouds on clusters and their corresponding topic models


# Data Cleaning and Preprocessing
Cleaning text data is important to obtain better features. It can be achieved by doing some of the basic preprocessing steps on the data.
The following are the preprocessing steps.
1. Make words lowercase.
2. Remove stop words.
3. Correct spelling.
4. Remove numbers.
5. Remove whitespace and special characters.

# Elbow Method
The elbow method is a type of method for checking the consistency of clusters created. It finds the ideal number of clusters in data. Explained variance considers the percentage of variance explained and derives an ideal number of clusters. If the deviation percentage explained is compared with the number of clusters, the first cluster adds a lot of information, but at some point, explained variance decreases, which gives an angle on the graph. At the moment, the number of clusters is selected.

# Silhouette Coefficient
The silhouette coefficient, or silhouette score, tells how much the object is similar to other clusters compared to its own cluster. The value varies from –1 to 1, where a high value indicates that the cluster fits well with itself, and the cluster does not match the neighboring cluster.
The silhouette value is calculated using distance metrics like Euclidean distance, the Manhattan distance, and so on.
