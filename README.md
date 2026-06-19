# AI Recipe Generator using Retrieval-Augmented Generation (RAG)

## Overview

This project generates recipes from user-provided ingredients using Retrieval-Augmented Generation (RAG).

The system combines semantic retrieval using Sentence Transformers with recipe generation using the Qwen2.5-7B-Instruct Large Language Model.

Users can enter available ingredients and receive context-aware recipes generated in real time.

---

## Architecture

User Ingredients

↓

Ingredient Filtering

↓

SentenceTransformer (all-MiniLM-L6-v2)

↓

Semantic Embeddings

↓

Cosine Similarity

↓

Top-K Recipe Retrieval

↓

Context Construction

↓

Qwen2.5-7B-Instruct

↓

Recipe Generation

↓

Gradio Interface

---

## Technologies Used

* Python
* Pandas
* PyTorch
* Sentence Transformers
* Hugging Face Transformers
* Qwen2.5-7B-Instruct
* Gradio

---

## Features

* Retrieval-Augmented Generation (RAG)
* Semantic Recipe Search
* Cosine Similarity Based Retrieval
* Context-Aware Recipe Generation
* Interactive Gradio Interface

---

## Models Used

### Embedding Model

all-MiniLM-L6-v2

Used to generate semantic embeddings for recipe retrieval.

### Large Language Model

Qwen2.5-7B-Instruct

Used to generate recipes from retrieved context.

---

## Evaluation

Generated recipes were evaluated using cosine similarity between generated outputs and retrieved recipes.

Sample Results:

* Highest Similarity: 0.59
* Average Similarity: 0.56

These scores indicate that generated recipes remain semantically aligned with retrieved recipes while still producing novel content.

---

## Future Improvements

* FAISS Vector Database
* Multi-LLM Comparison
* Nutritional Analysis
* Personalized Recipe Recommendations

---

## Author

Nabeela Javed
