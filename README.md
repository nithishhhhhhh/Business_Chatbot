# Business_Chatbot
Working model of Retrieval Augmented Generation (RAG) for a QA bot for a Business, leveraging the OpenAI API and a vector database (Pinecone DB).
Steps:
Set Up the Environment:
Import necessary libraries.
Set up OpenAI API key and Pinecone API key.
Initialize Pinecone:
Create a new index or connect to an existing one.
Define the schema for storing documents.
Document Ingestion:
Prepare documents and upload them to Pinecone.
Query Handling:
For each query, retrieve relevant documents from Pinecone.
Use OpenAI's GPT-4 model to generate answers based on retrieved documents.
Integration:
Combine retrieval and generation into a seamless pipeline.
