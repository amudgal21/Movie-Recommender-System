# Movie Recommender System 🎬
CS616A Course Project | Prof. Nisheeth Srivastava | Sept’23 - Oct’23

This project demonstrates a multi-faceted recommendation system for movies using the MovieLens-100K dataset. It combines various recommendation techniques, including collaborative filtering, KNN-based models, and a hybrid approach, to generate personalized movie suggestions for users. The project showcases content-based and popularity-based recommendations, collaborative filtering, and a hybrid model for optimal recommendations.

---

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Features](#features)
- [Implementation](#implementation)
- [Results](#results)
- [Installation](#installation)

---

## 📚 Overview
### Objective
The project aims to design and implement diverse recommendation systems using various methodologies:
- **Genre-Based & Popularity-Based Recommendations**: Utilized cosine similarity and ratings to recommend movies based on genre and popularity for **content based recommendations**.
- **Collaborative Filtering**: Calculated user and item similarity matrices on a subset of the **data (5%) using pairwise distances** for collaborative filtering.
- **K-Nearest Neighbors (KNN) Model**: Calculated user similarities via cosine distance on a **943x1682 sparse matrix** to enhance recommendation relevance.
- **Hybrid Recommendation System**: Combined KNN and content-based recommendations with weighted factors to improve user experience.

---

## 📂 Dataset
The project uses the [MovieLens-100K dataset](https://grouplens.org/datasets/movielens/100k/), which includes:
- **100,000 ratings** from **943 users** on **1,682 movies**.
- Movie details such as **genre**, **popularity**, and **average ratings**.

---

## 🔍 Features
- **Genre-Based Recommendation**: Recommends movies based on genre similarity using cosine similarity.
- **Popularity-Based Recommendation**: Recommends movies based on high ratings and frequency.
- **Collaborative Filtering**: Computes user and item similarities using pairwise distances on a 5% subset of data.
- **KNN for Similar Users**: Uses KNN with cosine distance on a sparse 943x1682 matrix for user similarity, yielding recommendations based on similar users.
- **Hybrid Recommendation System**: Combines KNN and content-based recommendations by weighting genre, popularity, and user preferences for a balanced recommendation list.

---

## 🛠 Implementation

### 1. Data Preprocessing
- **Data Cleaning**: Merges and refines the dataset for efficient processing.
- **Matrix Creation**: Transforms data into a sparse matrix format for memory efficiency.

### 2. Genre-Based & Popularity-Based Recommendation
- **Cosine Similarity and Ratings**: Utilizes cosine similarity on genre features and average ratings for content-based and popularity-based recommendations.

### 3. Collaborative Filtering
- **User and Item Similarity Matrices**: Constructs similarity matrices using pairwise distances on a subset of the data.
- **User-Item Interaction Matrix**: Builds a user-item matrix to calculate similarity and provide collaborative recommendations.

### 4. K-Nearest Neighbors (KNN) Model
- **Model Training**: Trains the KNN model using cosine distance on a 943x1682 sparse matrix for item-based recommendations.
- **Similarity Threshold**: Sets a threshold to limit recommendations to those with high similarity scores for relevant suggestions.

### 5. Hybrid Recommendation System
- **Combining KNN & Content-Based Recommendations**: Merges genre, popularity, and user ratings by applying weighted factors.
- **Weighted Recommendation**: Configurable weights for each recommendation type ensure a balanced list based on user preference.

### 6. Evaluation (RMSE)
- **RMSE Calculation**: Measures performance on both test and train data using RMSE (Root Mean Square Error).
- **Results**: Error metrics help fine-tune model performance.

---

## 📊 Results
The hybrid recommendation system achieved better user experience by balancing the strengths of collaborative filtering and content-based filtering. Key findings include:
- **Improved User Similarity with KNN**: KNN model with cosine distance provided effective user similarity metrics on the sparse matrix.
- **Diverse Recommendations via Content & Popularity-Based Filtering**: Content and popularity-based filtering added variety to the recommendation pool.
- **Hybrid System Optimization**: Weighted factors for genre, popularity, and user ratings in the hybrid system yielded a personalized recommendation list.

---

## ⚙️ Installation

### Clone the Repository
```bash
git clone https://github.com/amudgal21/Movie-Recommender-System.git
