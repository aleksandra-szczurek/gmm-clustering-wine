# Unsupervised Clustering with Gaussian Mixture Models (Wine Dataset)

**Group project** – Statistical Computing Methods, University of Perugia (Oct–Dec 2025)

## Goal

Identify the origin of **178 wines** from 5 chemical variables **without using the true labels**, then check the result against them.

## Method

- Exploratory analysis to find the most discriminating variables (flavanoids, total phenols)
- **Gaussian mixture model clustering** with `mclust`: number of clusters and covariance structure selected automatically by **BIC**
- **EM algorithm implemented from scratch** in R and benchmarked against `mclust`

## Results

| Approach | Clusters | Accuracy vs true classes |
|---|---|---|
| mclust (BIC-selected model) | 3 – matching the 3 true origins | **96.6%** (6 of 178 misclassified) |
| EM from scratch | 3 | 92.7% |

## Contents

- `report.pdf` – full homework report; the clustering analysis is Exercise 3 (the report also covers mixture simulation and optimisation exercises)

## Tools

R · mclust · EM algorithm
