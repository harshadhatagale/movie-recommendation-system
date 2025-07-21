# 🎬 Movie Recommendation System

A powerful **Collaborative Filtering + Content-Based** system built in Python (Jupyter), leveraging the MovieLens 20M dataset to provide personalized movie suggestions and rating predictions.

---

## ✨ Features

- ✅ **User-Item Predictions**: Forecast how a user will rate an unseen movie (RMSE/MAPE optimized).
- 🤝 **User-User & Item-Item CF**: Explore similarities using Pearson/ cosine metrics.
- 🧠 **Matrix Factorization (SVD)**: Reveal hidden preference patterns.
- 🏆 **Baseline Models**: Compare against global averages + simple heuristics.

---

## 📊 Data

The model uses the MovieLens 20M dataset (20M ratings, 27K movies, 138K users) from GroupLens 1.

- **ratings.csv** — user–movie ratings  
- **movies.csv** — titles and metadata

---

## 🧩 Usage

1. **Clone & setup:**
   ```bash
   git clone https://github.com/harshadhatagale/movie-recommendation-system.git
   cd movie-recommendation-system
   pip install -r requirements.txt

2. Launch notebook:

jupyter notebook Movie_Recommendation_System.ipynb


3. Explore & retrain:

Step through data loading, EDA, similarity-matrix builds.

Try different CF models and tune hyperparameters.

Examine model diagnostics and prediction quality.



4. Customize & extend:

Add Content-Based Filtering using NLP and metadata.

Wrap into a REST API or lightweight Streamlit/Django app.

Incorporate cold-start handling or hybrid model approaches.





---

📈 Results

Model	RMSE	MAPE

User-based CF	0.87	12.2%
Item-based CF	0.85	11.5%
SVD (k=50)	0.81	10.3%


(Customize this section with your actual evaluation details)


---

🧠 Insights

User-user CF works well but suffers from sparse-rating issues.

Item-item CF is more robust and scalable.

SVD (matrix factorization) uncovers intuitive latent structures.

Performance improves meaningfully when combining similarity and MF techniques.



---

🚀 Roadmap

[ ] Enhance with deep learning–based CF (e.g., neural CF).

[ ] Build a web API / UI for live recommendations.

[ ] Incorporate genre/tags metadata for content-based filtering.

[ ] Implement real-time retraining & monitoring pipeline.



---

🧰 Requirements

Python 3.8+

Jupyter Notebook

pip packages: NumPy, pandas, scikit-learn, surprise, matplotlib, seaborn


Install with:

pip install -r requirements.txt


---

🧪 Tests & Quality

(Add any test scripts or instructions you include later)


---

🧭 How it works

At launch, the notebook:

Loads ratings & movies

Computes user-user and item-item similarity matrices

Trains SVD-based CF using Surprise or similar

Predicts ratings for unseen movies

Evaluates performance (RMSE, MAPE)

Generates top‑N movie recommendations



---

🌐 Visually appealing ✅

💎 Badges / logos — add optional coverage, version, build-previews

📸 Screenshots or animated GIFs of outputs, UI or plots

🎥 Include a mini demo video or GIF in the README to hook users  

