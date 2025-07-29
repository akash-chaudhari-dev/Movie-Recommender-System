# 🎬 Movie Recommender System

A content-based movie recommender system built using Python, pandas, and Streamlit. It recommends movies based on the similarity of their overviews using cosine similarity.

---

## 📁 Project Structure

```

Movie_Reccomender/
├── .venv/                  # Virtual environment
├── data/                   # Raw datasets (e.g., movies metadata)
├── dumpted\_data/           # Precomputed pickle files
│   ├── movies.pkl
│   ├── similarity.pkl
│   └── movie\_dict.pkl
├── app.py                  # Streamlit application
├── model\_genrator.ipynb    # Notebook for data processing and model building
├── requirements.txt        # Project dependencies
├── .gitignore              # Git ignore rules
└── readme.md               # Project documentation

````

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone <your-repo-url>
cd vikas
````

### 2. Create & Activate Virtual Environment (Optional)

```bash
python -m venv .venv
.\.venv\Scripts\activate      # Windows
source .venv/bin/activate     # macOS/Linux
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the App

```bash
streamlit run app.py
```

---

## 🧠 How It Works

* Takes a movie title as input.
* Uses cosine similarity on TF-IDF vectorized movie overviews.
* Returns the top 5 most similar movies based on content.
* Precomputed similarity matrix and movie data are loaded from `.pkl` files for speed.

---

## 📦 Key Components

| File                   | Description                                              |
| ---------------------- | -------------------------------------------------------- |
| `app.py`               | Main Streamlit app                                       |
| `model_genrator.ipynb` | Data cleaning, feature extraction, and model generation  |
| `movies.pkl`           | Filtered movie DataFrame                                 |
| `similarity.pkl`       | Cosine similarity matrix                                 |
| `movie_dict.pkl`       | Dictionary version of movie DataFrame for faster loading |

---

## 🛠 Technologies Used

* Python 3.8+
* pandas
* scikit-learn
* nltk
* streamlit
* pickle

---

## ✍️ Author

Akash — GATE DS & AI aspirant, building projects toward AIR-1.

---

## ✅ Future Improvements

* Integrate TMDB API for movie posters and descriptions
* Use Word2Vec or BERT for context-aware recommendations
* Add genre-based filtering and search