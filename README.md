A repository of whole building electrical meters from non-residential buildings
==============================

Citation of Data-Set
------------

[Miller, C., Meggers, F., 2017. The Building Data Genome Project: An open public data set from non-residential building electrical meters. Presented at the CISBAT 2017, Lausanne, Switzerland.](https://www.researchgate.net/publication/314081046_The_Building_Data_Genome_Project_An_open_public_data_set_from_non-residential_buildings_electrical_meters)

Details of Project
------------
1. A temporal data set of hourly whole building electrical data for one year (8760 points per building for 507 buildings)
2. Meta data about each building including floor area, primary use type, weather file, and other various characteristics

Data Overview
------------
- Raw temporal and meta data are found in /data/raw/
- [Meta data overview](https://github.com/buds-lab/the-building-data-genome/blob/master/notebooks/00_Meta%20Data%20Exploration.ipynb)
- [Temporal data overview](https://github.com/buds-lab/the-building-data-genome/blob/master/notebooks/00_Temporal%20Data%20Exploration%20--%20Subset.ipynb)

Publications that use this data-set:
------------
[Miller, C., 2017. Screening Meter Data: Characterization of Temporal Energy Data from Large Groups of Non-Residential Buildings. ETH Zurich, Zurich, Switzerland.
](https://www.research-collection.ethz.ch/handle/20.500.11850/125778)

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │    │    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
                              generated with `pip freeze > requirements.txt`