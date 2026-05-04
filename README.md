# Code Archive: Master's Thesis on Isfjorden Sea Ice Dynamics

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19678997.svg)](https://doi.org/10.5281/zenodo.19678997) 

## Overview
This repository contains the data processing scripts and analysis code used in the Master's thesis: **"The Evolution of Isfjorden’s Sea Ice Regime: A 25-Year Analysis of Atmosphere-Ocean Forcing and Atlantification"** by Martin Lindlmayer. 

The code in this repository investigates the thermodynamic hierarchy of the Isfjorden system, specifically focusing on the atmospheric dominance (Freezing Degree Days, FDD) over ocean pre-conditioning (Volume-Weighted Mean Temperature, VTs) and the subsequent impact of sea ice on summer stratification.

**Please note: To keep this repository lightweight, no data files are hosted directly on GitHub. All publicly available datasets required to run this code are hosted on Zenodo.**

---

## Data Availability & Sources

To execute the notebook in this repository, you must first obtain the underlying data. 

### 1. Data Available on Zenodo
The following datasets have been archived and are openly available via Zenodo: **https://doi.org/10.5281/zenodo.19678997**
* **Atmospheric Data:** Daily air temperature data used to compute Freezing Degree Days (FDD). Originally obtained from the Norwegian Centre for Climate Services (NCCS) SeKlima web portal (Station: Svalbard Lufthavn, SN99840).
* **Sea Ice Data:** The foundational sea ice shapefiles derived from operational ice charts, generously provided by the Norwegian Meteorological Institute (MET Norway) Ice Service.

*Instructions:* Download the data archive from Zenodo and extract the contents into a local `data/` directory before running the notebook.

### 2. Restricted Oceanographic Data (Volume-Weighted Mean Temperature)
The Volume-Weighted Mean Temperature (VT) and summer ocean heat content (VTs) values utilized in this study are based on an unpublished, extended dataset. Due to licensing and publication constraints, **this dataset is not included in the Zenodo archive.**

This data builds upon the methodology established in:
> Skogseth, R., Olivier, L. L. A., Nilsen, F., Falck, E., Fraser, N., Tverberg, V., ... & Cottier, F. (2020). Variability and decadal trends in the Isfjorden (Svalbard) ocean climate and circulation—An indicator for climate change in the European Arctic. *Progress in Oceanography*, 187, 102394. https://doi.org/10.1016/j.pocean.2020.102394

The extended values were generously provided via personal communication. To request access to this specific dataset to fully replicate the analysis, please directly contact **Assoc. Prof. Ragnheid Skogseth** at the University Centre in Svalbard (UNIS). 

*Note: The code in this repository expects the files named `volume_weightedTandS_summer1987_2019.mat` and `volume_weightedTandS_winter1987_2019.mat` which users must obtain themselves.*

---

## Repository Structure

* `seaIceIsfjorden/`
  * `seaice_timeseries_notebook.ipynb`: The primary Jupyter Notebook containing all data processing, statistical analysis, and figure generation.
* `pyproject.toml` & `poetry.lock`: Dependency management files for the Python environment.
* `README.md`: This document.
* `LICENSE`: CC-BY-4.0 License details.

---

## Requirements and Installation

This project uses [Poetry](https://python-poetry.org/) for dependency management to ensure full reproducibility.

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/](https://github.com/)[YourGitHubUsername]/[YourRepoName].git
   cd [YourRepoName]
