# Brain Tumor Detection using RAG and Focling Vector Store

## Overview
This project implements a **Brain Tumor Detection** system using **Retrieval-Augmented Generation (RAG)** with a **Focling Vector Store**. The application uses **LangChain, OpenAI, Qdrant, and Streamlit** to analyze medical images and provide insights based on stored medical knowledge.

## Features
- **Image-based Brain Tumor Detection**: Accepts an image URL and determines whether it contains a brain tumor.
- **RAG Integration**: Uses a Qdrant vector store to retrieve relevant medical documents.
- **LLM-powered Responses**: Uses OpenAI's vision model to analyze the image and answer questions.
- **PDF Document Loader**: Ingests medical literature (PDFs) to enhance knowledge retrieval.
- **Streamlit UI**: Provides an interactive web interface for easy user interaction.

## Tech Stack
- **Programming Language**: Python
- **Frameworks & Libraries**:
  - OpenAI API (for vision model inference)
  - LangChain (for RAG pipeline)
  - Qdrant (for vector storage)
  - Ollama Embeddings (for text embeddings)
  - PyPDFLoader (for document ingestion)
  - Streamlit (for UI)

## Installation & Setup
### Prerequisites
Ensure you have Python installed (>=3.8) and install the required dependencies:
```sh
pip install openai langchain_qdrant langchain_ollama streamlit qdrant-client
```

### Configuration
- Set up **Qdrant** by providing the URL and API key.
- Ensure you have an **OpenAI API Key**.

## Usage
### 1. Start the Application
```sh
streamlit run app.py
```
### 2. Provide Inputs
- **Enter an image URL** for brain tumor analysis.
- **Ask a medical question** related to the image.

### 3. Check Results
- If the image contains a tumor, the model provides an answer based on stored medical knowledge.
- If no tumor is detected, it responds with **"I don't know"**.



## Future Enhancements
- Fine-tune a **custom vision model** for more accurate tumor classification.
- Add **multi-modal embeddings** to improve retrieval accuracy.
- Implement **real-time model inference** using a local LLM setup.

## Credits
Developed by [Your Name]. Contributions welcome!

## License
This project is licensed under the MIT License.

