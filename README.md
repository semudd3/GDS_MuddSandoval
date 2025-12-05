# Addressing Uncertainty in Forecasting Extreme River Flows

### Sydney Mudd and Gabriel Sandoval

**Summary**: This research project utilizes deep learning to predict monthly maximum discharge to reduce uncertainty for input into depth-damage functions for flood risk assessment, focusing on extrapolating onto ungauged sites.

**Problem Statement**: Can machine learning predictions of monthly maximum discharge improve uncertainty analysis for flood risk assessments at local sites without gauges?

**Data**
* [CAMELS Dataset - Catchment Attributes and MEteorology for Large-sample Studies](https://zenodo.org/records/15529996)

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

This project will use machine learning processes to predict monthly maximum discharge at a theoretical USGS gauge site from the CAMELS Dataset. Uncertainty will be integrated into assessment of probabilistic depth-damage curves of flood inundation estimates under these maximum daily discharge values. We will use data from nearby gauge sites to create a theoretical model (pretending no gauge exists), which will be tested against a model of an actual gauge on site to characterize the uncertainty of gauge prediction extrapolation.

**Expected outcomes**

* Predict the distribution of annual maximum discharge at multiple gauged sites in a chosen region for each year

* Calibrate uncertainty estimates

* Evaluate spatial generalization

* Produce time series results of streamflow plots

* Map showing geographical characteristics of data

**References**
1. Addor, N., Newman, A. J., Mizukami, N., & Clark, M. P. (2017). The CAMELS data set: Catchment attributes and meteorology for large-sample studies. Hydrology and Earth System Sciences, 21(10), 5293–5313. https://doi.org/10.5194/hess-21-5293-2017

2. Frame, J. M., Kratzert, F., Klotz, D., Gauch, M., Shalev, G., Gilon, O., Qualls, L. M., Gupta, H. V., & Nearing, G. S. (2022). Deep learning rainfall–runoff predictions of extreme events. Hydrology and Earth System Sciences, 26(13), 3377–3392. https://doi.org/10.5194/hess-26-3377-2022 

3. Gacu, J. G., Monjardin, C. E. F., Mangulabnan, R. G. T., & Mendez, J. C. F. (2025). Application of artificial intelligence in hydrological modeling for streamflow prediction in ungauged watersheds: A review. Water, 17, 2722. https://doi.org/10.3390/w17182722 

4. Kratzert, F., Klotz, D., Herrnegger, M., Sampson, A. K., Hochreiter, S., & Nearing, G. S. (2019). Toward improved predictions in ungauged basins: Exploiting the power of machine learning. Water Resources Research, 55(12), 11344–11354. https://doi.org/10.1029/2019WR026065

5. Kunkel, K. E., Easterling, D. R., Ballinger, A., Bililign, S., Champion, S. M., Corbett, D. R., Dello, K. D., Dissen, J. P., Lackmann, G. M., Luettich, R. A., Jr., Perry, L. B., Robinson, W. A., Stevens, L. E., Stewart, B. C., & Terando, A. J. (2020). North Carolina Climate Science Report. North Carolina Institute for Climate Studies. https://ncics.org/nccsr

6. North Carolina Governor’s Office. (2025, August 5). Governor Stein declares Tropical Storm Chantal Type I state disaster, activates individual assistance [Press release]. https://governor.nc.gov/news/press-releases/2025/08/05/governor-stein-declares-tropical-storm-chantal-type-i-state-disaster-activates-individual-assistance

7. U.S. Army Corps of Engineers. (2015). North Atlantic Coast Comprehensive Study: Physical depth–damage function summary report. Author. https://www.nad.usace.army.mil/Portals/40/docs/NACCS/10A_PhysicalDepthDmgFxSummary_26Jan2015.pdf

8. Wing, O. E. J., Pinter, N., Bates, P. D., & Kousky, C. (2020). New insights into U.S. flood vulnerability revealed from flood insurance big data. Nature Communications, 11, Article 1444. https://doi.org/10.1038/s41467-020-15264-2