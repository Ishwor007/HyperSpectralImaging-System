# Hyperspectral Image Analysis: Dimensionality Reduction and Endmember Extraction

## Overview

This project implements hyperspectral image analysis workflows focused on:

- **Dimensionality Reduction** using Principal Component Analysis (PCA).
- **Endmember Extraction** using three different algorithms:
  - Pixel Purity Index (PPI)
  - Vertex Component Analysis (VCA)
  - N-FINDR

The goal is to reduce the spectral dimensionality of hyperspectral data while retaining 99% of the variance, and then extract meaningful endmembers from the PCA-reduced data.

---

## Tasks

### Task 1: Dimensionality Reduction (10 marks)
- Apply PCA to hyperspectral image data to reduce spectral bands.
- Choose the number of principal components that explain at least 99% of the total variance.

### Task 2: Endmember Extraction (30 marks)
- Use the PCA-reduced data to extract endmembers with the following algorithms:
  - **Pixel Purity Index (PPI)**
  - **Vertex Component Analysis (VCA)**
  - **N-FINDR**
- For each method:
  - Extract a fixed number of endmembers (typically 7–10).
  - Visualize the extracted endmember spectra (3 separate graphs, one for each method).
  - Visualize scatter plots of the reduced-dimensional data highlighting the location of selected endmembers (3 scatter plots, one for each method).

---


---

## Usage Instructions

1. **Data Preparation:**  
   Place your hyperspectral data cube (e.g., `.npy` files) inside the `/data` folder.

2. **Run PCA:**  
   Use the PCA script to reduce spectral dimensionality while preserving 99% variance.

3. **Endmember Extraction:**  
   Apply PPI, VCA, and N-FINDR on the PCA-reduced data to extract endmembers.

4. **Visualization:**  
   Each extraction method produces:
   - Endmember spectra plots.
   - Scatter plots of PCA components highlighting endmembers.

---

## Dependencies

- Python 3.x
- numpy
- matplotlib
- scikit-learn (for PCA)
- spectral (for PPI)
- Additional packages as required by VCA and N-FINDR implementations

Install dependencies using:

```bash
pip install numpy matplotlib scikit-learn spectral

