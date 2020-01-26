# Coronavirus Data Science

This repository contains Jupyter notebooks and python scripts for investigating the 2019 coronavirus outbreak. The goal is to serve as a starting point to track and analyze this outbreak. Getting an environment set up to read, analyze, and plot the outbreak data is not trivial. I am hoping this helps more people get started.

If you are a researcher, journalist, or other interested member of the public, please use this freely. If you are a data scientist, please fork and contribute back to build a better foundation for future research.

## Goals

1. Provide a framework and tools for loading outbreak data into Python
1. Easily visualize outbreak geodata
1. Facilitate collaboration among researchers

## Background

From the [CDC](https://www.cdc.gov/coronavirus/2019-ncov/about/index.html):

> 2019 Novel Coronavirus (2019-nCoV) is a virus (more specifically, a coronavirus) identified as the cause of an outbreak of respiratory illness first detected in Wuhan, China. Early on, many of the patients in the outbreak in Wuhan, China reportedly had some link to a large seafood and animal market, suggesting animal-to-person spread. However, a growing number of patients reportedly have not had exposure to animal markets, indicating person-to-person spread is occurring. At this time, it’s unclear how easily or sustainably this virus is spreading between people.  The latest situation summary updates are available on CDC’s web page 2019 Novel Coronavirus, Wuhan, China.

This is an emerging, rapidly evolving situation and CDC will provide [updated information](https://www.cdc.gov/coronavirus/2019-ncov/summary.html) as it becomes available.

## Data Sources

The data for tracking the 2019-nCoV outbreak is provided by the [Johns Hopkins Center for Systems Science and Engineering](https://systems.jhu.edu/research/public-health/ncov/). They have created an interactive [GIS Dashboard](https://gisanddata.maps.arcgis.com/apps/opsdashboard/index.html#/bda7594740fd40299423467b48e9ecf6).

> In response to this ongoing public health emergency, we developed an online dashboard (static snapshot shown below) to visualize and track the reported cases on a daily timescale; the complete set of data is downloadable as a google sheet. The case data visualized is collected from various sources, including WHO, U.S. CDC, ECDC China CDC (CCDC), NHC and DXY. DXY is a Chinese website that aggregates NHC and local CCDC situation reports in near real-time, providing more current regional case estimates than the national level reporting organizations are capable of, and is thus used for all the mainland China cases reported in our dashboard (confirmed, suspected, recovered, deaths). U.S. cases (confirmed, suspected, recovered, deaths) are taken from the U.S. CDC, and all other country (suspected and confirmed) case data is taken from the corresponding regional health departments. The dashboard is intended to provide the public with an understanding of the outbreak situation as it unfolds, with transparent data sources.

## Progress

The [Jan 25 Jupyter notebook](2019-nCoV%20Jan%2025.ipynb) works on a snapshot of data from Jan 25.
1. Load the coronavirus data into a Pandas DataFrame and plot
1. Load world, China, and US shapefiles into GeoDataFrames
1. Merge the coronavirus DataFrame with the GeoDataFrames
1. Display on a map

![Jan 25](images/jan25.png?raw=true "Jan 25 Outbreak Snapshot")

## Dependencies

[Jupyter Notebooks](https://jupyter.org/)

```
pip install pandas
pip install requests
pip install geopandas
pip install descartes
```

## Short-term Roadmap

1. Load and visualize a data snapshot ✅
1. Create a script to download new data from Google Sheets
1. Visualize time-series data

*contributions welcome!*

**Coronavirus Data Science** © 2019+, P. Daniel Tyreus, PhD Released under the [MIT] License.<br>

> Twitter [@tyreus](https://twitter.com/tyreus)

[MIT]: http://mit-license.org/

