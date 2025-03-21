# PRISM Climate & Elevation Analysis

## Overview

This repository contains code to analyze the relationship between elevation and climate variables (temperature and precipitation) using PRISM 30-year climate normals and SRTM elevation data through Google Earth Engine.

## Description

This project utilizes the Google Earth Engine Python API to extract and analyze climate and elevation data for a specific area of interest (AOI) in Montana. The analysis focuses on understanding and quantifying the relationship between elevation and two key climate variables:

1. Mean annual temperature
2. Annual precipitation

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

## Results

The analysis reveals extremely strong correlations between elevation and climate variables:

- **Elevation-Temperature Correlation**: r = -0.971 (p < 1e-6)
- **Elevation-Precipitation Correlation**: r = 0.919 (p < 1e-6)

These results clearly demonstrate two fundamental climate patterns in mountainous regions:
1. A strong negative correlation between elevation and temperature (adiabatic lapse rate)
2. A strong positive correlation between elevation and precipitation (orographic effect)

With 2,378 sample points analyzed, these relationships are statistically robust and highly significant.

## Visualizations

The repository includes two primary visualizations:
1. An interactive map showing the Area of Interest (AOI)
2. Correlation plots displaying the relationships between:
   - Elevation and temperature
   - Elevation and precipitation

## Dependencies

- ee (Earth Engine API)
- numpy
- pandas
- matplotlib
- scipy
- geemap
- folium

## Usage

To run the analysis:

```python
# Initialize Earth Engine
ee.Initialize()

# Run the entire script to generate:
# 1. Interactive AOI map (saved as aoi_map.html)
# 2. Correlation plots (saved as elevation_climate_correlations.png)
# 3. Statistical output in the console
```

## License

[Add your preferred license here]

## Author

[Your name/organization]
