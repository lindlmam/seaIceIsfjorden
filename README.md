# Code Archive: Master's Thesis on Isfjorden Sea Ice Dynamics

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19678997.svg)](https://doi.org/10.5281/zenodo.19678997) 

## Overview
This repository contains the data processing scripts and analysis code used in the Master's thesis: **"The Evolution of Isfjorden’s Sea Ice Regime: A 25-Year Analysis of Atmosphere-Ocean Forcing and Atlantification"** by Martin Lindlmayer. 

The code in this repository investigates the thermodynamic hierarchy of the Isfjorden system, specifically focusing on the atmospheric dominance (Freezing Degree Days, FDD) over ocean pre-conditioning (Volume-Weighted Mean Temperature, VTs) and the subsequent impact of sea ice on summer stratification.

**Please note: To keep this repository lightweight, no data files are hosted directly on GitHub. All publicly available datasets required to run this code are hosted on Zenodo.**

---

## Data Availability & Sources

To execute the scripts in this repository, you must first obtain the underlying data. 

### 1. Data Available on Zenodo
The following datasets have been archived and are openly available via Zenodo: **10.5281/zenodo.19678997**
* **Atmospheric Data:** Daily air temperature data used to compute Freezing Degree Days (FDD). Originally obtained from the Norwegian Centre for Climate Services (NCCS) SeKlima web portal (Station: Svalbard Lufthavn, SN99840).
* **Sea Ice Data:** The foundational sea ice shapefiles derived from operational ice charts, generously provided by the Norwegian Meteorological Institute (MET Norway) Ice Service.

*Instructions:* Download the data archive from Zenodo and extract the contents into a local `data/` directory within this repository before running the scripts.

### 2. Restricted Oceanographic Data (Volume-Weighted Mean Temperature)
The Volume-Weighted Mean Temperature (VT) and summer ocean heat content (VTs) values utilized in this study are based on an unpublished, extended dataset. Due to licensing and publication constraints, **this dataset is not included in the Zenodo archive.**

This data builds upon the methodology established in:
> [Insert the citation for Ragnheid Skogseth's published paper here, e.g., Skogseth, R., et al. (Year). Title of paper. Journal.]

The extended values were generously provided via personal communication. To request access to this specific dataset to fully replicate the analysis, please directly contact **Assoc. Prof. Ragnheid Skogseth** at the University Centre in Svalbard (UNIS). 

*Note: The code in this repository expects a file named `volume_weightedTandS_summer1987_2019.mat` and `volume_weightedTandS_winter1987_2019` which users must obtain themselves.*

---

## Repository Structure

* `scripts/`: Contains all analysis code used to generate the thesis figures and statistics.
  * `[Script 1 name, e.g., 01_process_temperature.py]`: [Brief description of what it does]
  * `[Script 2 name, e.g., 02_calculate_FDD.R]`: [Brief description]
  * `[Script 3 name, e.g., 03_plot_correlations.py]`: [Brief description]

## Requirements and Installation
To run the code in this repository, you will need:
* [List your programming language, e.g., Python 3.9+ or R 4.2+]
* [List major packages used, e.g., pandas, numpy, matplotlib, xarray, geopandas]

## Citation
If you use the code provided in this repository, please cite the associated Master's thesis:

> Lindlmayer, M. (2026). *The Evolution of Isfjorden’s Sea Ice Regime: A 25-Year Analysis of Atmosphere-Ocean Forcing and Atlantification*. Master's Thesis, Graz University of Technology / University of Graz.

## Acknowledgements
A special thanks to the Norwegian Meteorological Institute (MET Norway) Ice Service for the ice chart shapefiles, and to Assoc. Prof. Ragnheid Skogseth (UNIS) for the extended VT dataset.
