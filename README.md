This repository contains code used to generate figures for the manuscript "Environmental and Microbial Drivers of Global Rhizosphere Resistome Assembly". 

Rhizosphere serves as a critical reservoir for antibiotic resistance genes (ARGs). Here we accessed the ecological mechanisms driving ARG assembly at the plant–soil interface. 

In the main branch, you can find all codes and scripts used for statistical analysis and visualization in this study. Demo datasets for analysis and visualization will be uploaded after the publication of our manuscript.

# analysis-code
This repository contains all R and Python scripts used for the statistical analyses and visualizations in our study on the rhizosphere resistome. The analyses integrate multivariate statistics, network analysis, and machine learning to explore the patterns and drivers of antibiotic resistance gene (ARG) assemblages across diverse crop rhizospheres.
1. Clustering Analysis
   1. K-means clustering was performed in Python (v3.12) using the FactoExtra package (v1.0.7) based on the ARG abundance matrix (4,803 ARGs).
   2. The optimal number of clusters (k) was determined using the elbow method (within-cluster sum of squares).
   3. Clustering validity was evaluated via PCA visualization.

2. Diversity and Ordination Analyses
   1. Alpha diversity indices (Chao1, Shannon), PCA, PCoA, NMDS, and Procrustes analyses were computed in R (v4.4.1) using the vegan package (v2.6.8).

3. Geographic Visualization
   1. Crop distribution maps were created using the maps (v3.4.2.1) and mapdata (v2.3.1) packages in R.

4. Network Construction
   1. Co-occurrence networks were built using Hmisc (v5.2.3) and visualized in Cytoscape (v3.10.3).
   2. Structural Equation Modeling (SEM) conducted with lavaan (v0.6.19) in R. 

5. Machine Learning and Feature Importance
   1. Random Forest and SHapley Additive exPlanations (SHAP) analyses were performed using scikit-learn (v1.5.0) and shap (v0.44.1) in Python (v3.12).

/R_scripts/              # R scripts for diversity, ordination, SEM, and mapping
/Python_scripts/         # Python scripts for clustering, Random Forest, and SHAP analysis
README.md                # Overview and instructions (this file)

# Requirements

R ≥ 4.4.1

Python ≥ 3.12

Detailed package versions are listed in requirements.txt.

# Contact

For questions or requests, please contact Huihui Yang at 17356889451@163.com.
