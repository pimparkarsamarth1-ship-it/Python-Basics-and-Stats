# Python Basics and Stats

This repository contains my practice notebooks from learning Python, basic programming concepts, and introductory data analysis using single-cell RNA-seq style datasets.

## Notebook

### `01_python_and_singlecell_basics.ipynb`

This notebook covers:

#### 1. Core Python fundamentals
- Printing and basic syntax
- Variables and core data types (`str`, `int`, `float`, `bool`)
- Type conversion (e.g. `int` → `str`, `bool` handling)
- Lists (e.g. favourite genes)
- Dictionaries (simple key–value data structures)

#### 2. Working with `pandas`
- Loading metadata and count matrices from CSV files
- Inspecting data with `.head()`, `.info()`, `.dtypes`
- Selecting columns and rows
- Filtering cells using boolean masks and `.query()`

#### 3. Basic single-cell QC-style plots
- Histograms of `nCount_RNA` and `nFeature_RNA`
- Side-by-side histograms using Matplotlib subplots
- Distribution of `nFeature_RNA` using Seaborn
- Violin plot of a mitochondrial gene (`MT-CO3`)
- Heatmap of mitochondrial genes (columns matching `^MT-`)
- Joint plot of log-transformed counts for `MT-ND1` vs `MT-ATP6`

## Data

The notebook expects the following files in a `data/` directory:

- `data/mini_meta.csv` – small metadata table (e.g. `nCount_RNA`, `nFeature_RNA`, cell IDs)
- `data/mini_counts.csv` – small gene-by-cell count matrix

These are toy/simplified datasets used for practice and demonstration only.

## Purpose

This repository tracks my learning as I build foundations in:

- Python programming
- basic statistics and plotting
- single-cell RNA-seq style data handling

It is a starting point for more advanced analysis workflows in neuroscience, genetics, and single-cell data.
