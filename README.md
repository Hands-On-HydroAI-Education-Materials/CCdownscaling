# Hands on Downscaling of Climate Change Scenarios using MyBinder

**This repository is a modification of https://github.com/drewpolasky/CCdownscaling repository for educational purposes.**

Description of Two Jupyter Notebooks
------------------------------------
**For application of downscaling of climate change scenarios, two jupyter notebooks were created.**

1. **The first jupyter notebook (1_Downloading_GCM_Data_from_Climate_Data_Store.ipynb)** demonstrated how to download GCM data from CDS(Climate Data Store) https://cds.climate.copernicus.eu/datasets.
- In this example, GCM(CIMP-6) data of EC-Earth3-CC(Europe) was downloaded for data preparation.

2. **The second jupyter notebook (2_Application_of _Downscaling_Methods_using_Machine_Learning.ipynb)** demonstrated how to apply Machine Leanring approaches for downscaling.
- In this exampe, (1) Random Forest, (2) Two Part Random Forest, (3) Quantile Mapping approaches were applied for downscaling.

Execution of Two Jupyter Notebooks
------------------------------------
**To start Jupyter notebook, please click [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Hands-On-HydroAI-Education-Materials/CCdownscaling.git/HEAD)**

1. After clicking **"lauch binder"**, please wait for this web browser to change to **Jupyterlab**.

2. Then, first open **1_Downloading_GCM_Data_from_Climate_Data_Store.ipynb** and execute each cell step by step to download GCM data
   
3. second open **2_Application_of _Downscaling_Methods_using_Machine_Learning.ipynb** and execute each cell step by step to apply statistical downscaling methods using machine learning.

>

    .
    ├── ...
    ├── iwssm_examples         # this folder is an example for Educational Program
    │   ├── data               # store gcm and observation data
    │   │   ├──cds             # gcm data folder
    │   │   │  ├── historical  # historical data of gcm
    │   │   │  ├── projection  # future projection data of gcm
    │   │   ├──obs             # observation data 
    │   ├── fig                # figures used to explain the process in jupyter notebooks
    │   ├── 1_Downloading_GCM_Data_from_Climate_Data_Store.ipynb                   # Download GCM from CDS using API
    │   └── 2_Application_of _Downscaling_Methods_using_Machine_Learning.ipynb     # Apply Machine Learning for Downscaling
    └── ...

>


## Citation

If you use CCdownscaling, please cite:

Andrew D. Polasky, Jenni L. Evans, Jose D. Fuentes,
CCdownscaling: A Python package for multivariable statistical climate model downscaling,
Environmental Modelling & Software,
Volume 165,
2023,    
105712,
ISSN 1364-8152,
https://doi.org/10.1016/j.envsoft.2023.105712.
