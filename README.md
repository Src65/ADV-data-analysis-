# ADV-analysis-
Code for ADV (acoustic doppler profiler) data processing. Used for data collected at Stillwater Cove 07-09, 2017 in and out of kelp beds. 
By Steven Cunningham, Moss Landing Marine Labs.  

**Libraries needed** 
1. import numpy as np
1. from matplotlib import pyplot as plt
1. from scipy.signal import periodogram
1. import pandas as pd
1. import csv
1. from physoce import tseries as ts - This is a code from Tom Connolly 
1. %matplotlib notebook

**Load 2 files from ADV**
-.dat & .sen

**Time stamp**
 -The duration you are looking for in the data will be dictated by start and end time = runindex 
 
 **Plot the data**
 - It's recomended that you plot the variable of interest to make sure the data is noise and anomaly free
 
 **PCA the velocity**
 - This simply rotates the axis to capture the highest variation ie. the direction of highest velocity. 
 
 **Save outputs**
 -The first time stamp runs cell 81. 
 -Cell 81 should be skipped in all time intervals of the same file after the first time interval. Instead, run cell 82 to append to the same .csv file output. 
