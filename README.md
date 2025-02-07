# Clustering-Based-Analysis-of-Sleep-patterns-in-Students

# Student Sleeping Patterns Clustering and Analysis

## Project Overview

This project focuses on the analysis and clustering of **student sleep patterns** based on various sleep-related features. The dataset comprises information from **500+ students**, including factors such as **age**, **gender**, **university year**, **sleep duration**, and lifestyle habits like **study hours**, **screen time**, and **caffeine intake**. The goal is to apply **unsupervised learning** techniques, specifically **KMeans clustering**, to identify distinct sleep behaviors among students. **Principal Component Analysis (PCA)** is used for dimensionality reduction, optimizing computational efficiency, and retaining essential data characteristics. The clustering performance is evaluated using the **Silhouette Score** to measure the quality of the clusters.

## Key Features

- **Data Preprocessing**:  
  The dataset is cleaned, normalized, and processed to ensure that it is in a suitable format for clustering.

- **Dimensionality Reduction with PCA**:  
  **Principal Component Analysis (PCA)** is applied to reduce the feature space by **75%**, optimizing computational efficiency and model interpretability.

- **Clustering with KMeans**:  
  **KMeans clustering** is used to identify groups of students with similar sleep patterns, achieving a **Silhouette Score of 0.87**, indicating well-separated clusters.

- **Data Visualization**:  
  Various visualizations, including scatter plots and bar charts, help interpret the clustering results and explore sleep behavior trends.

- **Model Evaluation**:  
  The **Silhouette Score** is used to evaluate the quality of the clusters, providing insights into how well-defined the groupings are.

## Prerequisites

This project requires Python 3.x and the following libraries:

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `warnings`

## Project Details

### 1. **Data Collection and Preprocessing**

The dataset includes the following independent features:

- **Student ID**: Unique identifier for each student.
- **Age**: The student's age.
- **Gender**: Gender of the student.
- **University Year**: Year of study (e.g., 1st year, 2nd year, etc.).
- **Sleep Duration**: Average duration of sleep per night.
- **Study Hours**: Number of hours spent studying per day.
- **Screen Time**: Daily screen usage in hours.
- **Caffeine Intake**: Daily caffeine intake in milligrams.
- **Physical Activity**: Daily physical activity level.
- **Sleep Quality**: Self-reported quality of sleep.
- **Weekday Sleep Start**: Time the student typically falls asleep on weekdays.
- **Weekend Sleep Start**: Time the student typically falls asleep on weekends.
- **Weekday Sleep End**: Time the student wakes up on weekdays.
- **Weekend Sleep End**: Time the student wakes up on weekends.

The data is preprocessed by removing colums that are not affecting the sleep quality, normalizing numerical features and encoding categorical variables where necessary.

### 2. **Dimensionality Reduction Using PCA**

**Principal Component Analysis (PCA)** is applied to reduce the feature dimensionality by **75%**. PCA works by identifying the most significant features that capture the majority of the variance in the data and then projecting the data into a lower-dimensional space, which benefits the clustering process by improving efficiency and interpretability. The main advantages of PCA are:

- **Faster computation**: With fewer dimensions, the clustering process is faster.
- **Improved model interpretability**: Fewer dimensions make it easier to visualize and understand the data.
- **Reduced risk of overfitting**: By eliminating less important features, PCA helps to avoid overfitting and ensures that the model generalizes well.

### 3. **Clustering with KMeans**

The KMeans clustering algorithm is used to group students into clusters based on their sleep patterns and lifestyle habits. The optimal number of clusters is determined through various validation techniques, and the quality of the clusters is evaluated using the **Silhouette Score**. A **Silhouette Score of 0.87** indicates that the clustering is well-separated and meaningful, with distinct groupings based on sleep behaviors.

### 4. Data Visualization

Data visualizations are used to interpret and understand the results. Key plots include:

- Scatter plots to visualize the relationship between different features.
- Bar charts to represent the distribution of sleep behaviors across clusters.
  
These visualizations help in interpreting the clustering results and understanding the patterns of student sleep behavior.

### 5. Model Evaluation

The performance of the clustering algorithm is evaluated using the **Silhouette Score**. This score ranges from -1 to 1, with higher values indicating better-defined clusters. A score of **0.87** signifies that the model has effectively grouped students into distinct clusters based on their sleep and lifestyle features.

