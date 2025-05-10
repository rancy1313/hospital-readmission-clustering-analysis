# hospital-readmission-clustering-analysis
K-means clustering analysis to identify patterns in hospital patient readmission using Python, scikit-learn, and t-SNE visualization.

## Project Overview
This project analyzes hospital patient data to identify patterns related to readmission using K-means clustering and t-SNE visualization techniques. By examining relationships between initial hospitalization duration, charges, and patient demographics, this analysis discovered a critical 48-day threshold that strongly predicts readmission risk.

## Key Findings
- **Readmission Threshold**: Patients staying less than 48 days had a 0% readmission rate, while those with longer stays had an 84% readmission rate
- **Feature Importance**: Initial hospital stay duration and total charges were the most significant factors in cluster separation
- **Model Optimization**: Reducing features from 7 to 2 improved the silhouette score from 0.27 to 0.80
- **High Blood Pressure Correlation**: Patients with high blood pressure incurred significantly higher additional charges

## Business Value
Healthcare facilities can use these insights to:
- Prioritize resources for patients approaching the 48-day threshold 
- Develop targeted intervention strategies for high-risk patients
- Potentially avoid penalties from Medicare/Medicaid for high readmission rates
- Review cost structures for patients with specific health conditions

## Technologies Used
- Python (Pandas, NumPy)
- Scikit-learn (K-means, StandardScaler)
- Matplotlib & Seaborn for visualization
- t-SNE for dimensionality reduction
- Yellowbrick for silhouette visualization

## Methodology
1. **Data Preprocessing**: Scaled features, identified outliers, checked for duplicates and missing values
2. **Cluster Evaluation**: Determined optimal number of clusters using elbow method and silhouette scores
3. **Feature Importance**: Analyzed separation between clusters for each feature
4. **Dimensionality Reduction**: Applied t-SNE to visualize high-dimensional data in 2D
5. **Cluster Analysis**: Explored relationships between cluster labels and categorical variables

## Future Work
- Apply hierarchical clustering techniques that don't favor uniform cluster sizes
- Incorporate categorical variables directly into the clustering process
- Develop predictive models based on the identified readmission threshold
- Investigate the relationship between high blood pressure, additional charges, and patient outcomes

---

*Note: This analysis was conducted for educational purposes and not for clinical decision-making.*
