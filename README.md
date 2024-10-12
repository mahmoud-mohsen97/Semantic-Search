# Semantic Search in articles using ChromaDB
## Introduction:
In this project, we aim to create a semantic search pipeline using the Chroma vector database to search for some words within English articles and extract hot keywords. Semantic search is essential for efficient information retrieval and has various real-world applications. 

**Problem Description:**

The challenge is to efficiently search for specific words in articles and extract relevant keywords that capture the article's essence. The pipeline utilizes Chroma vectors to address this problem effectively.
## Data Description:
I made a data that consists of some articles in .txt format that talk about the services that a company offers in AI & DS fields 
## Experiments:
- Pre-processing: To prepare the articles for semantic search, we cleaned and standardized the text for improving the accuracy of the search results.
- Semantic Search Pipeline : 
  - Creating ChromaDB Client and Collection
  - Adding Documents to ChromaDB and
  - Querying
  - Performing Semantic Searches
  - Extracting Hot Keywords and plotting by Word cloud

## Optimization for Time Efficiency:
We optimize the search process by using indexing techniques and efficient data structures. This ensures that the semantic search is performed with minimal time complexity.
## Conclusion :
Our semantic search pipeline successfully retrieves relevant articles based on specific keywords and then generates a word cloud visualization to highlight the most frequent words in each file's content 

**=> There is a need to enhance the information retrieval process where the output be a summary and more customized for the query**

Potential Applications: The developed pipeline can be applied in diverse scenarios, from assisting researchers in literature review to helping businesses analyze textual data for insights for example ChatPDF
## Tools and Resources:
- 🏡 Home | Chroma (trychroma.com)
- Sentence-transformers
- nltk
- Word cloud
- The handmade data is included in the folder with this file
## Challenges and Learnings:
Understanding and implementing the vector database and finding a suitable way to extract the hot keywords 
