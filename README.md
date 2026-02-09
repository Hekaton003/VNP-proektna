# Topic Modeling and Trend Detection in Large Text Corpora

## Introduction
Topic modeling is a technique in natural language processing (NLP) and machine learning that aims to uncover latent thematic structures within a collection of texts. Topic modelling is a system learning technique that robotically discovers the principle themes or "topics" that represents a huge collection of documents. At the coronary heart of topic modelling, the concepts of "topics" and "topic models" comes into mind. A 'topic' is defined as a recurring pattern of words that best represents a theme within the documents. Topic models are algorithms that scan the document collection to discover these topics. They provide a way to quantify the structure of topics within the text and how these topics are related to each other. Topic models can be useful tools to discover latent topics in collections of documents. Recent studies have shown the feasibility of approach topic modeling as a clustering task.

## BertTopic
BERTopic is a topic modeling technique that leverages transformers and c-TF-IDF to create dense clusters allowing for easily interpretable topics whilst keeping important words in the topic descriptions. BERTopic can be viewed as a sequence of steps to create its topic representations. There are five steps to this process:
- Embeddings (models for transforming our input documents into numerical representations)
- Dimensionality Reduction (important aspect of BERTopic where the main goal is to reduce the dimensionality of the embeddings to a workable dimensional space (e.g., 5) for clustering algorithms to work with.)
- Clustering (process where we need to cluster our input embeddings  into groups of similar embeddings to extract our topics)
- Vectorizers (representing the quality of the topic representations is key for interpreting the topics, communicating results, and understanding patterns)
- Optional Fine-Tuning

## Arxiv Dataset
For this project we will use the Arxiv dataset which is a mirror of the original ArXiv data. For nearly 30 years, ArXiv has served the public and research communities by providing open access to scholarly articles, from the vast branches of physics to the many subdisciplines of computer science to everything in between, including math, statistics, electrical engineering, quantitative biology, and economics. This rich corpus of information offers significant, but sometimes overwhelming depth. Since the full arXiv dataset is quite large (approximately 1.1 TB and continuously growing), for the purposes of this project I will be using only the first 40,000 rows to reduce resource usage and ensure faster processing during development and experimentation.
