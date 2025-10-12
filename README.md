
# 🛒 Product Recommendation System (ML Project)

An end-to-end **Machine Learning Recommender System** built using Collaborative Filtering (Truncated SVD) and Content-Based Filtering (TF-IDF Similarity) — now enhanced with a Streamlit interactive dashboard, hybrid model blending, and a real-time feedback learning system.
It predicts user preferences and recommends top-N products, similar to Amazon’s recommendation engine.

---

## 📦 Tech Stack
- Python 3.10+
- Pandas, NumPy, Scikit-Learn
- Cloudflare Tunnel (for deployment)
- Matplotlib, Seaborn
- Streamlit (for UI)
- Joblib, Pickle

---

## 🚀 Features
- ✅ Hybrid Recommendation Model (CF + CBF)
- ✅ Dynamic Weight Adjustment — automatically balances CF and CBF weights based on user activity and feedback
- ✅ Feedback Learning System — users can 👍 like / 👎 dislike products directly in the app
- ✅ Explainable Recommendations — every suggestion includes a clear reason (e.g., “Similar to your liked item: Product X”)
- ✅ Interactive Streamlit UI — choose user, number of recommendations, view product cards with reasons and feedback buttons
- ✅ Real-Time Feedback Logging — all user feedback is saved in /models/feedback.csv for continuous learning
- ✅ Undo Functionality — allows users to revert likes/dislikes (session-state based)
---

## 🧠 Model Overview
- **Collaborative Filtering (CF):**
Learns from similar users’ ratings using matrix factorization (TruncatedSVD).

- **Content-Based Filtering (CBF):**
Uses product descriptions with TF-IDF vectorization and cosine similarity to find similar items.

- **Hybrid Recommender:**
Dynamically combines CF and CBF scores using adaptive weights that evolve with user feedback.

- **Feedback Adaptive Learning:**
User interactions (likes/dislikes) influence future recommendations by adjusting model weights in real-time.

---

## 🧮 How It Works

- User selects ID and number of recommendations.
- Hybrid model computes CF and CBF scores for unseen products.
- System blends both scores with adaptive weights (α_CF, α_CBF).
- Explainability module generates textual reasons for each suggestion.
- User feedback (👍 / 👎) is stored in feedback.csv.
- Weights adjust automatically in subsequent sessions.

## 📊 Evaluation Metrics
| Metric | Description |
|---------|--------------|
| RMSE | Measures accuracy of predicted ratings |
| Precision@K | Evaluates recommendation quality |

---

## 💻 Streamlit UI Highlights

- Displays product image, title, category, hybrid score, and explanation
- Shows Why this recommendation? section
- Supports Like / Dislike / Undo buttons with instant UI updates
- Feedback instantly logged and stored persistently
- Automatically adjusts weights and refreshes recommendations
---

## 🧩 Future Improvements

- 🔁 Real-time model retraining using feedback
- 📊 Add dashboard for analytics and user trends
- 🧮 Implement ranking metrics like MAP@K
- ☁️ Deploy using Streamlit Cloud or Hugging Face Spaces


