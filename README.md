# Semantic Search in Articles

This project demonstrates building a semantic search pipeline to retrieve relevant information from English articles using vector embeddings. Traditional search methods rely on lexical matching, but semantic search leverages the meaning of words, enhancing the accuracy and relevance of search results. Two approaches are explored using ChromaDB and Cohere embeddings.

## Approach 1: Semantic Search with ChromaDB
### Problem Description
The goal is to efficiently search for specific words within English articles and extract relevant keywords. ChromaDB is used for vector-based search to improve the accuracy of information retrieval.
### Workflow
1. Pre-processing: Clean and standardize the text.
2. Semantic Search Pipeline:
  - Create a ChromaDB client and collection.
  - Add documents to ChromaDB and query using vector search.
  - Perform semantic searches and extract hot keywords.
3. Visualization: Generate a word cloud to visualize the frequent keywords in the articles.

### Results
The semantic search pipeline effectively retrieves relevant articles and highlights key concepts through word clouds. There is potential to enhance the output to generate summaries and more customized answers.
### Tools
- ChromaDB: Vector database for semantic search.
- Sentence-transformers, nltk, WordCloud for pre-processing and visualization.

## Approach 2: Semantic Search with Cohere and Annoy
### Problem Description
This approach focuses on embedding-based search using Cohere’s multilingual model and Annoy for fast vector search within a pre-existing article.
### Workflow
1. Data Processing: The article is split into meaningful paragraphs, which are embedded into numerical vectors.
2. Semantic Search Pipeline:
  - Embed paragraphs using Cohere’s multilingual model.
  - Build a vector search index using Annoy for fast retrieval of relevant chunks.
3. Search Optimization: Integrating Cohere’s command-r-plus model for answer generation improves search precision in both Arabic and English.
### Results
This approach successfully generated precise, context-aware answers and provided a better user experience for question-answering tasks based on the article.
### Tools
- Cohere API for text embeddings and answer generation.
- Annoy for fast vector search.
- NumPy, python-dotenv for embedding handling.

## Conclusion
Both approaches effectively implemented semantic search in articles, with vector-based methods enhancing the search accuracy compared to traditional methods. ChromaDB offers fast search and keyword extraction, while Cohere and Annoy provide contextual search and precise answer generation, particularly useful in multilingual scenarios.
## Tools and Resources
- ChromaDB, Sentence-transformers, Cohere API, Annoy, WordCloud.
- External resources: Chroma and Annoy documentation.
