# Installing Python Packages

In the COVID-19 critical trends geospatial analysis we used a pre-formatted geoJSON file to create a choropleth map that showed how the COVID-19 outbreak spread across the US. Here we'll format our own geoJSON file from a [shapefile](https://www.gislounge.com/what-is-a-shapefile/), a popular option for geospatial data sharing. To work with and view our shapefiles similarly to how we work with and view our pandas data frames, we'll need to download **`geopandas`** and **`descartes`**in our Anaconda business-analytics virtual environment. 

{% hint style="info" %}
**If you're working in Google Colab**, you'll need to import `geopandas`, `descartes`, and `rtree` before you can start writing code. Install these with: 

```text
!apt update
!apt upgrade
!apt install gdal-bin python-gdal python3-gdal 
# Install rtree - Geopandas requirment
!apt install python3-rtree 
# Install Geopandas
!pip install git+git://github.com/geopandas/geopandas.git
# Install descartes - Geopandas requirment
!pip install descartes 
```

in the first cell.
{% endhint %}

{% hint style="info" %}
 **If you don't install packages through the Anaconda interface**, try to install `geopandas` with [**`conda`**](https://anaconda.org/conda-forge/geopandas). The `geopandas` packages depends on earlier versions of a couple of other packages \(`fiona` and `shapely`\), so if you install this with `pip`, follow [these instructions](https://geopandas.org/install.html) closely, or you'll encounter errors.
{% endhint %}

