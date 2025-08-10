# RAG with LangChain and Pinecone

This project demonstrates a simple Retrieval-Augmented Generation (RAG) pipeline using [LangChain](https://www.langchain.com/), [Pinecone](https://www.pinecone.io/), and OpenAI embeddings.  
It consists of two main scripts:
- `ingestion.py` – for loading and embedding documents into Pinecone.
- `main.py` – for querying the stored data and retrieving relevant answers.

## Project Structure
├── ingestion.py # Handles document loading, chunking, embedding, and storage in Pinecone
├── main.py # Retrieves and queries the Pinecone index using LangChain
├── mediumblog1.txt # Example source document
