# ResearchPilot

**ResearchPilot** is an AI-powered academic research assistant designed to help researchers explore scientific literature, retrieve relevant evidence from research papers, and generate reliable, citation-grounded answers to research questions.

The application combines **Retrieval-Augmented Generation (RAG)** with external academic literature discovery, enabling users to query uploaded research papers, search for relevant publications, or combine both sources for a broader research perspective.

## Key Features

- **PDF Ingestion & Indexing** – Upload academic papers, extract text, and split content into overlapping chunks for efficient retrieval.
- **Semantic Search (RAG)** – Retrieve relevant passages from indexed papers using Sentence Transformers embeddings and ChromaDB vector storage.
- **External Literature Discovery** – Search academic publications through the OpenAlex API to identify relevant research, authors, publication years, DOIs, and citation counts.
- **Multi-Source Research** – Explore uploaded documents, external literature metadata, or combine both research modes.
- **Evidence-Grounded AI Responses** – Generate academic answers using retrieved evidence and OpenAI models.
- **Citation Validation** – Track local PDF citations and external references, validate citation formats, and flag missing or malformed citations.
- **Persistent Vector Database** – Store indexed paper chunks in ChromaDB for reuse during the Colab runtime.
- **Interactive Gradio Interface** – Access paper indexing and research functionality through a simple web-based interface.

## Tech Stack

Python · OpenAI API · ChromaDB · Sentence Transformers · PyMuPDF · OpenAlex API · Gradio · Requests

## Workflow

1. Upload a research paper in PDF format.
2. Extract and chunk the document text.
3. Generate embeddings and store them in ChromaDB.
4. Submit a research question.
5. Retrieve relevant local passages and/or external literature metadata.
6. Generate an evidence-based response with citations.
7. Review the answer alongside its retrieved supporting evidence.

## Research Modes

- **Local PDF** – Answer questions using uploaded and indexed research papers.
- **External Papers** – Discover relevant academic literature through OpenAlex.
- **Combined** – Integrate local document evidence with external literature metadata.

## Objective

To make academic research more accessible and efficient by simplifying literature exploration, semantic retrieval, and evidence-based synthesis while maintaining transparency about sources and limitations.

