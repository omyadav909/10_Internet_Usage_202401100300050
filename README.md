# 📊 Internet Usage Clustering

This project applies **unsupervised machine learning** to analyze and cluster users based on their internet usage patterns. By utilizing features such as **daily device usage**, **site categories visited**, and **frequency of sessions**, we identify behavior-based user groups for better insights and decision-making.

---

## 🧠 Problem Statement

To segment users into distinct behavioral clusters using internet activity data. This can support applications like:

- Personalized content recommendations  
- Network performance optimization  
- User profiling and digital wellbeing analysis

---

## 🎯 Objectives

- Preprocess and normalize internet usage data
- Use the Elbow Method to determine the optimal number of clusters
- Apply **KMeans clustering** to group similar users
- Visualize clusters for interpretability
- Analyze cluster centers to profile user behavior

---

## 📂 Dataset

The dataset (`internet_usage.csv`) contains the following features per user:
- `daily_usage_hours`: Total hours online per day
- `sessions_per_day`: Number of browsing sessions per day
- `site_category_counts`: Visits to categories like social media, entertainment, education, etc.

> _Note: Replace this with actual columns if different._

---

## 🛠️ Tech Stack

- Python 3  
- pandas  
- scikit-learn  
- seaborn  
- matplotlib

---

## 🔄 Workflow

### 1. Load & Preprocess
- Handle missing values
- Normalize numeric features using `StandardScaler`

### 2. Determine Clusters
- Use the **Elbow Method** to choose optimal `k`
- Visualize inertia vs. `k`

### 3. Apply KMeans
- Fit KMeans with selected number of clusters
- Assign each user to a cluster

### 4. Visualize & Analyze
- Scatter plot clusters based on usage metrics
- Analyze cluster centers in original scale

---

## 📈 Visualizations

- **Elbow Curve**: Helps select optimal number of clusters
- **Scatter Plot**: Displays user clusters by usage patterns
- **Heatmap**: Optionally show feature correlation or user behavior density

---

## ✅ Results

- Identified 3 key user groups:
  - Light Users (low time, low frequency)
  - Moderate Users (balanced usage)
  - Heavy Users (high time, frequent sessions)
  Cluster Centers:
   daily_usage_hours  sessions_per_day  social_media_visits  entertainment_visits  education_visits
0               1.85              2.31                  5.40                  2.18              0.94
1               4.52              4.85                  8.67                  5.33              1.52
2               7.20              7.14                 12.93                  9.50              2.34


![Screenshot 2025-04-22 113324](https://github.com/user-attachments/assets/2483523f-6fbc-4517-873f-508b9eceedf4)


