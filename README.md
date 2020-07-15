ams-2013-2014-solar-energy
==========================

Read ModelDocumentation.odt

Licensed under GPL v2


Guidelines:

We used 3 fold contiguous validation (folds with years 1994-1998, 1999-2003, 2004-2007)
Our models used all features of forecast files without applying any preprocessing, so we took all 75 forecasts as features
For each station, we used the 75 forecasts of 4 nearest mesos. So with this we had 75x4 such features.
Besides those forecast features we had the following: month of the year, distance to each used meso, latitude difference to each meso. In total it was aproximately 320 features (with the forecast ones).
We trained 11 models for this, one for each forecast member (the 11 independent forecasts given)
We averaged those 11 models optmising MAE.
We used pythons GradientBoostedRegressor fo this task.
Thats it!
