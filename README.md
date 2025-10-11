
# 🛒 Product Recommendation System (ML Project)

An end-to-end **Machine Learning Recommender System** built using Collaborative Filtering (Truncated SVD) and Content-Based Filtering (TF-IDF Similarity).  
It predicts user preferences and recommends top N products, similar to Amazon’s recommendation engine.

---

## 📦 Tech Stack
- Python 3.10+
- Pandas, NumPy, Scikit-Learn
- Matplotlib, Seaborn
- Streamlit (for UI)
- Joblib, Pickle

---

## 🚀 Features
✅ Synthetic or real Amazon review dataset  
✅ Data preprocessing & EDA  
✅ Collaborative Filtering (Matrix Factorization)  
✅ Content-Based Filtering (TF-IDF + Cosine Similarity)  
✅ Evaluation (RMSE, Precision@K)  
✅ Visualization of top products and rating distribution  
✅ Interactive Streamlit web app for recommendations  

---

## 🧠 Model Overview
- **Collaborative Filtering (CF):** Uses `TruncatedSVD` to learn latent factors from the user-item matrix.
- **Content-Based Filtering (CBF):** Computes TF-IDF vectors for product descriptions and uses cosine similarity.
- **Hybrid Recommendation:** Combines top results from both models.

---

## 📊 Evaluation Metrics
| Metric | Description |
|---------|--------------|
| RMSE | Measures accuracy of predicted ratings |
| Precision@K | Evaluates recommendation quality |

---

## 🧩 Folder Structure
