# Addressing Uncertainty in Forecasting Extreme River Flows

### Sydney Mudd and Gabriel Sandoval

**Summary**: This research project utilizes deep learning to predict annual maximum discharge to reduce uncertainty for input into depth-damage functions for flood risk assessment, focusing on extrapolating onto ungauged sites.

**Problem Statement**: Can machine learning predictions of monthly maximum discharge improve uncertainty analysis for flood risk assessments at local sites without gauges?

**Data**
* [USGS Stream Gauge Data](https://waterdata.usgs.gov/nwis/rt)
* [NOAA Precipitation Data](https://www.ncei.noaa.gov/access/search/index)
* [NLCD Land Cover Data](https://www.usgs.gov/centers/eros/science/national-land-cover-database)
* [All Data + Model Outputs for Benchmarking](https://zenodo.org/records/15529996)

**Python Packages**
* os
* glob
* time
* random
* itertools
* reduce from functools
* deepcopy from copy
* pandas
* numpy
* geopandas
* Point from shapely.geometry
* tensorflow
* layers, callbacks, backend from tensorflow.keras
* StandardScaler from sklearn.preprocessing
* matplotlib.pyplot
* Line2D from matplotlib.lines

**Methods**

This project will use machine learning processes to predict annual maximum daily discharge at a theoretical USGS gauge site from gridded precipitation, land cover data, and catchment boundaries. Uncertainty will be integrated into assessment of probabilistic depth-damage curves of flood inundation estimates under these maximum daily discharge values. We will use data from nearby gauge sites to create a theoretical model (pretending no gauge exists), which will be tested against a model of an actual gauge on site to characterize the uncertainty of gauge prediction extrapolation.

**Expected outcomes**

* Predict the distribution of annual maximum discharge at multiple gauged sites in a chosen region for each year

* Calibrate uncertainty estimates

* Evaluate spatial generalizatio

* Produce time series for depth-damage propagation

* Small interactive map and/or plots for presentation

**References**
1. Frame, J. M., Kratzert, F., Klotz, D., Gauch, M., Shalev, G., Gilon, O., Qualls, L. M., Gupta, H. V., & Nearing, G. S. (2022). Deep learning rainfall–runoff predictions of extreme events. Hydrology and Earth System Sciences, 26(13), 3377–3392. https://doi.org/10.5194/hess-26-3377-2022 

2. USACE. (1996, August 1). Risk-Based Analysis for Flood Damage Reduction Studies. Hydrologic Engineering Center. https://www.hec.usace.army.mil/confluence/fdadocs/fdaum/references-152636922.html 

3. Zhao, G., Bates, P., Neal, J., & Pang, B. (2021). Design Flood Estimation for Global River Networks based on machine learning models. Hydrology and Earth System Sciences, 25(11), 5981–5999. https://doi.org/10.5194/hess-25-5981-2021
