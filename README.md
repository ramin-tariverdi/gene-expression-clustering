# Gene Expression Analysis and Sample Clustering

This project focuses on the analysis of high-dimensional genomic data. It utilizes Python-based data science tools to process gene expression levels across multiple samples, perform exploratory data analysis (EDA), and implement clustering or classification status checks.

## Project Overview

### 1. Data Understanding & Preparation

The analysis uses a dataset (`data.csv`) containing gene expression data for 40 samples and 1,000 genes.

- **Data Transformation**: The raw CSV was loaded and transposed to ensure that genes are represented as features (columns) and samples as observations (rows).
- **Structure**:
  - **Rows**: 40 samples (labeled `sample1` to `sample40`).
  - **Columns**: 1,000 genes (labeled `gene1` to `gene1000`).

### 2. Exploratory Data Analysis (EDA)

The notebook includes statistical summaries and visualizations to understand the variance and distribution of the gene expression levels.

- **Visualizations**: Histograms and data distribution plots are used to inspect the range of expression values across different genes.
- **Correlation Analysis**: The project explores relationships between different genes through correlation matrices to identify potential co-expression patterns.

### 3. Sample Status & Classification

The project implements logic to assign and verify the status of specific samples.

- **Status Labeling**: A `real_status` column was added to the data to distinguish between different groups of samples (e.g., status 0 vs. status 1).
- **Grouping**:
  - **Samples 1-20**: Typically assigned to one status (e.g., Status 0 or 1).
  - **Samples 21-40**: Typically assigned to the opposing status.

## Technology Stack

- **Language**: Python 3.x
- **Core Libraries**:
  - `pandas`: For data manipulation and indexing.
  - `numpy`: For numerical computations and matrix operations.
  - `matplotlib`: For generating histograms and visual distributions.

## How to Run

1. Ensure the dataset `data.csv` is located in the root directory of the project.
2. Install the required dependencies:
   ```bash
   pip install pandas numpy matplotlib
   ```
3. Open `gene_expression.ipynb` in a Jupyter environment.
4. Run the cells sequentially to observe the data transformation and final sample status assignments.
