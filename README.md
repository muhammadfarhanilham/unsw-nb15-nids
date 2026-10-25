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

## Contact
M. F. Ilham (farhanilham@upi.edu)

## License
MIT
