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

# Multilingual NLP
The following are the most prominent multilingual models.
• mBERT
• XLM
• XLM-R
• Multilingual BERT (mBERT): This is released along with the BERT and it supports 104 languages. Essentially it is BERT trained in many languages.
• XLM and XLM-R: XLM-R trains RoBERTa on a huge multilingual data set at an enormous scale.

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


# BART: Simple-Transformer Pretrained Model (Bidirectional and AutoRegressive Transformers) 
Bidirectional encoders form the first part of the BART transformers architecture. Autoregressive decoders form the second part. They are integrated to devise the seq2seq 
model. And, hence BART can also be used for many text-to-text-based applications, including language translation and text generation.
The AR in BART stands for autoregressive, where the model consumes the previously generated output as an additional input at each step.
This makes BART particularly effective in text-generation tasks. We fine-tuned BART for abstractive text summarization. BART offers an abstractive summarizer that can 
intelligently paraphrase, capture, and combine information based on contextual overlap. 
You can also experiment with tuning the beam width hyperparameter to optimize generative capabilities while minimizing the chances of misinformation.

# T5 Pretrained Model
T5 is short for text-to-text transfer transformer. It’s a transformer model from Google where it takes text as input and modified text as output. It is easy to fine-tune this model on any text-to-text task, which makes it very special.
This transformer model is trained on the Colossal Clean Common Crawl (C4) data set. The architecture is integrated to devise text2text model. And hence T5 can also be 
used for many text-to-text-based applications.

# Evaluation Metrics for Summarization
• ROUGE score: Basically, the number of words in the human-generated summary appeared in the machine-extracted summary. 
It measures the recall of the output in terms of machine learning 
evaluation.
• BLEU score: The score is calculated using the following formula.
Score = number of words in the machine-generated summary that appeared in the human-created summary.
The BLUE score gives the precision of the model.
