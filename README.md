# chimaliro-schoolsite-accessibility

GIS project for site selection
Data source: Malawi OpenStreetMap
Projection used WGS 87 EPSG:32736 UTM ZONE 36 for map projected area
Projection for Web Map WGS 84 EPSG: 4326

## 1. Project Overview

This project uses Geographic Information Systems (GIS) and spatial analysis techniques to identify potentially suitable locations for establishing new schools within Chimaliro Traditional Authority (TA), Malawi.

The analysis considers the spatial distribution of existing schools, road networks, protected areas, and the geographical boundaries of Chimaliro Traditional Authority.

The main objective is to support evidence-based educational infrastructure planning by identifying locations that meet selected spatial suitability criteria and could potentially improve access to educational facilities.

### Objectives

- Identify potential locations for establishing new schools.
- Evaluate the spatial relationship between existing schools and potential school sites.
- Consider accessibility in relation to available road networks.
- Exclude areas that fall within protected areas.
- Produce maps showing the distribution of potentially suitable locations.

## 2. Ministry of Education School Site Selection Criteria

The analysis follows spatial considerations informed by the Ministry of Education's school site selection requirements.

The criteria considered in this project include:

1. **Accessibility:** Potential school locations should have reasonable access to existing road networks.
2. **Distance from existing schools:** New school locations should avoid unnecessary proximity to existing educational facilities.
3. **Protected areas:** Locations within designated protected areas should be excluded from potential school development.

**Note:** The final criteria and distance thresholds should be updated to match the actual Ministry of Education guidelines used in this study.

## 3. Data Sources

The analysis uses the following spatial datasets:

| Dataset                        | Description                        | Purpose                                 |
| ------------------------------ | ---------------------------------- | --------------------------------------- |
| Traditional Authority Boundary | Chimaliro TA boundary              | Defines the study area                  |
| Existing Schools               | Locations of existing schools      | Evaluates proximity to existing schools |
| Road Network                   | Road network within the study area | Evaluates accessibility                 |
| Protected Areas                | Protected area boundaries          | Identifies restricted locations         |

All datasets should be accompanied by their original source organizations and download links where available.

## 4. Methodology

The project uses Python-based geospatial analysis, primarily through GeoPandas.

The main analytical stages include:

1. Loading and preparing the spatial datasets.
2. Filtering the Traditional Authority boundary to obtain Chimaliro.
3. Clipping relevant spatial datasets to the study area.
4. Converting datasets into a suitable projected coordinate reference system (EPSG:32736).
5. Performing spatial operations to evaluate the selected suitability criteria.
6. Identifying locations that satisfy the required spatial conditions.
7. Visualizing the results using static and interactive maps.

## 5. Software and Libraries

The project uses the following tools:

- Python
- Jupyter Notebook
- GeoPandas
- Pandas
- NumPy
- Matplotlib
- Shapely
- Folium

## 6. Summary of Results

The analysis identifies potentially suitable locations for establishing new schools within Chimaliro Traditional Authority.

The resulting spatial dataset represents areas that satisfy the three spatial conditions considered in the analysis.

The results are intended to support educational infrastructure planning and provide a geographical basis for further investigation.

**Important:** The identified locations represent preliminary spatial suitability results. Actual land availability, ownership, terrain conditions, and adequacy of land for school construction require additional assessment.

### Key Findings

The following statistics should be added after completing the analysis:

- Total number of suitable locations: 15
- Number of existing schools: 29
- Study area: Chimaliro Traditional Authority

## 7. Map Preview

The following figure provides a preview of the static school site suitability map.

![Chimaliro School Site Suitability Map](outputs/suitable_areas_map.png)

The map illustrates the study area, existing schools, road network, protected areas, and identified potentially suitable locations.

## 8. Project Structure

```text
chimaliro-schoolsite-accessibility/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   └── school_site_analysis.ipynb
│
├── outputs/
│   ├── suitable_areas_map.png
│   └── chimaliro_school_suitability.html
│
├── README.md
└── LICENCE

```

## 9. Reproducing the Analysis

To reproduce the analysis:

### Step 1: Clone the repository

```bash
git clone https://github.com/Tedson-Jaffet/chimaliro-schoolsite-accessibility.git
```

### Step 2: Navigate into the project directory

```bash
cd chimaliro-schoolsite-accessibility
```

### Step 3: Install the required libraries

```bash
pip install geopandas pandas numpy matplotlib shapely folium jupyter
```

### Step 4: Open Jupyter Notebook

```bash
jupyter notebook
```

### Step 5: Run the analysis

Open:

`notebooks/school_site_analysis.ipynb`

Run the notebook cells sequentially to reproduce the spatial analysis and generate the maps.

Ensure that the required datasets are available in their expected directories.

## 10. Limitations

The analysis identifies potential locations based on selected spatial criteria. It does not independently establish whether a site is legally available, physically suitable for construction, or large enough to accommodate the required school infrastructure.

Field verification and additional assessments are therefore recommended before making final site selection decisions.

## 11. Author

**Tedson Jaffet**

Geo-information and Earth Observation Student

Malawi University of Science and Technology (MUST)

GitHub: [Tedson-Jaffet](https://github.com/Tedson-Jaffet)

---

_This project demonstrates the application of GIS and Python-based spatial analysis to support evidence-based educational infrastructure planning._
