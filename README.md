# llm-experiments
A small personal project exploring Retrieval-Augmented Generation (RAG)
with a fully local LLM stack — LangChain, Chroma, and Ollama.

This is a learning exercise, not affiliated with any organization.
Sample documents only; no confidential or proprietary data is used or included.

## Stack
- LLM: Ollama (llama3.2:1b)
- Embeddings: sentence-transformers (all-MiniLM-L6-v2)
- Vector store: Chroma
- Orchestration: LangChain

## Setup
\`\`\`bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
ollama pull llama3.2:1b
\`\`\`

## Usage
\`\`\`bash
python src/ingest.py   # build the vector index from docs/
python src/query.py    # ask questions against it
\`\`\`
