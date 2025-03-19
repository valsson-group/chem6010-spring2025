# Datasets 2D Correlation 

This folder contains a dataset of a time series sampled from a two-dimensional distribution $P(x,y)$. 

To practice, you should try the following task:
- Plot and visualize the time series of the $x$ and $y$ variables (ensure to have the correct time axis). What do you observe?  
- Estimate the one-dimensional densities $P(x)$ and $P(y)$ by using histogramming and kernel density estimation.
  - Here, you should compare the histogram to the KDE to determine the appropriate bandwidth parameters.
- Estimate the two-dimensional density $P(x,y)$ by using histogramming or KDE.
  - For the KDE, you should use the appropriate bandwidths estimated from the one-dimensional densities.
- Consider the correlation between the $x$ and $y$ variables by visualizing the two-dimensional density.
- Quantify the correlation between the two variables by calculating the [mutual information](https://en.wikipedia.org/wiki/Mutual_information) (see Eq 2 there).
  - Here, you should estimate the distributions using KDE.
  - To integrate the mutual information, you must ensure that all the KDE grids have the same range. This can be done using KDE in sklearn.
 
 
