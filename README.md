# Agentic AI & Multimodal Intelligence Portfolio

A practical collection of projects built while studying Agentic AI — covering how AI reasons, acts autonomously, and understands visual data. The work here moves beyond simple prompt-response patterns into systems that plan, evaluate, and improve their own outputs.

---

## Projects

### 🔬 Lab 1 — Vision-Language Fine-tuning (BLIP)
> [`Lab1_Finetuning/`](./Lab1_Finetuning)

Fine-tuning the BLIP (Bootstrapping Language-Image Pre-training) model to generate better image captions for specific domains. Built a custom PyTorch training pipeline using the Hugging Face `transformers` library to adapt a general-purpose vision-language model on a niche dataset.

- Custom image captioning pipeline with domain-specific training
- Evaluation of pre-trained vs. fine-tuned caption quality
- Hands-on exploration of how visual perception connects to language generation

---

### 📄 Lab 2 — Advanced Text Segmentation (5 Levels of Chunking)
> [`Lab2_Chunking_methods/`](./Lab2_Chunking_methods)

A deep dive into how you prepare data for retrieval-augmented AI systems. Covers five progressively smarter ways to split text, from basic character splitting to letting an LLM decide where topics begin and end.

| Level | Method | What It Does |
|-------|--------|-------------|
| 1–2 | Character & Recursive | Basic structural splitting |
| 3 | Document-Specific | Aware of Markdown, Python, JS structure |
| 4 | Semantic | Groups by embedding similarity |
| 5 | Agentic | LLM-driven topic boundary detection |

---

### 📝 Assessment — Self-Reflective Multi-Agent RAG System
> [`Assessment_RAG/`](./Assessment_RAG)

A question-answering system for research papers that goes beyond typical RAG. Instead of a single retrieve-and-generate pass, it uses multiple specialized agents — a planner that breaks complex queries into subtasks, an answer generator, a critic that scores responses, and a revision agent that iterates until quality thresholds are met.

- Multi-agent pipeline: Planner → Retriever → Answerer → Critic → Reviser
- Runs fully locally (no API keys) using FAISS + flan-t5-base
- Streamlit web UI and CLI interface included
- Full details in the [Assessment README](./Assessment_RAG/README.md)

---

## Tech Stack

| Category | Tools |
|----------|-------|
| Frameworks | LangChain, PyTorch, Hugging Face Transformers |
| Models | BLIP, flan-t5-base, all-MiniLM-L6-v2, OpenAI Embeddings |
| Search & Retrieval | FAISS, Scikit-Learn (Cosine Similarity) |
| Interface | Streamlit, Jupyter Notebooks |
| Utilities | PIL, pypdf |

## What This Repo Demonstrates

- **Autonomous reasoning** — AI that plans, retrieves, self-evaluates, and revises instead of giving one-shot answers
- **RAG optimization** — Multiple chunking strategies and retrieval techniques for better context feeding
- **Multimodal adaptation** — Taking a general-purpose vision-language model and specializing it for real use cases
