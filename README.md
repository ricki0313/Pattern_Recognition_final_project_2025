# Pattern Recognition for Customer Behavior Analysis  
*A Study Using the UCI Online Retail II Dataset*

This project uses the UCI Online Retail II dataset to explore how pattern recognition (PR) methods behave when grouping and classifying customer behavior. By building features, reducing dimensions, visualizing the data, and analyzing errors, this study evaluates how well different models explain the structure of the data and how useful they are in practice.

## Structure

- w1_Data cleaning, aggregation, visualization
- w2_Data standardization, dimensionality reduction
- w3_Unsupervised learning method (K-means)
- w4_Supervised learning method (compare LDA, KNN, Naive Gaussian)
- w5_Findings, analysis, and report

## Setup (Windows / PowerShell)
```bash
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

## Dataset and Features
The customer-level features used in this project are generated from the raw Online Retail II dataset.

Due to file size and licensing considerations, raw data and generated feature files are not included in this repository.

To reproduce the features:
1. Download the Online Retail II dataset from the UCI Machine Learning Repository:
    https://archive.ics.uci.edu/dataset/502/online+retail+ii
2. Place the raw XLSX file under `data/raw/`.
3. Run the data cleaning and aggregation notebooks in order.


## Execution Order
The notebooks in this project are organized by analysis stages and should be run in the following order:

1. **w1**
    - `data_cleaning.ipynb`
    - `data_aggregation.ipynb`
    - `data_visualization.ipynb`

2. **w2**
    - `standardization.ipynb`
    - `pca.ipynb`

3. **w3**
    - `k_means_pca.ipynb`
    - `k_means_feat.ipynb`

4. **w4**
    - `lda.ipynb`
    - `knn.ipynb`
    - `naive_gaussian.ipynb`

The final findings and interpretations are summarized in the report provided in **w5**.
All features will be generated automatically during this process.