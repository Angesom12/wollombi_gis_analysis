# wollombi_gis_analysis
This repository provides Python tools for analyzing GIS data of the Wollombi region, focusing on channel networks, gauging stations, and DEMs (10m/30m). It processes vector/raster data, automates visualization, and ensures data integrity. Technologies include GeoPandas, Rasterio, GDAL, and more. See README.md for details.

Project Structure

wollombi_gis_analysis/
│
├── data/
│   ├── raw/                  # Original RAR files
│   └── processed/            # Processed GIS data
│
├── src/
│   ├── data_loader.py       # Functions for loading RAR/GIS data
│   ├── analysis.py          # Analysis functions
│   ├── visualization.py     # Plotting functions
│   └── main.py             # Main script
│
├── notebooks/               # Jupyter notebooks for exploration
│
├── output/
│   ├── figures/            # Generated plots
│   ├── maps/              # Generated maps
│   └── stats/             # Statistical outputs
│
└── tests/                 # Unit tests


Setup

1.Clone the repository
2.Create virtual environment:

python -m venv venv
venv\Scripts\activate

3. Install requirements:

   pip install -r requirements.txt


Data Required
Place the following RAR files in the data/raw directory:

wollombi_channelline.rar
wollombi_gauging.rar
wollombi_DEM_10m.rar
wollombi_DEM_30m.rar

Usage

Place raw data files in data/raw/
Run the analysis:

python src/main.py


Outputs

Vector data visualization: output/figures/vector_data.png
DEM comparison: output/figures/dem_comparison.png
Processed data: output/stats/gauging_stations_with_elevation.gpkg
