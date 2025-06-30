# rsds_downscale

Aim: 
Downscale solar irradiance datasets to increase temporaral and spatial resolution.

Method:
Train multiple-linear regression (MLR) and machine learning (ML) models on SARAH-3 satellite observations (30 minute timesteps, 0.05 lat/lon grid).
https://wui.cmsaf.eu/safira/action/viewDoiDetails?acronym=SARAH_V003

Apply to CMIP6 style General Circulation Models (GCM) with low temporaral and spatial resolution (3 hourly mean time-steps, e.g. 2.5 lat/lon grid) and model bias issues to make the output usable, for example by PV energy models.

Code provided to:
* Read in SARAH-3 Surface incoming direct and total radiation data
* Read in CMIP6 GCM rsds data (total only)
* Train MLR and ML models to on SARAH-3 data, and test performance
* Apply MLR and ML models to CMIP6 GCM rsds data
