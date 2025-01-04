Wollombi GIS Analysis
This repository contains GIS analysis tools for processing and analyzing Wollombi channel line data, gauging stations, and Digital Elevation Models (DEMs).
Project Structure
Copy
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
1.	Clone the repository
2.	Create virtual environment:
bash
Copy
python -m venv venv
venv\Scripts\activate
3.	Install requirements:
bash
Copy
pip install -r requirements.txt
Data Required
Place the following RAR files in the data/raw directory:
•	wollombi_channelline.rar
•	wollombi_gauging.rar
•	wollombi_DEM_10m.rar
•	wollombi_DEM_30m.rar
Usage
1.	Place raw data files in data/raw/
2.	Run the analysis:
bash
Copy
python src/main.py
Outputs
•	Vector data visualization: output/figures/vector_data.png
•	DEM comparison: output/figures/dem_comparison.png
•	Processed data: output/stats/gauging_stations_with_elevation.gpkg

