
# Business Chatbot with Retrieval-Augmented Generation (RAG)

This repository contains the implementation of a Business Chatbot that utilizes Retrieval-Augmented Generation (RAG) for efficient and accurate question-answering (QA). The chatbot combines the power of OpenAI's language models and Pinecone's vector database to provide answers based on a set of documents, such as PDFs.

## Overview

The Business Chatbot is designed to assist users by answering questions based on the contents of provided documents. This is achieved through the following steps:

1. **Document Ingestion**: PDF documents are processed, and their text content is extracted.
2. **Embedding Generation**: The extracted text is converted into embeddings using OpenAI's embedding models.
3. **Indexing**: The embeddings are stored in Pinecone's vector database for efficient retrieval.
4. **Query Handling**: When a user asks a question, the chatbot retrieves the most relevant documents from Pinecone.
5. **Answer Generation**: The retrieved documents are used as context to generate accurate answers using OpenAI's language models.

## Features

- **PDF Document Processing**: Automatically extracts text from PDF files.
- **Embedding Creation**: Utilizes OpenAI's latest embedding models for robust representation.
- **Efficient Retrieval**: Uses Pinecone's vector database to quickly find relevant documents.
- **Accurate Answer Generation**: Employs OpenAI's language models to generate coherent and contextually relevant answers.

## Prerequisites

- Python 3.7 or higher
- OpenAI API Key
- Pinecone API Key and environment

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/business-chatbot-rag.git
   cd business-chatbot-rag
   ```

2. **Install Required Packages**:
   ```bash
   pip install openai pinecone-client pymupdf
   ```

3. **Set Up API Keys**:
   Replace the placeholder values in the code with your actual OpenAI and Pinecone API keys.

## Usage

1. **Initialize Pinecone and Create Index**:
   Create an instance of the Pinecone client and initialize the index for storing document embeddings.

2. **Process PDF Documents**:
   Extract text from PDF files in the specified directory and convert the text into embeddings.

3. **Upload Embeddings to Pinecone**:
   Store the embeddings in Pinecone for efficient retrieval during query handling.

4. **Handle Queries and Generate Answers**:
   Retrieve relevant documents based on user queries and generate answers using the context from the retrieved documents.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an issue to discuss any changes.
