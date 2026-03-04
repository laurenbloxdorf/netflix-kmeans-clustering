# Netflix Content Clustering with KMeans

An unsupervised machine learning project that clusters Netflix titles by genre, rating, and duration and uses those clusters to power a content recommendation engine.

---

## Overview

This project applies **KMeans clustering** to the Netflix dataset to discover natural groupings of content. After clustering, a **cosine similarity recommender** suggests similar titles from within the same cluster based on any movie or show you input.

---

## Techniques Used

- **KMeans Clustering** — unsupervised grouping of Netflix titles
- **Elbow Method + Silhouette Score** — to select the optimal number of clusters
- **PCA (Principal Component Analysis)** — to visualize high-dimensional clusters in 2D
- **Multi-Label Binarization** — to encode multi-genre tags
- **Cosine Similarity** — to rank recommendations within a cluster
- **Google Colab form UI** — interactive title input and slider

---

## Features

- Encodes genre, rating, and duration into a unified feature matrix
- Determines optimal k using both WCSS and silhouette score
- Visualizes clusters with a labeled PCA scatter plot
- Profiles each cluster by its top genres, average duration, and most common rating
- Interactive recommender: type any Netflix title → get the 10 most similar titles

---

## Dataset

[Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows) via Kaggle  
~8,800 titles with genre, rating, duration, cast, and description.

---

## How to Run

1. Open the notebook in **Google Colab**
2. Run all cells in order
3. In the last cell, type any Netflix title into the form and hit ▶

> No local setup needed — the dataset downloads automatically via `kagglehub`.

---

## Files

| File | Description |
|------|-------------|
| `Netflix_KMeans_Portfolio.ipynb` | Main notebook with clustering + recommender |

---

## 🛠️ Libraries

`pandas` `numpy` `scikit-learn` `matplotlib` `kagglehub`
