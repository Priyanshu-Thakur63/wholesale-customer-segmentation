# 🛍️ Wholesale Customer Segmentation using K-Means Clustering

This project performs customer segmentation using **K-Means Clustering** on wholesale spending data. It groups customers based on annual spending patterns across six product categories. The model also includes an interactive tool for **real-time cluster prediction** based on new input.

---

## 📌 Problem Statement

Wholesale businesses often serve a mix of customer types — from small restaurants to large retailers — each with unique purchasing patterns. This project uses clustering to identify **four distinct customer groups** using their annual spending. An interactive predictor helps classify new customers into these groups.

---

## 📂 Dataset

- **Source**: [Kaggle – Wholesale Customer Purchasing Behavior](https://www.kaggle.com/code/saurabhbadole/wholesale-customer-purchasing-behavior/input)
- **Original Provider**: UCI Machine Learning Repository  
- **Features Used**:
  - `Fresh`, `Milk`, `Grocery`, `Frozen`, `Detergents_Paper`, `Delicassen`
- **Learning Type**: Unsupervised learning (no labels)

---

## 🚀 Project Workflow

1. **Data Loading & Preparation**:
   - Loaded CSV file with wholesale customer data
   - Selected 6 spending features for analysis

2. **Preprocessing**:
   - Standardized the data using `StandardScaler` to normalize scale

3. **Elbow Method**:
   - Ran KMeans for `k = 1 to 10` and plotted WCSS
   - Chose **4 clusters** using the elbow point

4. **Modeling with KMeans**:
   - Trained KMeans on scaled data
   - Assigned cluster labels to original dataset

5. **Visualization**:
   - Plotted **Elbow Curve** to determine best `k`
   - Plotted **Milk vs Grocery scatter** with cluster color mapping

6. **Cluster Profiling**:
   - Inverse-transformed cluster centers to interpret real-world spending
   - Printed distribution and average behavior per cluster

7. **Interactive Prediction**:
   - Accepts new customer inputs via console
   - Predicts the cluster they belong to
   - Displays the spending profile of that cluster

---

## 📊 Key Insights

- Cluster 0: High spending on Milk and Grocery — potential **retailers**
- Cluster 1: Higher Fresh and Frozen — likely **restaurants or cafes**
- Other clusters vary in Detergents_Paper and Delicassen usage
- Real-time prediction helps quickly categorize new customers

---

## 🛠️ Technologies Used

| Tool | Purpose |
|------|---------|
| Python | Core programming language |
| Jupyter Notebook | Development environment |
| pandas / numpy | Data handling |
| matplotlib | Visualization |
| scikit-learn | Machine learning (clustering, scaling) |

---

## 📁 Files Included

| File Name | Description |
|-----------|-------------|
| `customer_segmentation.ipynb` | Main notebook with full analysis |
| `Wholesale customers data.csv` | Dataset used in the project |
| `README.md` | Project overview and guide |

---

## 💬 How to Use the Predictor

Once the notebook runs, Enter the values and get the prediction:

