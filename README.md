# Defining Artist "Eras" Through Lyrical Analysis

This project explores how an artist’s lyrics evolve over time and whether their musical “eras” can be identified through semantic analysis.

Inspired by the concept of the **Eras Tour**, this Jupyter Notebook uses modern AI techniques to detect distinct lyrical themes and evaluate how they align with traditional markers like albums and release dates.

## Origin

This project began as a capstone for Kaggle's [5-Day Gen AI Intensive Course with Google](https://www.kaggle.com/learn-guide/5-day-genai).

The official submission on Kaggle, which includes the full notebook **and results**, can be found [here](https://www.kaggle.com/code/ronsarbo/lyric-analysis-capstone-ron-arbo)

You can edit and run the notebook directly on Kaggle.

## Notebook Outline

The Notebook contains the following sections:

### Setup

- Install and import required packages
- Set up API Key

### Data

- Import datasets
- Clean data

### Create Embeddings

- Create `clustering` embeddings for lyrics

### Dimensionality Reduction

- Use [TSNE](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html) to reduce embeddings to 2 dimensions for visualization

### Clustering Embeddings

- Use [KMeans](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) to create semantic clusters from the embeddings

### Defining the Cluster Using AI

- Define the clusters by prompting an AI to identify commonalities between the lyrics of each cluster

### Visualizing Cluster Relationships

- Graph cluster relationships
  - Cluster-Album
  - Cluster-Time

### Evaluating Cluster Definitions

- Create document embeddings for cluster definitions and query embeddings for lyrics
- Evaluate definitions by querying vector database and comparing returned definition to the original

### Conclusion

- Review goals, findings, and limitations with the project

### Citations

- Cite sources used

## Technologies Used

- **Kaggle**
  - Python
    - Pandas, NumPy, Seaborn, Scikit-learn
  - Jupyter Notebook
- **AI Capabilities**
  - Embeddings (`clustering`, `retrieval_query`, and `retrieval_document`)
  - Few-shot Prompting
  - Structured output with JSON
  - Vector databases and querying
