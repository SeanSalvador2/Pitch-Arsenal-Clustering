
# Pitch Arsenal Clustering: A Machine Learning Approach

## Overview
This project applies **machine learning clustering techniques** to classify pitchers based on **similar pitch arsenals** using **Statcast pitch metric data**. The goal is to identify **archetypes of pitchers** and analyze how different pitchers succeed based on their pitch characteristics, movement, and usage.

## Goals
1. **Cluster pitchers based on their pitch arsenals** to find groups of pitchers with similar repertoires.
2. **Analyze differences in pitch usage and characteristics** among top and bottom performers within each cluster.
3. **Improve pitch inflection graphs** by refining how we identify **optimal pitch effectiveness zones**, accounting for variations in velocity, movement, and other metrics.

## Process

### 1. Data Collection & Preprocessing
- Using **Statcast** data for pitch metrics and season performance statistics.
- Normalizing and scaling data for effective clustering.

### 2. Clustering Methodology
- **Initial focus on four-seam fastballs** to keep the analysis simple.
- **Starting with 3D clustering (velocity, horizontal movement, vertical movement)** for visualization.
- Expanding to include **more pitch types and features** once initial clusters are validated.

### 3. Clustering Validation & Feature Selection
- Using **K-Means clustering** with:
  - **Elbow Method & Inertia** (measuring cluster tightness)
  - **Silhouette Score** (assessing within-cluster cohesion vs. separation from other clusters)
- Evaluating **dimensionality reduction techniques** (e.g., PCA, SVD) to improve clustering in higher-dimensional spaces.

### 4. Pitch Performance Analysis
- **Comparing top and bottom performers** in each cluster to identify key differentiating factors.
- Investigating whether **different types of pitchers succeed in distinct ways** based on:
  - Vertical Approach Angle (VAA)
  - Release height and extension
  - Pitch mix and movement profiles

### 5. Enhancing Pitch Inflection Graphs
- Refining the way we visualize **optimal pitch effectiveness zones** based on clustering results.
- Examining whether **multiple "sweet spots"** exist for the same pitch based on movement profiles.

## Challenges & Considerations
- **Defining optimal clusters**: Ensuring that clusters meaningfully differentiate pitcher types.
- **Curse of dimensionality**: High-dimensional feature spaces can degrade clustering performance.
- **K-Means limitations**: Requires careful feature selection and cluster evaluation metrics.
- **Accounting for arsenal effects**: Clustering by individual pitch vs. entire arsenal requires different approaches.

## Current Status
- **In progress**:
  - Initial clustering on four-seam fastballs with **K-Means**.
  - Experimenting with **feature selection** and **dimensionality reduction** to improve cluster quality.
  - Planning to expand to **multi-pitch clustering** for deeper arsenal insights.

## Future Work
- Test alternative clustering techniques (**DBSCAN, Gaussian Mixture Models**).
- Integrate additional pitch types for **full-arsenal clustering**.
- Develop interpretable visualizations for **inflection point analysis**.
- Apply results to real-world pitching strategies and optimization.

---

This project combines **data science, machine learning, and baseball analytics** to extract meaningful insights about **pitching success**.








- 
