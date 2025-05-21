# NHANES BMI–Diabetes Exploratory Analysis & Machine-Learning Pipeline  

This notebook walks through an end-to-end investigation of the 2021-2022 NHANES public-use data.  
It merges seven component files, engineers outcomes and predictors, produces interactive
visualisations with **Bokeh**, builds a random-forest diabetes classifier, and finishes with a
K-means + PCA lifestyle–health segmentation.

---

## 1  Quick start

Run the single cell below **once** to install every Python package used in the notebook
(including widgets and plotting back-ends). Skip it if your environment already has these
libraries ≥ the versions shown.

```bash
# ──- pip bootstrap ─────────────────────────────────────────────────────────────
pip install -q \
    pandas        \
    numpy        \
    scikit-learn  \
    matplotlib    \
    bokeh         \
    jupyterlab-widgets ipywidgets \
    seaborn      \
    statsmodels  \
    tqdm
```

