# Remote sensing
# Satellite-Based Environmental Analysis of the Indus River Basin

<img width="515" height="424" alt="image" src="https://github.com/user-attachments/assets/2353476b-b0e9-414c-93c8-cabfeb1ccca2" />
 <img width="483" height="238" alt="image" src="https://github.com/user-attachments/assets/f4865822-47a9-4fdb-986a-83808025b350" />
<!-- Replace with actual map from Fig 1/5 -->

## Project Overview
This repository contains the methodology and analysis for evaluating environmental changes in Pakistan's Indus River Basin using multi-satellite remote sensing data. The study focuses on:
- Vegetation Health Index (VHI) trends (1980-2023)
- Evapotranspiration (ET) patterns (1995-2023)
- Terrestrial Water Storage (GRACE WET) dynamics (2002-2024)
- Cross-correlation between climate variables

**Key Objectives**:
1. Assess drought impacts on vegetation in Baluchistan
2. Analyze ET variability across agricultural regions
3. Monitor groundwater depletion using GRACE data
4. Identify climate change indicators in the basin

## Data Sources
| **Dataset**         | **Source**                                                                 | **Temporal Coverage** |
|---------------------|----------------------------------------------------------------------------|----------------------|
| Vegetation Health Index | [NOAA STAR](https://www.star.nesdis.noaa.gov/smcd/emb/vci/VH/vh_adminMean.php) | 1980-2023            |
| Evapotranspiration  | [NASA EarthData](https://www.earthdata.nasa.gov/)                          | 1995-2023            |
| GRACE WET           | [JPL GRACE](https://grace.jpl.nasa.gov/data/data-analysis-tool/)           | 2002-2024            |

##  Methodology
1. **Data Processing**:
   - Anomaly calculation: `ET_anom = ET_i - ET_avg`
   - VHI computation: `VHI = α×VCI + (1-α)×TCI` (α=0.5)
   - GRACE TWS conversion to WET

2. **Trend Analysis**:
   - Sen's Slope estimator
   - Mann-Kendall test
   - Linear regression models

3. **Drought Classification**:
   - VHI < 30: Severe drought
   - 30 ≤ VHI < 40: Moderate drought
   - VHI ≥ 40: Healthy vegetation

## Key Findings
- **Vegetation Health**: Significant decline in Baluchistan (r = -0.31 with ET)
- **Water Storage**: 14.77 cm/year depletion trend (p < 0.01) 
- **Evapotranspiration**: 22% increase in peak summer ET since 2010
- **Drought Correlation**: Strong linkage between WET anomalies and VHI (Fig 23)

<img width="822" height="506" alt="image" src="https://github.com/user-attachments/assets/7e1fc5b6-b9d7-4e6f-a541-890a1d564f42" />
<!-- Replace with actual Fig 23 -->

## Project Structure
├── data/ # Processed datasets
├── scripts/
│ vhi_analysis.py # Vegetation health processing
│ grace_processing.R # WET calculations
│ correlation_analysis.ipynb
├── figures/ # Generated visualizations
├── references/ # Bibliographic resources
└── docs/ # Supplementary documentation

## References
1. Ahmed et al. (2020) - Divergence of PET trends [DOI](https://doi.org/10.1007/s00704-020-03195-3)
2. Salam et al. (2020) - GRACE groundwater analysis [DOI](https://doi.org/10.26480/bdwre.01.2020.10.15)
3. Naz et al. (2020) - Baluchistan drought trends [DOI](https://doi.org/10.3390/w12020470)

> **Note**: Full seminar paper available in `docs/RESE.pdf`




