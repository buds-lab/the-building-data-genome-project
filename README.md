<!-- A repository of whole building electrical meters from non-residential buildings
============================== -->

![building data genome logo](https://raw.githubusercontent.com/buds-lab/the-building-data-genome-project/master/figures/buildingdatagenome1.png)

- Does your data science technique actually scale across hundreds of buildings?
-  Is it actually faster or more accurate?

These are questions that researchers should ask when developing data-driven methods. Building performance prediction, classi cation, and clustering algorithms are becoming an essential part of analysis for anomaly detection, control optimization, and demand response. But how do we actually compare, each individual technique against previously created methods?

The time-series data mining community identifed this problem as early as 2003: “Much of this work has very little utility because the contribution made”...“offer an amount of improvement that would have been completely dwarfed by the variance that would have been observed by testing on many real world datasets, or the variance that would have been observed by changing minor (unstated) implementation details.” ([Keogh, E. and Kasetty, S.: On the need for time series data mining benchmarks: A survey and empirical demonstration. Data Mining and Knowledge Discovery, 7(4):349–371, Oct. 2003.](https://link.springer.com/article/10.1023/A:1024988512476))

[They created the time-series data benchmarking set](http://www.cs.ucr.edu/~eamonn/time_series_data/). This data set enables testing of new techniques on an assortment of real world data sets. For commerical buildings data, we are doing the same!

### Most of the existing building performance data science studies rely on each individual researcher creating their own methods, finding a case study data set and determining efficacy on their own. Not surprisingly, most of those researcher find positive, yet questionably meaningful results.

![old way](https://raw.githubusercontent.com/buds-lab/the-building-data-genome-project/master/figures/Oldway.png)


### Using a large, consistent benchmark data set from hundreds (or thousands) of buildings, a researcher can determine how well their methods actually perform across a heterogeneous data set. If multiple researcher use the same data set, then there can be meaningful comparisons of accuracy, speed and ease-of-use.

![new way](https://raw.githubusercontent.com/buds-lab/the-building-data-genome-project/master/figures/NewWay.png)

## Introducing the Building Data Genome Project
It is an open data set from 507 non-residential buildings that includes hourly whole building electrical meter data for one year. Each of the buildings has meta data such as  or area, weather, and primary use type. This data set can be used to benchmark various statistical learning algorithms and other data science techniques. It can also be used simply as a teaching or learning tool to practice dealing with measured performance data from large numbers of non-residential buildings. The charts below illustrate the breakdown of the buildings according to location, building industry, sub-industry, and primary use type.

![meta data](https://raw.githubusercontent.com/buds-lab/the-building-data-genome-project/master/figures/allbars.png)

## Please contribute new data sets or provide analysis examples in Jupyter or R markdown using the data


Citation of Data-Set
------------

[Miller, C., Meggers, F., 2017. The Building Data Genome Project: An open public data set from non-residential building electrical meters. Presented at the CISBAT 2017, Lausanne, Switzerland.](https://www.researchgate.net/publication/314081046_The_Building_Data_Genome_Project_An_open_public_data_set_from_non-residential_buildings_electrical_meters)

<!-- Details of Project
------------
1. A temporal data set of hourly whole building electrical data for one year (8760 points per building for 507 buildings)
2. Meta data about each building including floor area, primary use type, weather file, and other various characteristics -->

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