# 🎵 Multi-Modality in Music: Predicting Emotion from Audio and Lyrics

This repository archives and summarizes the paper **"Multi-Modality in Music: Predicting Emotion in Music from High-Level Audio Features and Lyrics"** by Tibor Krols, Yana Nikolova, and Ninell Oldenburg (University of Copenhagen).

The paper explores the effectiveness of **multimodal music emotion recognition (MER)** by combining high-level audio features retrieved from the Spotify API with lyrics-based features such as **VADER sentiment scores** and **TF-IDF vectors**. The aim is to predict **valence** and **arousal** scores using machine learning models.

---

## 📄 Included

- Descriptions of dataset and features
- Experimental setup and results from 4 regression models
- Comparative performance of uni-modal vs multi-modal approaches

---

## 🎯 Key Findings

- **Multimodal models** outperform unimodal models when predicting **valence**.
- **Lyrics features alone** are poor predictors of **arousal**.
- Selected Spotify audio features (e.g., `danceability`, `energy`) contribute strongly to prediction accuracy.
- Simple MLR models achieved performance competitive with deep learning baselines.

---

## 🧠 Techniques Used

- Feature engineering: Spotify high-level audio features, VADER sentiment analysis, TF-IDF + PCA
- Regression models: `LinearRegression`, `RandomForestRegressor`, `SVR`, `MLPRegressor` (from `scikit-learn`)
- Model evaluation using **R² scores** for valence and arousal prediction

---

## 📊 Dataset

- **Deezer Mood Detection Dataset (DMDD)** (18,644 songs with valence/arousal scores)
- Lyrics scraped from Genius.com
- Spotify features retrieved via [Spotify Web API](https://developer.spotify.com/documentation/web-api/)

---


