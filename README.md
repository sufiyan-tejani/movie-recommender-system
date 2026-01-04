# Content-Based Movie Recommendation System using NLP

---

**Live Demo (Streamlit App):** https://sufiyan-tejani-movie-recommender-system-app-xuosxi.streamlit.app/ 

## Overview
This project implements a **content-based movie recommendation system** that suggests similar movies based on textual metadata such as genres, keywords, cast, and overview. Natural Language Processing (NLP) techniques are used to convert text data into numerical representations, enabling similarity-based recommendations.

The system is deployed as an interactive web application that allows users to select a movie and receive personalized recommendations in real time.

---

## Objective
To design and deploy a content-based recommendation engine that leverages NLP and cosine similarity to provide accurate movie recommendations.

---

## Project Workflow
1. Data collection and cleaning  
2. Text preprocessing and feature extraction  
3. Vectorization using NLP techniques  
4. Similarity computation  
5. Recommendation logic implementation  
6. Model serialization  
7. Deployment using Streamlit  

---

## Dataset
- **Type:** Structured movie metadata  
- **Features:** Movie title, genres, keywords, cast, crew, overview  
- **Source:** Movie metadata dataset (CSV format)

---

## Data Preprocessing
- Handled missing and inconsistent values  
- Merged multiple textual features into a single representation  
- Applied text normalization and tokenization  
- Removed irrelevant and redundant information  

---

## Natural Language Processing (NLP)
- Converted text data into numerical vectors using **CountVectorizer**  
- Limited vocabulary size to reduce dimensionality  
- Removed common stopwords to improve feature quality  

---

## Recommendation Technique
- Computed **cosine similarity** between movie vectors  
- Implemented similarity-based ranking to recommend top N similar movies  
- Ensured efficient lookup using precomputed similarity matrix  

---

## Model Artifacts
- `movie_dict.pkl` – Serialized movie metadata dictionary  
- `similarity.pkl` – Precomputed cosine similarity matrix  

These artifacts ensure fast inference without recomputing features at runtime.

---

## Deployment
- Built an interactive **Streamlit web application**  
- Users can select a movie title from a dropdown menu  
- The app returns top recommended movies based on content similarity  

---

## Project Structure
├── movie_recommendation.ipynb # Data preprocessing, NLP, and similarity computation
├── movies.csv # Movie metadata dataset
├── movie_dict.pkl # Serialized movie dictionary
├── similarity.pkl # Precomputed similarity matrix
├── app.py # Streamlit web application
├── requirements.txt # Project dependencies
├── README.md # Project documentation

yaml
Copy code

---

## Tech Stack
- **Programming Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, NLTK  
- **NLP Techniques:** CountVectorizer, Cosine Similarity  
- **Deployment:** Streamlit  
- **Tools:** Git, GitHub, Jupyter Notebook  

---

## Key Learnings
- Applying NLP techniques to real-world recommendation systems  
- Feature engineering for textual data  
- Efficient similarity computation and storage  
- Deploying data-driven applications with Streamlit  

---

## Future Improvements
- Implement TF-IDF vectorization for better recommendations  
- Add movie posters using external APIs  
- Incorporate user-based or hybrid recommendation techniques  
- Improve recommendations using word embeddings  

---

## Author
**Sufiyan Ashraf Tejani**  
M.Sc. Mathematics, IIT Kharagpur  

---
