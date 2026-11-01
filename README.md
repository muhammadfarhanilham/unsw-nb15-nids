# Optimizing Network Intrusion Detection Using Explainable Gradient Boosting

Code accompanying the manuscript submitted to the Journal of Applied
Informatics and Computing (JAIC). The notebook evaluates LightGBM, XGBoost,
and an MLP on UNSW-NB15 using SMOTENC, LightGBM Gain-based feature
selection, and SHAP.

## Environment
Tested on Google Colab (CPU), Python 3.13. Install the tested versions:

    pip install -r requirements.txt

## Dataset
Download `UNSW_NB15_training-set.parquet` and `UNSW_NB15_testing-set.parquet`
from https://research.unsw.edu.au/projects/unsw-nb15-data-set and place both
files in a folder named `archive/` in the working directory.

## Usage
Open `notebooks/UNSW_NB15_NIDS.ipynb` and run the cells from top to bottom.
The random seed is 42. Small numerical differences may occur across
library versions or hardware.

## Mapping to the manuscript

The notebook reproduces the numbers reported in the manuscript:

| Manuscript item | Notebook cell (heading) |
|---|---|
| Table 1: Top-10 Gain ranking | Revision (B2): Top-10 Gain ranking and share |
| Table 2: SMOTENC class distribution | Revision (B4): Class distribution before and after SMOTENC |
| Table 5, Figure 2: per-class results and confusion matrix | Revision (B3/B4) cells |
| Tables 7 and 8: binary confusion matrix, DR, FNR, FAR | Revision (A1): Binary confusion matrix |
| McNemar test and 95% CI of the paired difference | STEP 7.3 and Revision (B4): 95% CI |

## Contact
M. F. Ilham (farhanilham@upi.edu)

## License
MIT

## Notes
Code comments are in English. Console messages (printed output) are in
Indonesian, the language in which the experiments were run; all reported
metrics and table headers are language-independent. Inference times are
single-run, amortized batch measurements on a shared Colab CPU and may vary
between runs.
