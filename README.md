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

## 2  Data files you need
Download the following 2021-2023 NHANES component files (.XPT) from https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/[data-file]
- DEMO_L.XPT: Demographics

- BMX_L.XPT: Body Measurements

- GHB_L.XPT: Glycohemoglobin

- PAQ_L.XPT: Physical Activity Questionnaire

- INQ_L.XPT: Income Questionnaire

- DIQ_L.XPT: Diabetes Questionnaire

- DR1TOT_L.XPT: 24-h Dietary Recall (Total Nutrients)
