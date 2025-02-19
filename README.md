# 📚 Research Paper Recommendation System based on Abstract Similarity    

## 🏆 Project Overview  

Finding relevant academic papers is challenging with the **ever-growing volume of research**. This system **solves** that problem by providing **accurate and context-aware recommendations** based on **abstract similarity**.  

✅ **Natural Language Processing (NLP) based recommendations**  
✅ **State-of-the-art Embeddings (SBERT, AllenAI-Specter, TF-IDF)**  
✅ **Fast retrieval with LanceDB for large datasets**  
✅ **Explainability with RAG (Retrieval-Augmented Generation)**  


---

## 🚀 Key Features  

- **🔹 Abstract Similarity Matching** - Finds the most relevant papers based on **semantic similarity**.  
- **🔹 Hybrid Scoring Mechanism** - Considers **category, similarity, clustering, and temporal relevance**.  
- **🔹 Fast & Scalable Retrieval** - Uses **LanceDB** to store and query high-dimensional embeddings efficiently.  
- **🔹 Explainable AI** - **Google FLAN-T5** generates **human-readable explanations** for recommendations.  
- **🔹 Support for Large-Scale Datasets** - Handles **millions of research papers** effectively.  


## 🏗️ System Architecture  

### 🛠 **Technologies Used**  
- **Python 3.8+**
- **Hugging Face Transformers** (SBERT, AllenAI-Specter, FLAN-T5)
- **LanceDB** (Vector storage & retrieval)
- **Scikit-learn** (TF-IDF, Clustering)
- **Streamlit** (User Interface)

### 🔍 **How it Works**
1. **User inputs an abstract**.
2. **Preprocessing:** Cleaning & feature extraction.
3. **Embedding Generation:** Using **TF-IDF, SBERT, or AllenAI-Specter**.
4. **Similarity Matching:** Finds the closest abstracts using **cosine similarity**.
5. **Hybrid Scoring:** Adjusts ranking based on **category, clustering, and temporal relevance**.
6. **RAG Explainability:** Generates **human-like explanations** for recommendations.
7. **Results Displayed!** 🎉  


## 📊 Dataset Details  

📖 **Source:** [ArXiv Metadata Snapshot](https://www.kaggle.com/datasets/Cornell-University/arxiv)  
📝 **Size:** 2.6M+ research papers across 149 categories  
📊 **Filtered Sample:** ~100,000 papers for high relevance  
🔍 **Fields Used:**  
- **Title, Authors, Categories, Abstract, Publication Date**  

🛠 **Preprocessing Steps:**  
- **Stratified Sampling** to ensure category balance.  
- **Text Cleaning** (stopword removal, lowercasing, lemmatization).  
- **TF-IDF and Embedding Generation** for accurate recommendations.  


## 📈 Performance & Evaluation  

### ✅ **Evaluation Methods:**  
✔ **Category Matching** - Measures how well recommendations match the input category.  
✔ **Clustering-Based Similarity** - Uses **K-Means clustering** for grouping similar papers.  
✔ **Temporal Relevance** - Prioritizes **recent** publications.  
✔ **Hybrid Scoring** - Combines multiple factors for best recommendations.  

### 📊 **Metrics Used:**  
- **Precision@k**  
- **Recall@k**  
- **Mean Reciprocal Rank (MRR)**  

### 🏆 **Key Findings:**  
📌 **AllenAI-Specter embeddings** delivered the **most accurate recommendations**.  
📌 **Fine-tuned SBERT** performed well but was **task-specific**.  
📌 **TF-IDF Baseline** provided quick results but lacked deep semantic understanding.  