# heart-rate-monitors
Jupyter notebook to compare heart rate data between devices with Python.

# How It Works
This notebook uses matplotlib.pyplot, numpy, pandas, regex, scipy.stats, sklearn.metrics, and xml to clean, wrangle and analyze heart rate data from both Polar H10 chest-strap monitor and Apple Watch Series 8.  

The main steps of the notebook: 
1. Import Watch & Polar data as DataFrames
2. Wrangle both datasets, leveraging timestamps, regex and pandas filtering.
3. Reconcile Polar and Watch data, keeping only the data points with synched timestamps.
4. Calculate sampling frequencies for both devices.
5. Plot rolling mean heart rate graphs for each training date.
6. Filter dateframes by heart rate zones and analyze per zone.
7. Plot Bland-Altman agreement plots between devices per zone.   
8. Explore mean absolute error, pearson correlation and intraclass correlation coefficient for each heart rate zone.

# Usage (Mac) 
This notebook ships assuming the following folder structure. You are welcome to modify this for your needs within the notebook.

     ├── heart-rate-monitors (repo)
     │   ├── analysis.ipynb
     │   ├── data
     │   │   ├── polar
     │   │   ├── watch
     │   ├── figs        
