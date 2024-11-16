# Hands on Downscaling of Climate Change Scenarios using MyBinder

This repository is a modification of https://github.com/drewpolasky/CCdownscaling repository for educational purposes.

For application of downscaling of climate change scenarios, two jupyter notebooks were created.

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






This package provides implementation of several statistical climate downscaling techniques, as well as evaluation tools for downscaling outputs. 

## Requirements

See [`environment.yml`](./environment.yml). Tensorflow is pinned in this conda environment in the interest of reproducibility.

## Installation 

With conda:
```bash
git clone https://github.com/drewpolasky/CCdownscaling
cd CCdownscaling
conda env create -f environment.yml -n ccdown_env
conda activate ccdown_env 
export PYTHONPATH=$PWD:$PYTHONPATH
```
## Usage

An example use case for downscaling precipitation at Chicago O'Hare airport can be found in the example folder.
This example requires some example data, which can be downloaded from: https://zenodo.org/records/7817799

Once that data is in place, the example can be run with: 
```bash
cd example
python ohare_example.py
```
And runs through several downscaling methods, including SOM, random forest, and quantile mapping. 
All these methods are then compared on PDF skill score, KS test, RMSE, bias, and autocorrelation, 
along with the undownscaled values from the NCEP reanalysis.

There are several command line settings that can be adjusted: target variable (max_temp or precip), stationID, 
and split_type (simple, percentile, seasonal):
```bash
python ohare_example.py
```
There is also a jupyter notebook with the same example included in the example folder. 

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

