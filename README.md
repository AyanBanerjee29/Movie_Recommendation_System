# 🎬 Movie Recommendation System using Graph Neural Networks

## 📌 Overview

This project implements a **Movie Recommendation System** using **Graph Neural Networks (GNN)** based models such as **Graph Convolutional Network (GCN)** and **LightGCN** on the popular **MovieLens 100K dataset**. The system is designed to predict user preferences and recommend movies by learning user-item interactions from graph structures.

---

## 💡 Problem Statement

Recommender systems aim to suggest items to users based on their interests or past behavior. Traditional models like Matrix Factorization struggle to capture complex relationships between users and items.

By leveraging **Graph Neural Networks**, we represent users and movies as nodes in a bipartite graph and model their interactions through graph convolutions. This approach improves the system’s ability to discover latent connections and deliver accurate, personalized recommendations.

---

## 🗂️ Dataset Description

- **Dataset:** [MovieLens 100K](https://grouplens.org/datasets/movielens/100k/)
- **Files Used:**
  - `u.data`: Contains UserID, MovieID, Rating, Timestamp
  - `u.item`: Contains MovieID and Movie information

**Ratings File Structure (`u.data`):**

- **Total Users:** 943  
- **Total Movies:** 1682  
- **Total Ratings:** 100,000  

---

## 🔍 Model Details

✅ LightGCN
Simplified GCN for recommendation.

Removes non-linear transformations and feature projections.

Learns user and item embeddings directly via message passing.

✅ GCN (Graph Convolutional Network)
Utilizes normalized Laplacian and node feature aggregation.

Captures complex connectivity patterns among nodes.

✅ GAT (Graph Attention Network)
Employs self-attention mechanisms to assign different importance (weights) to neighbor nodes.

Enables the model to focus more on influential neighbors, improving recommendation quality.

Suitable for graphs where relationships among nodes vary in importance.

---

🔮 Future Enhancements

Hyperparameter tuning using grid/random search.

Deployment as a real-time web application using Streamlit or Flask.

Test on larger datasets (MovieLens 1M or 10M)



