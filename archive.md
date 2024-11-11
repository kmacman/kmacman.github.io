### XGBoost and Transformer Time Series Models to Predict Emergency Department Visits

Using [publicly available data](https://dataverse.harvard.edu/dataset.xhtml;jsessionid=14a51733a6d8f4ce61701457b27c?persistentId=doi:10.7910/DVN/QHPZOX), I trained an XGBoost model to predict daily emergency department visits at UC Davis.

I engineered time series features (lags, rolling averages) to maximize the xgb model results.

This is an ongoing project, with plans to include more robust external data, such as holidays, local major events, air quality, and internet search data.

I have also begun working on a transformer model for the same task.

<img src="images\time_series.png"/> <br>
_XGB model results_

<img alt="Static Badge" src="https://img.shields.io/badge/Python-grey?logo=Python"> <img alt="Static Badge" src="https://img.shields.io/badge/scikit learn-grey?logo=scikitlearn"> <img alt="Static Badge" src="https://img.shields.io/badge/Pandas-grey?logo=PAndas"> <img alt="Static Badge" src="https://img.shields.io/badge/pyTorch-grey?logo=pytorch"> <img alt="Static Badge" src="https://img.shields.io/badge/XGBoost-grey?logo=">


 [GitHub Repo of Model Development Notebook](https://github.com/kmacman/er_visits_xgb/blob/main/davis_xgb_fe.ipynb)<br>
 [PDF of EDA Notebook](pdf\davis_eda.pdf)<br>
 [GitHub Repo of Transformer Model](https://github.com/kmacman/er_visits_transformer/blob/main/notebook.ipynb)
 

---