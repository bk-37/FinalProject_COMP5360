# Spotify Song Recommendation System (4100 Project)

## 🎧 Overview
This project explores the development of a song recommendation system based solely on audio features and genre clustering, rather than personalized user behavior. Our goal was to evaluate whether music can be effectively recommended using **unsupervised learning (KMeans clustering)** and **nearest neighbor search**, using a large public dataset of Spotify tracks.

This project was developed for a Data Science course (COMP 5360) at the University of Utah.

---

## 💡 Motivation
Spotify’s existing recommendation system is highly personalized, factoring in user behavior, demographics, and preferences. However, not all users are satisfied with it. Our group explored whether recommendations made *only* from acoustic features like tempo, danceability, and energy — without personalization — could still be effective.

We were curious:  
> Are Spotify’s recommendations overfitting to our habits?  
> Can a content-only system broaden users' discovery?

---

## 📊 Dataset
- **Source**: [Spotify Dataset on Kaggle](https://www.kaggle.com/datasets/vatsalmavani/spotify-dataset)  
- ~171,000 songs, each with 17+ features such as:
  - `valence`, `acousticness`, `danceability`, `energy`, `tempo`, `popularity`, `explicit`, `genre`
- Categorical features like `artist`, `genre`, and `explicit` were cleaned and preprocessed for clustering.

---

## 🔧 Methods & Tools
- **Data Preprocessing**:
  - Handled missing values
  - Removed duplicates
  - Scaled numerical features
  - Dropped non-essential columns for clustering (`name`, `artist`, `id`)
- **Exploratory Data Analysis**:
  - Correlation heatmaps
  - Elbow and Silhouette method to determine optimal `k`
- **Machine Learning**:
  - `KMeans` clustering
  - `KNN` (within-cluster) for song recommendation
- **Visualization**:
  - PCA plots of clustered data
  - Cluster centroids and spread
  - Survey response visualization
- **Libraries Used**: pandas, NumPy, scikit-learn, matplotlib

---

## 🎯 Objectives
1. Can we recommend songs effectively using only acoustic features?
2. Which features most strongly inform recommendation clusters?
3. How does satisfaction with our system compare to Spotify's?

---

## 🧪 Evaluation
- Recommendations were tested via user surveys
- Participants rated familiarity and enjoyment of recommended songs
- Results were compared to Spotify’s baseline satisfaction scores (65% user satisfaction from existing studies)

---

## 🔐 Ethical Considerations
- Possible biases against niche artists or non-Western genres
- Transparent use of data (Spotify ToS and Kaggle licensing respected)
- Stakeholders: users, artists, streaming platforms, and researchers

---

## 📅 Timeline Summary
| Week | Focus |
|------|-------|
| Week 1 | Data cleaning, EDA, initial preprocessing |
| Week 2 | Feature selection, dimensionality reduction, clustering |
| Week 3 | KNN song recommendation and similarity metrics |
| Week 4 | Survey creation, data collection, user feedback |
| Week 5 | Final analysis, results summary, and visualization |

---

## ✍️ Authors
- **Brian Keller**
- **Tyler Adamson** 
- **Wyatt Young**
- University of Utah | Department of Biomedical Engineering 

---

## 📌 License
For educational purposes only. Dataset used under Kaggle’s and Spotify API's permissible use policies.
