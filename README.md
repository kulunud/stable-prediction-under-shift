# Learning When the Concept Shifts: Confounding, Invariance, and Dimension Reduction


This repository contains the code and instructions to reproduce the results presented in Section 5 of the manuscript.

## 1. Computational Environment

The code requires Python 3 and several scientific computing libraries. You can set up the environment using `conda`.

```bash
conda env create -f environment.yml
conda activate concept_shift_repro
```

**Hardware Requirements:**
The simulations can run on a standard CPU. 

## 2. Directory Structure

*   `*.ipynb`: Jupyter notebooks for the experiments.
*   `data/`: Directory for input datasets.
*   `figs/`: Directory where generated figures will be saved.

**Note:** The notebooks are configured to automatically create the `data` and `figs` directories if they do not exist.

## 3. Data

Please ensure the following datasets are placed in the `data/` directory:
*   **Bike Sharing:** `data/bike+sharing+dataset/hour.csv` 
    - The whole folder `bike+sharing+dataset` is available at https://doi.org/10.24432/C5W894.
*   **Forest Fires:** `data/forest+fires/forestfires.csv`
    - The whole folder `forest+fires` is available at https://doi.org/10.24432/C5D88D.
*   **Institutions:** `data/Institutions/Institutions.DTA`
    - Available at https://didattica.unibocconi.it/mypage/upload/48805_20241119_031344_48805_20100622_123124_REGIONS_GT_JUN10.ZIP.
    - Zip the downloaded file and rename the `.DTA` file to `Institutions.DTA`.
*   **Wine:** `data/wine+quality/winequality-red.csv` and `data/wine+quality/winequality-white.csv`
    - The whole folder `wine+quality` is available at https://doi.org/10.24432/C56S3T.

## 4. Reproduction Pipeline

To reproduce the results, run the notebooks in the following order (or as needed):

1.  **`bike-sharing.ipynb`**: Reproduces the Bike Sharing dataset analysis.
2.  **`forest-fires.ipynb`**: Reproduces the Forest Fires dataset analysis.
3.  **`institutions.ipynb`**: Reproduces the Institutions dataset analysis.
4.  **`wine.ipynb`**: Reproduces the Wine dataset analysis.

Each notebook is expected be executed in less than five minutes on a standard CPU.
