# Venice 1740 Transportation – Multimodal Traffic Assignment

This repository contains code and data for the analysis of multimodal (walking + traghetto/ferry) transportation in 18th-century Venice, using historical parish and property data from the 1740s. The main analysis implements traffic assignment models to understand cross-canal connectivity, demand, and economic implications of the traghetti network.


### Data files (in `rawdata/`)

- **1740_redrawn_parishes_cleaned_wikidata_standardised.geojson**  
  Cleaned and standardised parish boundary polygons for 1740 Venice (with Wikidata references).

- **catastici_1740_full_geojson_20240917.geojson**  
  Full spatial property records (Catastici) in GeoJSON format.

- **catastici_1740.csv**  
  Tabular property records with attributes (owners, property types, etc).

- **venice1740_parishes_processed.geojson**  
  Additional processed parish boundaries.

### Code

- **TAP-analysis.ipynb**  
  Jupyter notebook containing all code for:
    - Loading, processing, and visualizing parish and property data
    - Constructing the multimodal transport network
    - Running user equilibrium (UE) and system optimum (SO) assignments
    - Economic analysis (fare sensitivity, demand curves, revenue analysis)
    - Plotting and summarizing results


### Installing dependencies

All required Python packages are listed in `requirements.txt`.  
To install them, run: `pip install -r requirements.txt`

