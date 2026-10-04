# RAG Open AI Demo

A hands-on Retrieval-Augmented Generation (RAG) project designed to explore how modern LLM systems ground responses in external knowledge sources. This repository demonstrates a practical understanding of document ingestion, chunking strategies, vector search, retrieval optimization, and answer generation using LangChain, ChromaDB, and OpenAI embeddings.

## Project overview

This project is a demonstration of core AI engineering skills in building RAG pipelines for enterprise-style knowledge retrieval. It covers the end-to-end workflow of turning raw documents into searchable, queryable knowledge assets that can support grounded responses from a large language model.

The repository emphasizes:

- Document loading and preprocessing
- Text chunking and chunk quality optimization
- Embedding generation with OpenAI models
- Vector store creation and persistence with Chroma
- Retrieval strategies for relevance and quality
- Answer generation with grounded context
- Advanced retrieval patterns such as hybrid search and reranking
- Notebook-based experimentation for learning and prototyping

## Skills showcased

This project reflects knowledge across several relevant AI and software engineering areas:

- Python development for AI workflows
- Retrieval-Augmented Generation architecture
- Vector databases and similarity search
- Prompt-aware document retrieval
- LLM application design and orchestration
- LangChain pipelines and integration patterns
- Query-based information retrieval and ranking
- Experimentation with notebooks and reproducible examples
- Practical understanding of chunking, context windows, and answer quality

## Repository structure

- `1_ingestion_pipeline.py` — loads documents from the `docs` directory and creates a Chroma vector store
- `2_retrieval_pipeline.py` — basic retrieval flow for querying stored embeddings
- `3_answer_generation.py` — generates answers grounded in retrieved documents
- `4_history_aware_generation.py` — conversation-aware generation using prior context
- `5_recursive_character_text_spliiter.py` — chunking using recursive character splitting
- `6_semantic_chunking.py` — semantic chunking experiments
- `7_agentic_chunking.py` — agent-like chunking and document organization logic
- `8_multi_modal_rag.ipynb` — multimodal RAG exploration
- `9_retrieval_methods.py` — evaluation of different retrieval approaches
- `10_multi_query_retrieval.py` — multi-query retrieval strategy
- `11_reciprocal_rank_fusion.py` — combining retrieval results through RRF
- `12_hybrid_search.ipynb` — hybrid search experimentation
- `13_reranker.ipynb` — reranking for improved result quality
- `docs/` — folder for source documents to ingest
- `requirements.txt` — Python dependencies
- `synthetic_questions.txt` — sample prompts for evaluation and testing

## Tech stack

- Python
- LangChain
- ChromaDB
- OpenAI embeddings and LLM APIs
- Jupyter Notebooks
- Python dotenv for environment management

## Typical workflow

1. Add relevant documents to the `docs/` directory.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Set your OpenAI API credentials in a `.env` file:
   ```bash
   OPENAI_API_KEY=your_api_key_here
   ```
4. Run the ingestion script:
   ```bash
   python 1_ingestion_pipeline.py
   ```
5. Query the vector store using retrieval examples and answer-generation scripts.
6. Explore notebook-based experiments to test chunking, reranking, multimodal, and hybrid retrieval strategies.

## Example use cases

This project is useful for understanding how to build:

- Internal knowledge assistants
- Document Q&A systems
- Research copilots
- Enterprise search over local knowledge bases
- Retrieval-based chat experiences grounded in trusted data sources

## Why this project matters

RAG is one of the most practical and valuable patterns in modern AI product development because it combines the strengths of large language models with trusted external knowledge. This repository demonstrates a real-world approach to building grounded AI systems that can answer questions using local or domain-specific documents instead of relying only on general model knowledge.

## Getting started

```bash
git clone https://github.com/godspeedmc/RAG_Open_AI_Demo.git
cd RAG_Open_AI_Demo
pip install -r requirements.txt
```

Then create a `.env` file with your OpenAI API key and start with the ingestion and retrieval scripts.

## Notes

This project is intended as an educational and demonstration repository for learning advanced retrieval patterns in AI applications. It is a strong example of applied knowledge in LLM workflows, vector search, and RAG system design.

