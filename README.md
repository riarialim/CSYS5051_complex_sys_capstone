# CSYS5051: Complex Systems Capstone Project  
**Visualising Smart Meter Data by Manifold Learning using Dynamic Time Warping**  
A capstone project conducted by me in 2021 with supervision and guidance of A/Prof. Anastasios Panagiotelis.

---

## Project Summary

This capstone project explored how **manifold learning** and **Dynamic Time Warping (DTW)** can be used to analyze and visualize household electricity usage patterns. Working with the Irish Smart Meter Dataset, I applied dimensionality reduction techniques to detect temporal patterns and identify anomalous energy consumption behavior.

---

## Tools & Technologies

- **Language:** Python 3  
- **Libraries:**  
  - `scikit-learn` (for manifold learning and trustworthiness metrics)  
  - `dtaidistance` (for DTW computation)  
  - `pandas`, `NumPy`, `Matplotlib` for data handling and visualisations

---

## Problem & Approach

### Objective:
How can we effectively visualize and detect hidden patterns in high-dimensional smart meter data?

### Approach:
1. **Preprocessed** smart meter data for over 5000 households across 535 days
2. **Computed DTW distances** between time series to better capture temporal similarity
3. Applied **dimensionality reduction** techniques (MDS, Isomap, LLE)
4. Evaluated embedding quality using **Trustworthiness metrics**
5. Used **Local Outlier Factor (LOF)** to detect anomalous households on Christmas Day

---

## Key Insights

- **DTW** captured shape-based similarities better than Euclidean distance
- **Isomap and MDS** produced high-quality embeddings, outperforming LLE
- Detected clear seasonal trends and usage clusters
- Identified anomalies with **distinctive consumption patterns**


---

## Files
- `csys5051_500386873_report.pdf`: Full methodology, experiments, results, and discussion.
- `csys5051_500386873_presentation.pdf`: Presentation slides for project
- `data_processing-4.ipynb`: Script to preprocess data
- `ID 1003-Copy4.ipynb`, `ID 1539-Copy3.ipynb`, `Households for File1 (June Electric Usage).ipynb`: Scripts to analyse the data and visualise the results
- `euclidean vs dtw distance.ipynb`: Script to illustrate the difference of warping methods to compute distances between DTW and Euclidean
