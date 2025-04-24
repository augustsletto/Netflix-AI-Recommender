# Netflix-AI-Movie-Recommender
A simple yet powerful content-based movie recommendation engine using LLaMA2 for embeddings and FAISS for fast similarity search on the Netflix dataset.


# 🎬 Netflix AI Movie Recommender

A content-based recommendation system that uses [Meta's LLaMA2](https://ai.meta.com/llama/) model to generate text embeddings of Netflix titles, and [FAISS](https://github.com/facebookresearch/faiss) for fast similarity search.

This project turns Netflix metadata into rich textual descriptions, encodes them with LLaMA2, and lets you search for similar shows or movies based on your favorite title.

## 🔧 Features

- Parses Netflix metadata from CSV
- Uses Open Source LLaMA2 for embedding generation
- Stores embeddings with FAISS (Facebook AI Similarity Search)
- Given a favorite movie, finds the most similar titles

## 🧠 How it Works

1. Netflix titles are turned into detailed natural language descriptions.
2. These descriptions are passed through LLaMA2's embedding API.
3. The high-dimensional vectors are indexed with FAISS for similarity comparison.
4. A chosen favorite title is encoded, and its top-5 most similar matches are returned.

## 📦 Requirements

- Python 3.8+
- pandas
- numpy
- faiss-cpu
- requests
- LLaMA2 API running locally (e.g. Ollama)

