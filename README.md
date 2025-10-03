# 🛍️ Mall Customer Segmentation using K-Means Clustering

## 📌 Project Overview
This project is part of **Task 8 of the AI & ML Internship**.  
The objective is to perform **unsupervised learning** using the **K-Means algorithm** to segment mall customers based on their purchasing behavior.

The notebook covers:
- Data loading & preprocessing  
- Feature scaling (Standardization)  
- Elbow Method to find the optimal number of clusters  
- K-Means clustering & cluster assignment  
- Visualization of clusters (2D and PCA projection)  
- Evaluation using **Silhouette Score**  

---

## 🚀 Run in Google Colab
Click below to open and run the notebook in Google Colab:  

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1-CqMtu78iDAFgMA-DmFNHJhpG3CYJW9H?authuser=1#scrollTo=r1k4CCJeSNHS)

---

## 📂 Repository Contents
- `Mall_Customers.csv` → Dataset used for clustering  
- `ClusteringwithKmeans.ipynb` → Main Colab notebook with step-by-step implementation  
- `README.md` → Project documentation  
- `Screenshots` → Cluster visualizations, screenshots (optional)  

---

## 🔎 Steps Performed

1. **Data Exploration**
   - Loaded dataset and examined basic statistics  
   - Visualized distributions of key features: Age, Annual Income, Spending Score

2. **Data Preprocessing**
   - Selected numerical features: `Age`, `Annual Income (k$)`, `Spending Score (1-100)`  
   - Standardized features using `StandardScaler` to bring them to a similar scale  

3. **Finding Optimal Clusters**
   - Applied the **Elbow Method** by plotting inertia vs. number of clusters (K)  
   - Identified **K = 5** as the optimal number of clusters  

4. **Model Training**
   - Trained K-Means with `n_clusters=5`  
   - Assigned each customer to one of the 5 clusters

5. **Evaluation**
   - Calculated **Silhouette Score** to measure clustering performance  

6. **Visualization**
   - Plotted clusters using **Annual Income vs Spending Score**  
   - Used **PCA** to project high-dimensional data into 2D for clear visualization  

---

## 📊 Results

### 📝 Sample of Clustered Data
| CustomerID | Gender | Age | Annual Income (k$) | Spending Score (1-100) | Cluster |
|------------|--------|-----|---------------------|--------------------------|---------|
| 1          | Male   | 19  | 15                  | 39                       | 2       |
| 2          | Male   | 21  | 15                  | 81                       | 2       |
| 3          | Female | 20  | 16                  | 6                        | 3       |
| 4          | Female | 23  | 16                  | 77                       | 2       |
| 5          | Female | 31  | 17                  | 40                       | 2       |

- **Optimal K (Elbow Method):** 5  
- **Silhouette Score:** `0.4084`  

📌 The clusters clearly segment customers into distinct groups based on **income** and **spending patterns**, which can be used for targeted marketing strategies.

---

## 🛠️ Tools & Libraries
- Python 3  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- Google Colab  

---

## 🧾 Key Learnings
- K-Means effectively groups customers based on behavioral patterns  
- The **Elbow Method** helps identify the optimal number of clusters  
- The **Silhouette Score** provides a good measure of cluster quality  
- **PCA** is useful for visualizing high-dimensional clusters in 2D  
- Clustering is **unsupervised**, meaning no predefined labels are needed  

---

👩‍💻 **Author**  
Samruddhee Sapkale  
📅 *October 2025*  
