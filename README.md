# 🎬 Movie Recommendation System

A movie discovery web application that helps users explore movies, search by title or keyword, view movie details, and discover recommendations through an interactive interface.

## Features

- **Movie Discovery:** Browse trending and categorized movie collections.
- **Search:** Find movies using titles or keywords.
- **Movie Details:** Explore individual movies through dedicated detail views.
- **Recommendations:** Discover related movies.
- **Interactive UI:** Browse movie posters and results using Streamlit.
- **REST API:** Backend services powered by FastAPI.

## Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core application logic |
| FastAPI | Backend API |
| Streamlit | Interactive web interface |
| Scikit-learn | Machine learning and text processing |
| Pandas & NumPy | Data processing |
| TMDB API | Movie metadata and information |

## Project Structure

```text
movie-recommendation-system/
├── app.py
├── main.py
├── movies.ipynb
├── movies_metadata.csv
├── requirements.txt
├── runtime.txt
├── df.pkl
├── indices.pkl
├── tfidf.pkl
├── tfidf_matrix.pkl
└── README.md
```

## Getting Started

### Prerequisites

- Python 3.12
- Git
- TMDB API key

### 1. Clone the repository

```bash
git clone https://github.com/jintumahanta/movie-recommendation-system.git
cd movie-recommendation-system
```

### 2. Create and activate a virtual environment

**Windows:**

```bash
py -3.12 -m venv .venv
.venv\Scripts\activate
```

### 3. Install dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Configure the API key

Create a `.env` file in the project root:

```env
TMDB_API_KEY=your_tmdb_api_key
```

Replace the placeholder with your own API key. Keep `.env` private and never commit it to GitHub.

### 5. Run the backend

Open a terminal in the project directory:

```bash
uvicorn main:app --reload
```

API documentation: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

### 6. Run the frontend

Open a second terminal:

```bash
.venv\Scripts\activate
streamlit run app.py
```

Open the local URL displayed in the terminal, usually [http://localhost:8501](http://localhost:8501).

Keep both services running while using the application.

## Future Enhancements

- Improve recommendation relevance and search functionality.
- Evaluate recommendation quality using suitable metrics.
- Add automated tests and improve error handling.
- Deploy the application for public access.

## License

Check the licenses of the source code, datasets, and third-party services before redistributing them.
