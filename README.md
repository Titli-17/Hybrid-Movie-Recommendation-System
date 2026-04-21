# 🎬 Hybrid Movie Recommendation System

## 📌 Overview
This project implements a **Hybrid Movie Recommendation System** that combines **Content-Based Filtering** and **Collaborative Filtering (KNN)** to provide accurate and personalized movie recommendations.

The system uses **TF-IDF vectorization and cosine similarity** for content-based filtering and **K-Nearest Neighbors (KNN)** for collaborative filtering. A weighted hybrid approach integrates both models to improve recommendation performance.

---

## 🚀 Features
- Hybrid recommendation (Content + Collaborative)
- TF-IDF based feature extraction
- Cosine similarity for movie similarity
- KNN-based collaborative filtering (no SVD)
- User-based and item-based recommendations
- Data preprocessing and cleaning pipeline
- Evaluation using Precision, Recall, and F1-score

---

## 🧠 Methodology

### 🔹 Data Preprocessing
- Handling missing values
- Removing duplicates
- Merging datasets
- Text preprocessing (title + genres)

➡️ Implemented in: `data_preprocessing.py` :contentReference[oaicite:0]{index=0}  

---

### 🔹 Content-Based Filtering
- TF-IDF vectorization on movie features
- Cosine similarity for recommendation

➡️ Implemented in: `content_based.py` :contentReference[oaicite:1]{index=1}  

---

### 🔹 Collaborative Filtering
- User-item matrix creation
- KNN algorithm (cosine similarity)
- User-based & item-based recommendations

➡️ Implemented in: `collaborative_filtering.py` :contentReference[oaicite:2]{index=2}  

---

### 🔹 Hybrid Model
- Normalization of scores
- Weighted combination:
  
  Hybrid Score = 0.4 × Content + 0.6 × Collaborative

➡️ Implemented in: `hybrid_recommender.py` :contentReference[oaicite:3]{index=3}  

---

### 🔹 Pipeline Execution
➡️ Main file: `main.py` :contentReference[oaicite:4]{index=4}  

---

## 📊 Dataset
- MovieLens (ml-latest-small)
- 9742 movies
- 100,836 ratings
- 610 users :contentReference[oaicite:5]{index=5}  

---

## 📈 Sample Output
