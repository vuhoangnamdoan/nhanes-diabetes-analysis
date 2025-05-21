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
    pandas>=2.2        \
    numpy>=1.26        \
    scikit-learn>=1.4  \
    matplotlib>=3.8    \
    bokeh>=3.3         \
    jupyterlab-widgets ipywidgets>=8.1 \
    seaborn>=0.13      \
    statsmodels>=0.14  \
    tqdm               \
    pyreadstat         # faster .xpt reading (optional but recommended)
```
