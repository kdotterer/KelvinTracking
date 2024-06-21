# KelvinTracking
Tracks filteredTb CCKW centers as they propagate. Adapted from AEW tracking as described in Lawton et al., 2022.

Here "center" is a loose term. This tracker does not track a center of circulation nor is it intended to be used to treat CCKWs as point systems. 

This tracker was written with the intention of seperating CCKW strength from location and number. Previous CCKW climatologies rely on statistical methods such as variance to determine CCKW activity. However, it is impossible to seperate strength from number using variance. High variance could be created by one especially strong system or several moderate ones. Variance also requires a climatology with a long timespan; too few datapoints leaves variance highly noisy. Tracking individual waves allows for independance from wave strength (outside of a minimum threshold), while also allowing for short climatologies. 

This tracker identifies a wave "center" in both longitude and latitude. 

Current tracker is written for the merged CLAUS-IR dataset. It does not work for longitudes of -180-180 in its current form. 
Tracker is untested for CCKW identification methods other than Kelvin-filtered Tb, as described in Wheeler and Kiladis, 1999. 

Copyright Krista Dotterer
kdotterer@albany.edu
