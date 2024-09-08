# Langchain Basics

## Project Overview

This project demonstrates the use of Langchain for document ingestion, data transformation, embeddings generation, and vector store management. The aim is to build a GenAI application that processes documents using Langchain, allowing for flexible and efficient information retrieval using OpenAI and Ollama embeddings.

## Key Features

1. **Data Ingestion**: 
   - Utilizes various document loaders such as:
     - PDF documents
     - Wikipedia articles
     - Web links
     - Arxiv papers
   - These loaders enable easy data extraction from different sources.

2. **Data Transformation**: 
   - Implements techniques for efficient text chunking, including:
     - `RecursiveTextCharacterSplitter`
     - `CharacterTextSplitter`
     - `HTMLTextSplitter`
   - These techniques ensure that the input text is appropriately segmented for downstream processing.

3. **Embeddings**: 
   - Supports multiple embedding models for generating vector representations of text:
     - `OpenAIEmbedding` (OpenAI's paid embedding service)
     - `OllamaEmbedding` (open-source alternative)
     - `HuggingfaceEmbedding` (Hugging Face models for embeddings)

4. **Vector Store**: 
   - Vector stores enable fast and efficient similarity search and retrieval using embeddings. This project uses:
     - `FAISS` (Facebook AI Similarity Search)
     - `Chroma` (an open-source vector store)
   
5. **GenAI App**:
   - Built a simple Generative AI (GenAI) app using:
     - OpenAI's API for generating responses
     - Ollama's embedding model as a cost-effective, open-source alternative
   - The app demonstrates how to integrate different embeddings and vector stores.
