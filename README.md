# Multi-PDF RAG Chatbot

An AI-powered document chatbot built using LangGraph, Qdrant, OpenAI, and Streamlit.

## Features

- Multi-PDF ingestion
- Semantic search using Qdrant
- Retrieval-Augmented Generation (RAG)
- LangGraph workflow orchestration
- Conversational document QA
- Streamlit UI

## Tech Stack

- LangGraph
- LangChain
- OpenAI
- Qdrant
- Streamlit

## Architecture

PDFs
→ Chunking
→ Embeddings
→ Qdrant Vector DB
→ Retrieval
→ OpenAI LLM
→ Final Response

## Run Locally

### Install dependencies

```bash
# Requirements

## Software Requirements

- Python 3.11+
- Git
- Qdrant Cloud account
- OpenAI API key

## Python Libraries

Install all dependencies using:

```bash
pip install -r requirements.txt
```

Main libraries used:

- langgraph
- langchain
- langchain-openai
- langchain-community
- langchain-qdrant
- langchain-text-splitters
- qdrant-client
- streamlit
- python-dotenv
- pypdf

## Environment Variables

Create a `.env` file:

```env
OPENAI_API_KEY=your_openai_api_key

QDRANT_URL=your_qdrant_cluster_url

QDRANT_API_KEY=your_qdrant_api_key
```
```

### Add environment variables

Create `.env`

```env
OPENAI_API_KEY=your_key
QDRANT_URL=your_url
QDRANT_API_KEY=your_key
```

### Run ingestion

```bash
python ingest.py
```

### Run chatbot

```bash
streamlit run app.py
```

## Example Questions

- What is Generative AI?
- Explain embeddings
- What is LangGraph?
- Which place is famous for beaches?
