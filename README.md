# Text Embedding and Answer Generation Project

This project is designed to create a text embedding and answer generation pipeline using BERT and GPT-2 models. The project includes:

- Loading and splitting PDF documents into smaller chunks.
- Creating embeddings for the text chunks using BERT.
- Storing and retrieving embeddings using ChromaDB.
- Generating answers to queries based on the retrieved context using GPT-2.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/text-embedding-answer-generation.git
    cd text-embedding-answer-generation
    ```

2. Install the required packages:
    ```sh
    !pip install langchain langchain_community transformers chromadb openai pypdf
    ```
3. Add path to the text.pdf
4. Add a local path to the ChromaDB database

## Usage

1. Place your PDF file in the `content` directory and rename it to `text.pdf`.

2. Run the Jupyter notebook to execute the entire pipeline:
    ```sh
    jupyter notebook text_embedding_answer_generation.ipynb
    ```

3. The pipeline includes:
    - Loading the PDF document and splitting it into smaller chunks.
    - Creating text embeddings using a BERT model.
    - Storing embeddings in ChromaDB.
    - Retrieving relevant chunks based on a query.
    - Generating answers using a GPT-2 model based on the retrieved chunks.

4. Add the required question which you need an answer to in the query.
    ```python
    query = "question"
    ```

## Project Structure
```
text-embedding-answer-generation/
│
├── content/
│ └── text.pdf
│
├── text_embedding_answer_generation.ipynb
```
