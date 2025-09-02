# Book_recommender
This project is a semantic book recommender that uses Large Language Models (LLMs) to provide intelligent book recommendations.
## Features

### Text Data Cleaning
The data-exploration.ipynb notebook handles the initial data preparation. It contains the code to download the dataset from Kaggle and perform a thorough cleaning process, including dropping irrelevant columns to ensure the data is ready for analysis.

### Semantic (Vector) Search
The vector-search.ipynb notebook focuses on semantic search by building a vector database. It uses libraries like langchain-chroma and langchain-openai to create embeddings from the book descriptions. This allows the system to understand the meaning of a natural language query and find books with conceptually similar content.

### Zero-Shot Text Classification
In the text-classification.ipynb notebook, books are categorized as "fiction" or "non-fiction" using zero-shot classification. The code uses an LLM to automatically assign a category to each book, creating a valuable facet that users can use to filter their search results.

### Sentiment Analysis
This sentiment-analysis.ipynb notebook performs sentiment and emotion analysis on the book descriptions. It utilizes a pre-trained transformers model from Hugging Face library to analyze the text and extract emotions like joy, sadness, or suspense. The results are saved to a new CSV file, enabling users to sort books based on their tone.

### Web Application
The gradio-dashboard.py Python script contains the code for the web application. It uses the Gradio library to create an interactive user interface allowing users to get real-time book recommendations.

## Installation
This project was initially created with Python 3.11.
1. Clone the repository
2. The following dependencies are required:
   - kagglehub
   - pandas
   - matplotlib
   - seaborn
   - python-dotenv
   - langchain-community
   - langchain-opencv
   - langchain-chroma
   - transformers
   - gradio
   - notebook
   - ipywidgets
3. Create a .env file in the root directory and add your API keys.
  
    ```OPENAI_API_KEY="your_openai_api_key_here"```
    
    ```HUGGING_FACE_TOKEN="your_hugging_face_token_here"```
