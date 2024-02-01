# Time Series Data Extract from Multi-dimensional Raster Dataset for Statistical Analysis

1. Background of the project:

These scripts contain the algorithms to evaluate BETHY/DLR model outputs (GPP & NPP) against the outputs of other process-based ecosystem models (LPJ-GUESS and CASA). I created these scripts using Python during my internship project at the German Aerospace Agency (DLR). At DLR, I worked with the second version of the BETHY/DLR ecosystem model's outputs to evaluate the model performance. This task contributed to the ongoing updating process of the model before releasing its second version's data.

2. Multi-dimensional raster data:

Multi-dimensional raster data contains spatial and temporal dimensions for every variable. The standard data formats for multi-dimensional rasters are NetCDF and HDF. The "xarray" and "rioxarray" Python libraries are used to process these raster data types. The "rioxarray" is built on top of "xarray" library integrating "rasterio" library.

A layer of sample points has been created using systematic random sampling over the study area to extract time series data for different sample points. The point layer is a KML file that underwent processing to match the spatial reference system of the raster layers.

3. Workflow: what can these codes do?

These scripts contain the workflow from reading, stacking, temporal unit changes, reprojection of point features, extracting data from raster layers and storing in a tuple, performing statistical analysis (i.e., RMSE, r-square estimation), and plotting the time series data.

Are you curious to learn about my internship project? You can read the report from "InternReport_Saiful_s6048943".

![pt3](https://github.com/mds-islam/Multi-dimensional-Raster-TimeSeries/assets/158111120/84e06dc7-1b94-4fee-974e-4c0813be7b7b)

Figure: Comparison between GPP from BETHY/DLR and LPJ-GUESS models (Lon: 5.34E, Lat: 44.29N).

![pt3](https://github.com/mds-islam/Multi-dimensional-Raster-TimeSeries/assets/158111120/f58a86e3-b014-486d-b3ba-386734b1ae1d)

Figure: Comparison between NPP from BETHY/DLR and CASA models (Lon: 10.94E, Lat: 11.62N)

