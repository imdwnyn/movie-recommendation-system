# 🎬 Movie Recommendation System

## 📌 Overview

This project builds a **content-based movie recommendation system** that suggests movies similar to a given input based on their descriptions, genres, and taglines.

Instead of relying on user ratings, the system analyzes **movie content** to find similarities and generate recommendations.

---

## 🎯 Problem Statement

With thousands of movies available, it becomes difficult for users to decide what to watch next.
This project aims to solve that by recommending movies with similar content to a selected movie.

---

## ⚙️ How the System Works

### 1. Data Preparation

* Load movie metadata dataset
* Select relevant features: `title`, `overview`, `genres`, `tagline`
* Handle missing values and remove duplicates

### 2. Feature Engineering

* Combine multiple text fields into a single **tags** column
* Extract genre names from structured data

### 3. Text Preprocessing

* Convert text to lowercase
* Remove special characters
* Remove stopwords
* Apply lemmatization

### 4. Vectorization

* Convert text into numerical form using **TF-IDF**
* Use unigrams and bigrams to capture context

### 5. Similarity Computation

* Compute similarity using **cosine similarity**
* Identify movies with highest similarity scores

### 6. Recommendation

* Input: Movie title
* Output: Top N similar movies

---

## 🛠️ Tech Stack

* **Python**
* **Pandas, NumPy** → data handling
* **NLTK** → text preprocessing
* **Scikit-learn** → TF-IDF & cosine similarity

---

## 📂 Dataset

* TMDB Movie Metadata Dataset

*(https://www.kaggle.com/datasets/faseeh001/movies-dataset)*

---

## ▶️ How to Run

1. Open the notebook in Google Colab
2. Run all cells
3. Call the recommendation function:

```python
recommend('La La Land')
```

---

## 🎬 Example Output

Input:

```python
recommend('La La Land')
```

Output:

* List of movies similar in theme, genre, and content

---

## 📈 Key Highlights

* End-to-end ML pipeline from raw data to recommendations
* Clean and structured preprocessing workflow
* Efficient similarity computation using vectorization
* Handles missing and noisy data effectively

---

## 🚀 Future Improvements

* Add **collaborative filtering** (user-based recommendations)
* Build a **web app (Streamlit)** for interaction
* Use **advanced embeddings (BERT / Sentence Transformers)**
* Improve ranking using ratings and popularity

---

## 👨‍💻 Author

Dwinayan Deb

---

## ⭐ If you found this useful

Consider giving this repo a star!
