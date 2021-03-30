# Check out the Building Data Genome 2 - the latest version that supercedes this one: https://github.com/buds-lab/building-data-genome-project-2

<!-- A repository of whole building electrical meters from non-residential buildings
============================== -->

![building data genome logo](https://raw.githubusercontent.com/buds-lab/the-building-data-genome-project/master/figures/buildingdatagenome1.png)

- Does your data science technique actually scale across hundreds of buildings?
-  Is it actually faster or more accurate?

These are questions that researchers should ask when developing data-driven methods. Building performance prediction, classi cation, and clustering algorithms are becoming an essential part of analysis for anomaly detection, control optimization, and demand response. But how do we actually compare, each individual technique against previously created methods?

The time-series data mining community identifed this problem as early as 2003: “Much of this work has very little utility because the contribution made”...“offer an amount of improvement that would have been completely dwarfed by the variance that would have been observed by testing on many real world datasets, or the variance that would have been observed by changing minor (unstated) implementation details.” ([Keogh, E. and Kasetty, S.: On the need for time series data mining benchmarks: A survey and empirical demonstration. Data Mining and Knowledge Discovery, 7(4):349–371, Oct. 2003.](https://link.springer.com/article/10.1023/A:1024988512476))

[They created the time-series data benchmarking set](http://www.cs.ucr.edu/~eamonn/time_series_data/). This data set enables testing of new techniques on an assortment of real world data sets. For commerical buildings data, we are doing the same!

## The need for Benchmarking Data Set for Non-residential Building Data Analytics

### Most of the existing building performance data science studies rely on each individual researcher creating their own methods, finding a case study data set and determining efficacy on their own. Not surprisingly, most of those researcher find positive, yet questionably meaningful results.

![old way](https://raw.githubusercontent.com/buds-lab/the-building-data-genome-project/master/figures/Oldway.png)


### Using a large, consistent benchmark data set from hundreds (or thousands) of buildings, a researcher can determine how well their methods actually perform across a heterogeneous data set. If multiple researcher use the same data set, then there can be meaningful comparisons of accuracy, speed and ease-of-use.

![new way](https://raw.githubusercontent.com/buds-lab/the-building-data-genome-project/master/figures/NewWay.png)

## Introducing the Building Data Genome Project
It is an open data set from 507 non-residential buildings that includes hourly whole building electrical meter data for one year. Each of the buildings has meta data such as  or area, weather, and primary use type. This data set can be used to benchmark various statistical learning algorithms and other data science techniques. It can also be used simply as a teaching or learning tool to practice dealing with measured performance data from large numbers of non-residential buildings. The charts below illustrate the breakdown of the buildings according to location, building industry, sub-industry, and primary use type.

![meta data](https://raw.githubusercontent.com/buds-lab/the-building-data-genome-project/master/figures/allbars.png)

### Please contribute new data sets or provide analysis examples in Jupyter or R markdown using the data


Citation of Data-Set
------------

[Clayton Miller, Forrest Meggers, The Building Data Genome Project: An open, public data set from non-residential building electrical meters, Energy Procedia, Volume 122, September 2017, Pages 439-444, ISSN 1876-6102, https://doi.org/10.1016/j.egypro.2017.07.400.](http://www.sciencedirect.com/science/article/pii/S1876610217330047) 

[ResearchGate](https://www.researchgate.net/publication/319507342_The_Building_Data_Genome_Project_An_open_public_data_set_from_non-residential_building_electrical_meters)

```
BibTex:
@article{Miller2017439,
title = "The Building Data Genome Project: An open, public data set from non-residential building electrical meters ",
journal = "Energy Procedia ",
volume = "122",
number = "",
pages = "439 - 444",
year = "2017",
note = "\{CISBAT\} 2017 International ConferenceFuture Buildings &amp; Districts – Energy Efficiency from Nano to Urban Scale ",
issn = "1876-6102",
doi = "https://doi.org/10.1016/j.egypro.2017.07.400",
url = "http://www.sciencedirect.com/science/article/pii/S1876610217330047",
author = "Clayton Miller and Forrest Meggers",
keywords = "Open Data",
keywords = "Non-Residential Building Meter Data",
keywords = "Benchmark Data Set",
keywords = "Big Data",
keywords = "Machine Learning ",
abstract = "Abstract As of 2015, there are over 60 million smart meters installed in the United States; these meters are at the forefront of big data analytics in the building industry. However, only a few public data sources of hourly non-residential meter data exist for the purpose of testing algorithms. This paper describes the collection, cleaning, and compilation of several such data sets found publicly on-line, in addition to several collected by the authors. There are 507 whole building electrical meters in this collection, and a majority are from buildings on university campuses. This group serves as a primary repository of open, non-residential data sources that can be built upon by other researchers. An overview of the data sources, subset selection criteria, and details of access to the repository are included. Future uses include the application of new, proposed prediction and classification models to compare performance to previously generated techniques. "
}
```

Getting Started
------------

We recommend you download the [Anaconda Python Distribution](https://www.continuum.io/downloads) and use Jupyter to get an understanding of the data.
- Raw temporal and meta data are found in `/data/raw/`

Example notebooks are found in `/notebooks/` -- a few good overview examples:
- [Meta data overview](https://github.com/buds-lab/the-building-data-genome/blob/master/notebooks/00_Meta%20Data%20Exploration.ipynb)
- [Temporal data overview](https://github.com/buds-lab/the-building-data-genome/blob/master/notebooks/00_Temporal%20Data%20Exploration%20--%20Subset.ipynb)

Publications or Projects that use this data-set:
------------

Please update this list if you add notebooks or R-Markdown files to the ``notebook`` folder.

- [Miller, Clayton. “Screening Meter Data: Characterization of Temporal Energy Data from Large Groups of Non-Residential Buildings.” ETH Zürich, 2017.](https://www.research-collection.ethz.ch/handle/20.500.11850/125778) - [ResearchGate](https://www.researchgate.net/publication/313720565_Screening_Meter_Data_Characterization_of_Temporal_Energy_Data_from_Large_Groups_of_Non-Residential_Buildings)
- [Temporal Data Mining Library for Buildings](https://github.com/buds-lab/temporal-features-for-nonres-buildings-library)


# Contact -- (Add yours if you contribute to the data set)
Dr. Clayton Miller
Building and Urban Data Science (BUDS) Group 
National University of Singapore
clayton@nus.edu.sg 
http://budslab.org/


Dr. Forrest Meggers
Cooling and Heating for Architecturally Optimized System (CHAOS) Lab
Princeton University
fmeggers@princeton.edu
http://chaos.princeton.edu/


Anjukan Kathirgamanathan
PhD Student, Energy Institute
University College Dublin
anjukan.kathirgamanathan@ucdconnect.ie
https://energyinstitute.ucd.ie/


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


Project Organization
------------
The MIT License (MIT)
Copyright (c) 2016, Clayton Miller

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

