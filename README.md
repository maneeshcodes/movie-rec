# 🎬 Movie Recommendation System

A full-stack movie recommendation system that helps users discover movies they’ll love using **content-based filtering**, **TF-IDF similarity**, and **genre-based recommendations** — powered by a FastAPI backend and a Streamlit UI.

---

## 🚀 Live Demo

- **Frontend (Streamlit):** https://movie-rec-gan7fcdzylskgcfjzsmy.streamlit.app  
- **Backend API (FastAPI):** https://movie-rec-g56g.onrender.com/docs

---

## 🧠 Features

- 🔍 **Search movies by keyword** with live suggestions
- 🎭 **Genre-based recommendations**
- 📊 **TF-IDF content-based similarity recommendations**
- 🏠 **Home feed** (Trending, Popular, Top Rated, Upcoming, Now Playing)
- 📄 **Detailed movie pages** with overview, genres, posters & backdrop
- ⚡ Fast API responses with caching
- 🌐 Deployed backend + frontend

---

## 🛠️ Tech Stack

### Backend
- **Python**
- **FastAPI**
- **Pandas, NumPy**
- **Scikit-learn (TF-IDF)**
- **TMDB API**
- **Render (Deployment)**

### Frontend
- **Streamlit**
- **Requests**
- **Modern UI with custom CSS**

---

## 🧩 How It Works

1. **Movie data preprocessing**
   - Cleaned metadata (genres, overview, titles)
   - Vectorized text using **TF-IDF**

2. **Recommendation logic**
   - TF-IDF cosine similarity for content-based recommendations
   - Genre-based fallback recommendations

3. **API layer**
   - FastAPI exposes endpoints for search, details, and recommendations

4. **UI layer**
   - Streamlit app consumes backend APIs and renders an interactive UI

---

## 📡 API Endpoints (Backend)

| Method | Endpoint | Description |
|------|---------|-------------|
| GET | `/health` | Health check |
| GET | `/home` | Home feed movies |
| GET | `/tmdb/search` | Search movies |
| GET | `/movie/id/{tmdb_id}` | Movie details |
| GET | `/recommend/genre` | Genre recommendations |
| GET | `/recommend/tfidf` | TF-IDF recommendations |
| GET | `/movie/search` | Combined recommendations |

---

## ▶️ Run Locally

### 1️⃣ Clone the repository
```bash
git clone https://github.com/maneeshcodes/movie-rec.git
cd movie-rec
