# Image Compression and Restoration with PCA

An interactive application that uses **Principal Component Analysis (PCA)** to compress grayscale images and reconstruct them from a reduced number of components.

## Description

This project demonstrates how PCA can be used as a dimensionality reduction technique applied to images: each row of pixels is treated as a point in a high-dimensional space, and reconstruction from the first *k* principal components approximates the original image with less stored information.


## Features

- Load images from the browser (Jupyter widget)
- Slider to select the number of PCA components (1–100)
- Visual comparison between the original and reconstructed images
- Download the restored image in `.jpg` format
- Automatic conversion to grayscale if the image is RGB

## Pipeline

```
RGB/grayscale image → Normalization → Standardization (StandardScaler)

→ PCA (k components) → Inverse reconstruction → Restored image
```

## Technologies

- Python 3/Jupyter
- `numpy`, `scikit-learn` (PCA, StandardScaler)
- `Pillow` (image handling)
- `matplotlib` (visualization)
- `ipywidgets` (interactive interface)

## How run

```tap
installation of piping pillow numpy science learning matplotlib ipywidgets
jupyter notebook Project_CompriRestau.ipynb
```

## Parameter Key

| Parameter | Range | Effect |
|---|---|---|
`n_components` | 1 – 100 | Higher number, better quality; less compression |

## Applied Mathematical Concepts

- Singular Value Decomposition (SVD)
- Cumulative Explained Variance
- Low-Range Matrix Reconstruction
