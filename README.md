# Replication materials for humid heat detection and attribution project
### Christopher Callahan, May 2021, Theories, Models, Data course

This repository provides data and code required to replicate the findings of my TMD project. The repo is organized into **Data**, **Scripts**, and **Figures** folders. Each script is either a python (.py) file or a Jupyter notebook (.ipynb). The total size of the repo is XX MB.

Raw data from ERA5 and CMIP is not provided here due to large file sizes, but scripts to process the raw data are provided if you would like to download the raw data yourself. Processed data is provided in each case, so the results of the analysis can be replicated except for the initial processing steps (i.e., calculating wet bulb temperature from daily maximum temperature, daily mean humidity, and daily mean pressure).

If you have questions or find errors in the analysis, feel free to email Christopher.W.Callahan.GR (at) dartmouth (dot) edu.

**Organization of Data folder:**
* **./Data/Tw/ERA5/**: Processed wet bulb temperature from ERA5 reanalysis using the Davies-Jones algorithm, warm season maximum, mean, and median, 1980-2019.
* **./Data/Tw/CMIP6/**: Processed wet bulb temperature from CMIP6 historical and SSP3-7.0 simulations, warm season maximum, mean, and median, 1980-2019.
* **./Data/Tw/CMIP6/piControl/**: Processed wet bulb temperature from CMIP6 pre-industrial control simulations, warm season maximum, mean, and median, 1980-2019.
* **./Data/Fingerprint/**: Theoretical spatial fingerprints from the CMIP6 historical/SSP3-7.0 simulations.
* **./Data/Noise/**: Timeseries of pattern similarity between the fingerprint and Tw anomalies from pre-industrial simulations, for use in calculating null distributions of signal strength.

**Organization of Scripts folder:**
* **./Scripts/CMIP6_Tw_Fingerprint_forGithub.ipynb**: Calculate spatial pattern of characteristic "fingerprint" from CMIP6 simulations.
* **./Scripts/ERA5_Tw_Detection_Analysis.ipynb**: Perform formal detection and attribution analysis using ERA5 Tw anomalies, CMIP6 fingerprint, and CMIP6 piControl distribution.
