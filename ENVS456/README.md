# ENVS456 - Geographic Information Systems (GIS)

## Course Overview

ENVS456 is a Geographic Information Systems course that focuses on web-based GIS applications, spatial data analysis, and interactive mapping techniques. This course combines theoretical knowledge with practical hands-on experience using modern GIS tools and technologies.

## Learning Objectives

- Understand the fundamentals of Geographic Information Systems
- Learn web-based mapping and spatial data visualization
- Develop skills in interactive dashboard creation
- Explore spatial data architectures and web services
- Work with OpenStreetMap data and advanced mapping techniques
- Create interactive geospatial applications

## Course Structure

### Labs
The course includes several practical lab sessions covering:

- **Week 01**: Introduction to GIS concepts (`w01_intro.ipynb`)
- **Week 02**: Basic mapping and visualization (`w02_maps.ipynb`)
- **Week 03**: Web architecture for GIS (`w03_webArch.ipynb`)
- **Week 04**: Spatial data architecture (`w04_dataArch.ipynb`)
- **Week 05**: Interactive mapping (`w05_interactive.ipynb`)
- **Week 07**: OpenStreetMap integration (`w07_OSM.ipynb`)
- **Week 08**: Dashboard development (`w08_dashboards.ipynb`)
- **Week 09**: Advanced GIS techniques (`w09_advanced.ipynb`)
- **Lecture 08**: Additional content (`lecture08.ipynb`)

### Assignments
The course includes two major assignments:

- **AS01**: Foundational GIS assignment
- **AS02**: Advanced dashboard and visualization project

## Environment Setup

### Prerequisites
- Python 3.11.5 or later
- Conda package manager

### Installation
1. Navigate to the ENVS456 directory:
   ```bash
   cd ENVS456
   ```

2. Create the conda environment from the provided YAML file:
   ```bash
   conda env create -f envs456.yml
   ```

3. Activate the environment:
   ```bash
   conda activate gis
   ```

### Key Dependencies
The course environment includes essential GIS and data science libraries:

- **Spatial Analysis**: GeoPandas, Shapely, Fiona, Rasterio
- **Mapping**: Folium, Cartopy, Contextily
- **Data Processing**: Pandas, NumPy, SciPy
- **Visualization**: Matplotlib, Plotly, Bokeh, Seaborn
- **Interactive Tools**: Jupyter Lab, Panel, HoloViews
- **Web GIS**: OSMnx for OpenStreetMap analysis
- **Machine Learning**: Scikit-learn

## Directory Structure

```
ENVS456/
├── README.md              # This file
├── envs456.yml           # Conda environment specification
├── assignments/          # Course assignments
│   ├── AS01/            # Assignment 1
│   └── AS02/            # Assignment 2
├── labs/                # Weekly lab notebooks
├── labs_img/            # Images and figures for labs
└── data/                # Course datasets
```

## Getting Started

1. Set up the conda environment using the instructions above
2. Launch Jupyter Lab:
   ```bash
   jupyter lab
   ```
3. Start with the introduction notebook: `labs/w01_intro.ipynb`
4. Progress through the weekly labs in sequence
5. Complete assignments as scheduled

## Additional Resources

- Course data is stored in the `data/` directory
- Lab images and figures are available in `labs_img/`
- Cache files for improved performance are stored in `labs/cache/`

## Support

For technical issues with the GIS environment or course materials, refer to the official course documentation or contact the instructor.