# DA5401 A5: Visualizing Data Veracity Challenges in Multi-Label Classification
**Name:** Samyam Rishika  
**Roll Number:** CE22B101  

---

## Project Overview  
This assignment explores **data veracity issues** in the **Yeast multi-label dataset**, focusing on challenges in visualizing and interpreting noisy, ambiguous, and overlapping data.  
We employ **t-SNE** and **Isomap** to study how dimensionality reduction reveals label overlap and structure in gene expression data.  

The goal is to understand how **data veracity problems** such as noisy labels, outliers, and complex manifolds affect classifier performance and why simple models struggle in such datasets.

## Folder Structure
```bash
├── assignment5.ipynb # Main Jupyter Notebook (all code, plots, analysis, narrative)
├── README.md
└── data/             # Directory for dataset files
    ├── yeast.arff
    └── yeast.xml
```

## How to Run
1. Clone the repository and navigate to the project directory:

```bash
git clone https://github.com/Rishika-28/assignment-5-Rishika-28.git
cd assignment-5-Rishika-28
```
2. Open assignment5 in Jupyter Notebook.

3. Run all cells in sequence. The notebook will:

- Load and preprocess Yeast dataset (2417 samples, 103 features, 14 labels)
- Select top single and multi-label categories for visualization
- Scale features using StandardScaler
- Apply t-SNE (local structure) with optimized perplexity
- Apply Isomap (global structure)
- Visualize clusters and inspect data veracity issues (noise, outliers, overlapping labels)

## Notes
1. The dataset (arff and xml files) have been uploaded in the data folder. The notebook also contains information on how to download it from the source.
2. t-SNE and Isomap can be computationally intensive for very large datasets. For this dataset size, typical execution times are manageable.

## Requirements
```bash
pip install numpy pandas scikit-learn matplotlib seaborn scikit-multilearn liac-arff
```


