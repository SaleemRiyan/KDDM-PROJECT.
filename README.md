# Spatial Similarity Discovery Using K-Nearest Neighbors (KNN)

# Project Overview
This project focuses on discovering spatial similarity between geographic locations using the "K-Nearest Neighbors (KNN)" algorithm. The goal is to identify locations that are most similar to a given target point based on "latitude and longitude coordinates".

Instead of prediction or classification, this work emphasizes "unsupervised similarity discovery", making it suitable for real-world geospatial applications such as urban planning, resource allocation, and location-based analysis.

---

# Problem Statement
Goal:  
Identify the most similar locations to a target location using geographic coordinates.

Why this matters:  
Many real-world problems rely on understanding spatial proximity and similarity. Unlike simple categorical data, spatial data is continuous and distance-sensitive, making similarity discovery non-trivial.

Key challenges include:
- Continuous spatial data (latitude & longitude)
- Distance-based similarity computation
- Sensitivity to distance metrics and scale

---

# Dataset Description
- File: `challenge.csv`
- All attributes are numerical
- Includes "latitude (N)" and "longitude (E)"
- No missing values
- The "last record*" in the dataset is treated as the "query instance"
- All previous records serve as "candidate locations" for similarity comparison

---

# KDD Pipeline
This project follows the "Knowledge Discovery in Databases (KDD)" process:

1. Data Selection – Load CSV dataset  
2. Preprocessing – Feature selection  
3. Transformation – Coordinate extraction  
4. Data Mining – KNN-based similarity computation  
5. Interpretation – Visual and distance-based analysis  

---

# Methodology
- Algorithm: "K-Nearest Neighbors (KNN)"
- Distance Metric: Euclidean Distance
- Features Used: Latitude and Longitude
- Number of Neighbors: k = 10
- Implementation: `NearestNeighbors` module from scikit-learn

KNN is chosen because it is an instance-based learning method that is highly effective for similarity discovery in spatial data.

---

# Baseline & Evaluation Strategy
- Baseline: Random neighbor selection
- Evaluation Approach:
  - Distance-based ranking
  - Visual inspection of spatial proximity
- No train-test split or accuracy metrics are used since the task is unsupervised

---

# Results & Discussion
- KNN-selected neighbors show "significantly smaller spatial distances" compared to the random baseline
- Distance-based similarity proves to be effective for spatial data
- Visual analysis confirms clustering around the target location

---

# Key Findings
- Spatial distance is a strong indicator of similarity
- KNN provides a simple yet effective baseline for spatial similarity tasks
- The approach is interpretable, reproducible, and easy to implement

---

# Limitations
- KNN is sensitive to noise
- Does not generalize beyond stored instances
- Performance depends heavily on distance metric and feature scaling

---

# Future Work
- Feature scaling and normalization
- Weighted distance metrics
- Incorporation of additional attributes
- Comparison with clustering methods such as "DBSCAN"

---

# Authors
- Farhan Ali  
- Trinish Nepal  
- Riyan Saleem  

Group: 6

---

#  Technologies Used
- Python
- NumPy
- Pandas
- scikit-learn
- Matplotlib

---

# How to Run
1. Clone the repository
2. Install required dependencies
3. Run the evaluation or KNN script
4. Analyze distance tables and visual outputs

---

# License
This project is for academic and educational purposes.

