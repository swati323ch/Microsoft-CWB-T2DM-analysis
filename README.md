# Discovering personas associated with Type 2 diabetes risk using Kaggle data
## Visualisation of data
Required libraries - matplotlib,seaborn,pandas
### Bivariate Plots
The function plot_bivariate in the code generates bivariate plots for the specific features. This is useful for visualizing the relationship between categorical features and a target variable.
![img 1](https://github.com/swati323ch/Microsoft-CWB-T2DM-analysis/assets/133630051/b9e6e6ef-e9b5-4cea-afd7-45037869a9c9)
###  Correlation Matrix Heatmap
A correlation matrix is a table showing correlation coefficients between variables. Each cell in the table shows the correlation between two variables. This is useful for identifying relationships between numerical features and understanding how variables in your dataset interact with each other.
![Corelation](https://github.com/swati323ch/Microsoft-CWB-T2DM-analysis/assets/133630051/1fb018d0-f04f-4e00-9601-28e919390672)
###  Box Plots of Features
 Box plots are useful for visualizing the distribution, central tendency, and variability of data. They also highlight outliers within each feature.

## Feature Selection 
### Chi-Square Test
Since all the features are categorical, a Chi-Square test was performed to determine the significance of each feature with respect to the target variable. The Chi-Square test helps in identifying the most relevant features for predicting diabetes.

### Results of Chi-Square Test
Based on the Chi-Square test, features were ranked according to their significance. The feature AnyHealthcare was found to be the least significant and was dropped from the dataset.

## Persona Creation using Clustering
### Elbow Method
The Elbow Method was used to determine the optimal number of clusters for K-Means clustering. This method helps in identifying the number of clusters that best fit the data by plotting the inertia against the number of clusters.
![Elbow](https://github.com/swati323ch/Microsoft-CWB-T2DM-analysis/assets/133630051/8c04d69c-be3d-4766-876b-c70d5f99a98d)

### K-Means Clustering and Cluster Profiles
K-Means clustering was applied to the dataset to group individuals with similar health profiles. The resulting clusters represent groups with distinct characteristics, identified through the mean values of each feature within the clusters. This analysis provides insights into the typical health profiles of individuals in each cluster.
![Cluster](https://github.com/swati323ch/Microsoft-CWB-T2DM-analysis/assets/133630051/b8d390a8-f32d-4b1d-9078-c4d0a81f4f91)
## Cluster Profile Generation
To gain deeper insights, cluster profiles were generated to describe the typical characteristics and health behaviors of individuals in each cluster. The profiles included demographic information, health behaviors, and overall health status and also to generate actionable insights.


![actionable insights](https://github.com/swati323ch/Microsoft-CWB-T2DM-analysis/assets/133630051/c8852787-9569-4a04-a9cd-71f78c9f67e2)


## Model Training and Evaluation
After clustering, machine learning models were trained to predict diabetes within each cluster.
The overall accuracy is given bellow-


![Accuracy Score](https://github.com/swati323ch/Microsoft-CWB-T2DM-analysis/assets/133630051/63b48db3-cf76-4189-a156-978053ff42b0)

## Conclusion
This project utilizes K-Means clustering and machine learning to group individuals by health profiles, providing actionable insights for targeted interventions. Identification of distinct clusters with specific risk factors facilitates the development of personalized healthcare strategies. Enhancing data-driven approaches enriches our understanding of population health dynamics, leading to improved public health outcomes and advancements in personalized medicine.



