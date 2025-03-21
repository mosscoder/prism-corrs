# Bitterroot ValleyPRISM Climate & Elevation Analysis

## Overview

This repository contains code to analyze the relationship between elevation and climate variables (mean annual temperature and precipitation) using PRISM 30-year climate normals and SRTM elevation data through Google Earth Engine. Please find the code in [plot_corrs.ipynb](https://github.com/mosscoder/prism-corrs/blob/main/plot_corrs.ipynb).

## Data Sources

- **Climate Data**: PRISM 30-year climate normals (OREGONSTATE/PRISM/Norm81m)
- **Elevation Data**: SRTM Digital Elevation Model (USGS/SRTMGL1_003)
- **Resolution**: PRISM data has a resolution of approximately 927.66 meters

## Study Area

The study area is located in western Montana, covering a rectangular region defined by the following coordinates:
- Northwest: [-114.08229911631165, 46.80969368443738]
- Northeast: [-113.84197318857727, 46.80969368443738]
- Southeast: [-113.84197318857727, 46.12679350521872]
- Southwest: [-114.08229911631165, 46.12679350521872]

![AOI Map](aoi_map.png)

## Results

The analysis reveals extremely strong correlations between elevation and climate variables:

- **Elevation-Temperature Correlation**: r = -0.971 (p < 1e-6)
- **Elevation-Precipitation Correlation**: r = 0.919 (p < 1e-6)

These results clearly demonstrate two fundamental climate patterns in mountainous regions:
1. A strong negative correlation between elevation and temperature (adiabatic lapse rate)
2. A strong positive correlation between elevation and precipitation (orographic effect)

With 2,378 sample points analyzed, these relationships are statistically robust and highly significant.

![Elevation vs Temperature](https://github.com/mosscoder/prism-corrs/blob/main/elevation_climate_correlations.png)