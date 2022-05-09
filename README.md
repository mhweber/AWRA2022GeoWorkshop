# AWRA 2022 GeoWorkshop

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/cheginit/AWRA2022GeoWorkshop/HEAD)

Material for [AWRA2022](https://www.awra.org/Members/Events_and_Education/Events/2022_GIS_Conference/2022_GWTC_Workshops.aspx)
Geospatial R and Python Workshop.

## Getting Started

For working with R, you can use [RStudio](https://www.rstudio.com/) and you will
need the following libraries installed:

```r
library(sf)
library(ggplot2)
library(dplyr)
library(readr)
library(knitr)
library(rnaturalearth)
library(stringr)
library(osmdata)
library(mapview)
library(dataRetrieval)
library(terra)
library(stars)
library(remotes)
library(elevatr)
install_github("mhweber/awra2020spatial")
library(awra2020spatial)
install_github("mhweber/Rspatialworkshop")
library(Rspatialworkshop)
```

For running with Python notebooks you can use a combination of
[Mambaforge](https://github.com/conda-forge/miniforge) and your favorite
IDE such as VS Code or Jupyter Lab. For example, you can install it on OSX
as follows:

```bash
APP_DIR="~/.local/apps" && \
wget https://github.com/conda-forge/miniforge/releases/latest/download/Mambaforge-MacOSX-x86_64.sh && \
chmod +x Mambaforge-MacOSX-x86_64.sh && \
bash ./Mambaforge-MacOSX-x86_64.sh -b -p ${APP_DIR}/mambaforge && \
rm -f Mambaforge-MacOSX-x86_64.sh
```

where `APP_DIR` can be set to any location of interest.

After installing `mambaforge` you can create a Python environment as follows:

```bash
git clone https://github.com/mhweber/AWRA2022GeoWorkshop && \
cd AWRA2022GeoWorkshop && \
mamba env create -f environment.yml
```

Now a new environment called `awra2022` is created that can be loaded from your IDE.
You can also use the Binder service by clicking on the Binder badge to launch a Jupyter Lab
instance with all the required Python libraries installed.

## Resources

Here is a list of some useful geospatial tools and resources:

* General:
  * [Awesome Geospatial](https://github.com/sacridini/Awesome-Geospatial):
    A Long list of geospatial analysis tools.
* R:
  * [HydroData](https://mikejohnson51.github.io/HydroData/):
    An open-source tool that is designed
    to help (1) find, (2) get, (3) visualize, and (4) format disparate earth systems data through
    a core language (R).
  * [EPA R User Group R Spatial Workshop](https://mhweber.github.io/R-User-Group-Spatial-Workshop-2021/):
    Workshop material from 2021 EPA R User Group meeting on spatial analysis in R
  * [AWRA 2020 R Spatial Workshop](https://mhweber.github.io/AWRA_2020_R_Spatial/):
    Material from 2020 AWRA R Spatial Workshop
  * [Geocomputation With R](https://geocompr.robinlovelace.net/):
    One of the best overall resources for working with spatial data in R
  * [nhdplusTools](https://usgs-r.github.io/nhdplusTools/):
    R package for manipulation of hydrographic data using the NHDPlus data model
  * [Hydroinformatics in R](https://vt-hydroinformatics.github.io/):
    Extensive Notes and exercises for a course on data analysis techniques in hydrology using the programming language R
  * [r-spatial](https://github.com/r-spatial):
    Suite of fundamental packages for working with spatial data in R
* Python:
  * [PyNHD](https://docs.hyriver.io/en/latest/readme/pynhd.html):
    Navigate and subset NHDPlus (MR and HR) dataset using web services.
  * [Py3DEP](https://docs.hyriver.io/en/latest/readme/py3dep.html):
    Access topographic data through National Map's 3DEP web service.
  * [PyGeoHydro](https://docs.hyriver.io/en/latest/readme/pygeohydro.html):
    Access NWIS, NID, WQP, HCDN 2009, NLCD, CAMELS, and SSEBop databases.
  * [PyDaymet](https://docs.hyriver.io/en/latest/readme/pydaymet.html):
    Access Daymet for daily climate data both single pixel and gridded.
  * [Python Geospatial](https://github.com/giswqs/python-geospatial):
    A collection of Python packages for geospatial analysis with binder-ready notebook examples.
  * [xarray](https://xarray.pydata.org/en/stable/):
    An open-source project and Python package that makes working with labeled multi-dimensional
    arrays simple, efficient, and fun!
  * [rioxarray](https://corteva.github.io/rioxarray/stable/index.html):
    Rasterio xarray extension.
  * [GeoPandas](https://geopandas.org/en/stable/):
    An open-source project to make working with geospatial data in python easier.
  * [Proplot](https://proplot.readthedocs.io/en/stable/):
    A succinct `matplotlib` wrapper for making beautiful, publication-quality graphics.
  * [OSMnx](https://github.com/gboeing/osmnx):
    A Python package that lets you download and analyze geospatial data from OpenStreetMap.
  * [Xarray Spatial](https://xarray-spatial.org/master/index.html):
    Implements common raster analysis functions using `numba` and provides an easy-to-install, easy-to-extend codebase for raster analysis.
  * [Datashader](https://datashader.org/):
    Accurately render even the largest data
