📚 Research Paper Recommendation System based on Abstract Similarity

📌 Project Overview

This project focuses on developing a Research Paper Recommendation System that suggests academic papers based on abstract similarity. Using advanced Natural Language Processing (NLP) techniques, the system efficiently identifies semantically similar research papers across diverse scientific disciplines.

🚀 System Overview

The system was developed with the following key components:

TF-IDF Baseline Model: Used for initial similarity calculations.

SBERT Embeddings (all-MiniLM-L6-v2): Pre-trained embeddings to enhance semantic similarity.

AllenAI-Specter Embeddings: Used to capture contextual nuances in research abstracts.

Fine-Tuned all-MiniLM-L6-v2: Optimized version of SBERT for improved recommendation accuracy.

LanceDB: A high-performance vector database for efficient similarity search and retrieval.

Retrieval-Augmented Generation (RAG): Integrated with google/flan-t5-large to provide natural language explanations for recommendations.

🗂️ Dataset

Source: ArXiv Metadata Snapshot

Contains 2.6 million research papers across 149 categories.

Stratified sample of 100,000 papers selected to ensure balanced representation.

Preprocessing steps applied:
Combined fields (title, authors, categories, comments, abstracts).

Text normalization (stopword removal, lowercasing, lemmatization).

TF-IDF vectorization & embeddings generation.

📊 Evaluation & Results

The system was evaluated using five scoring methods:

Category-Based Evaluation 🏷️

Clustering-Based Evaluation 📊

Similarity-Based Evaluation 🔎

Temporal Evaluation ⏳

Hybrid Scoring ⚖️

Performance Metrics Used:

Precision@k

Recall@k

Mean Reciprocal Rank (MRR)

🔬 Findings:
AllenAI-Specter embeddings produced the most contextually accurate recommendations.

Fine-tuned all-MiniLM-L6-v2 performed well but was more suitable for specific domains like vehicle-level control and congestion analysis.

Retrieval-Augmented Generation (RAG) enhanced explainability by providing natural language explanations for recommendations.

