# Wikipedia RAG System

A Retrieval-Augmented Generation (RAG) application that extracts, processes, and queries Wikipedia content using natural language processing techniques.

---

## Overview

This project demonstrates how external knowledge sources can be integrated into an AI pipeline to improve information retrieval and question answering. The system retrieves Wikipedia article content, preprocesses textual data, and enables intelligent querying through a Retrieval-Augmented Generation workflow.

The project focuses on evaluating how document chunking strategies and contextual overlap influence retrieval accuracy and response quality.

---

## Features

- Wikipedia content extraction
- Text preprocessing and document parsing
- Prompt-based querying
- Retrieval-Augmented Generation pipeline
- Modular Python implementation
- Retrieval performance experimentation

---

## Technologies Used

- Python
- Natural Language Processing (NLP)
- Information Retrieval
- Retrieval-Augmented Generation (RAG)
- Prompt Engineering

---

## Project Structure

```
RAG_app.py              Main application logic
text_extractor.py       Wikipedia text extraction and preprocessing
prompts.md              Query templates
Selected_Document.txt   Source document
requirements.txt        Project dependencies
```

---

## Installation and Usage

### Clone the repository

```bash
git clone https://github.com/jesusbenitez08/wikipedia-rag-system.git
cd wikipedia-rag-system
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Run the application

```bash
python RAG_app.py
```

---

## Retrieval Evaluation

The system was evaluated using multiple document chunking configurations to analyze retrieval effectiveness and generated response quality.

### Observations

- Smaller chunks (~200 tokens) enabled faster retrieval but often lacked sufficient contextual information.
- Larger chunks (600–800 tokens) improved answer completeness by preserving semantic context.
- Introducing overlap between chunks (50–100 tokens) significantly reduced information loss across related sections.
- Retrieval accuracy improved when contextual continuity between document segments was maintained.

### Limitations Identified

- Responses occasionally inferred missing information when retrieval confidence was low.
- Ranking of retrieved results could be improved through reranking techniques.
- Pronoun resolution across long text segments remained challenging in some cases.

---

## Example Use Case

The system retrieves structured information from Wikipedia articles and enables users to query knowledge sources efficiently using AI-assisted retrieval techniques.

---

## Future Improvements

- Vector database integration (FAISS or ChromaDB)
- Retrieval reranking models
- Multi-document knowledge ingestion
- LLM API integration
- Web-based user interface
- Quantitative evaluation metrics

---

## Learning Outcomes

This project explores practical challenges involved in building Retrieval-Augmented Generation systems, including:

- Document preprocessing strategies
- Context preservation during retrieval
- Prompt-driven querying workflows
- Trade-offs between performance and contextual accuracy
