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
-Top Hybrid Recommendations for User 1:

1.Rosencrantz and Guildenstern Are Dead (1990)
2.The General (1926)
3.Spartacus (1960)
4.Now You See Me (2013)
 ...

 
➡️ Full output available in: `results.txt` :contentReference[oaicite:6]{index=6}  

---

## ⚙️ Installation

```bash
pip install pandas numpy scikit-learn scipy matplotlib


```

## ▶️ Run the Project
    ```bash
    python main.py


  ```

## 📊 Evaluation Metrics

   1. Precision@K
   2.Recall@K
   3.F1-score

   The hybrid model shows improved performance compared to individual models.


  ```

## 🎯 Applications

  Movie streaming platforms
  Personalized recommendation systems
  E-commerce recommendation engines


```

## 🤝 Acknowledgement

   Dataset provided by GroupLens Research (MovieLens)

```

## 👩‍💻 Author
      TITLI BISWAS

  ```

 ## ⭐ Support

   If you like this project, give it a ⭐ on GitHub!

