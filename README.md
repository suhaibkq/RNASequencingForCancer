# 🧬 RNA-Seq Gene Expression Analysis – PCA Case Study

## 📌 Problem Statement

RNA sequencing (RNA-Seq) is a cornerstone technique in life sciences and oncology. This project analyzes gene expression data from various cancer types to uncover patterns through dimensionality reduction using Principal Component Analysis (PCA).

## 🎯 Objective

- Apply PCA to reduce the dimensionality of RNA-Seq gene expression data
- Visualize high-dimensional gene expression data in 2D space
- Identify clusters and separability between cancer types

## 🧪 Techniques Used

- **Principal Component Analysis (PCA)** for unsupervised dimensionality reduction
- **Visualization** of PCA components using scatter plots
- **Data preprocessing** including standardization and feature selection

## 📊 Dataset

- `labels.csv`: Contains labels for each RNA-Seq sample (tumor types)
- `RNA-Seq Data (Google Sheet)`: Contains gene expression values (dummy gene names: `gene_1`, `gene_2`, ..., `gene_n`) for each patient sample

- **Tumor Types in the dataset**:
  - `BRCA` – Breast Cancer
  - `KIRC` – Kidney Renal Clear Cell Carcinoma
  - `COAD` – Colon Adenocarcinoma
  - `LUAD` – Lung Adenocarcinoma
  - `PRAD` – Prostate Adenocarcinoma

## 📁 Repository Structure

```
├── USL_W2_AdditionalCaseStudy_GeneAnalysis.ipynb    # Main notebook
├── labels.csv                                       # Tumor type labels
├── RNA_Sequencing_Data.gsheet (linked/external)     # Gene expression data
├── README.md                                        # Project documentation
```

## 📈 Project Workflow

1. **Data Import & Merging**
   - Combined gene expression values with cancer type labels

2. **Data Preprocessing**
   - Standardized gene expression values to zero mean and unit variance
   - Converted categorical tumor types into labeled color groupings

3. **PCA Implementation**
   - Applied PCA using `scikit-learn` to reduce thousands of gene features to just 2 principal components
   - Analyzed the explained variance ratio

4. **Visualization**
   - Plotted the 2D PCA projection to identify how cancer types separate in lower dimensions
   - Color-coded by tumor type

## 🏆 Results & Insights

- PCA successfully reduced thousands of features into just 2 components with high interpretability
- Distinct clustering was observed for specific cancer types (e.g., BRCA vs. LUAD)
- PCA can act as an effective exploratory tool for pattern recognition in genomics data

## 🔍 Takeaways

- Dimensionality reduction is essential when dealing with high-throughput biological data
- PCA aids not only in compression but also in visual diagnostics and hypothesis generation
- RNA-Seq data can show clear groupings by cancer type, enabling downstream tasks like classification or biomarker discovery

## 🚀 Future Enhancements

- Explore other techniques like t-SNE or UMAP for non-linear embeddings
- Combine gene expression data with clinical metadata for deeper insights
- Implement clustering algorithms (e.g., K-means, DBSCAN) on PCA results

## 👨‍💻 Author

**Suhaib Khalid**  
Machine Learning in Healthcare

