# Customer Segmentation Using KMeans Clustering
This project applies unsupervised machine learning techniques to identify distinct customer groups based on demographic and behavioral data. It uses KMeans clustering to discover segments and visualizes them using PCA.

## Features
- Clustering with KMeans
- Elbow Method & Silhouette Score for optimal cluster selection
- PCA-based 2D visualization of clusters
- Cluster profile analysis (e.g., age, income, spending behavior)
- Naming of clusters based on interpreted behavioral patterns
- Classification model to predict cluster membership for new customers

## Dataset
## 📁 Dataset

The dataset used in this project is the [Mall Customer Segmentation Data](https://www.kaggle.com/datasets/shwetabh123/mall-customers) from Kaggle.

It contains basic customer information:
- CustomerID
- Gender
- Age  
- Annual Income (k$)  
- Spending Score (1–100)
 
### Additional Columns Created:
As part of this project, the following new columns were added through analysis and modeling:
- `Cluster`: Cluster ID assigned using KMeans
- `Segment Name`: Descriptive label for each cluster (e.g., *Affluent Big Spenders*)
- `Predicted Cluster`: Output from a classification model for new customer inputs
These enhancements support customer profiling, prediction, and business insights.

## Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Seaborn, Matplotlib

## Cluster Segments
| Cluster ID | Segment Name             | Description                                                   |
|------------|--------------------------|---------------------------------------------------------------|
| 0          | Sensible Seniors         | Older adults with moderate income and moderate spending       |
| 1          | Affluent Big Spenders    | High-income, high-spending middle-aged individuals            |
| 2          | Young Value Shoppers     | Young customers with low income but high spending             |
| 3          | Young Professionals      | Young adults with balanced income and spending                |
| 4          | Wealthy Minimalists      | Older, high-income customers with low spending                |

Includes a supervised model (Random Forest Classifier) trained to predict a customer’s cluster based on Age, Income, and Spending Score.

## Future Work
- Add product recommendation logic based on cluster
- Deploy as a simple Streamlit or Flask web app
- Connect with marketing platforms for real-time targeting

