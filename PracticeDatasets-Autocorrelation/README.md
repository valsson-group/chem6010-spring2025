# Datasets Autocorrelation 

This folder contains four datasets with time series sampled from four different models. 
- All the models have the same mean and should have very similar standard deviations.
- For two of the models, there is no correlation between data points.
- For the other two models, the data points are correlated to a certain degree but differ in the correlation.
- The data points are sampled with a frequency of 0.1 ns. 

To practice, you should perform the following tasks for the different datasets:
- Visualize and plot the time series (ensure the time axis is correct).
- Estimate the densities using discrete histograms and kernel density estimation.
- You should compare the results obtained with the discrete histogram and KDE to ensure you are using appropriate bandwidth parameters in the KDE. It is easy to oversmooth the KDE densities using bandwidth parameters that are too large. 
- Calculate the average (i.e., mean) and standard deviation. 
- Calculate and plot the autocorrelation function.
- Use block averaging to estimate the standard error of the mean.
- Estimating the autocorrelation times (keep in mind that the data points are sampled with a frequency of 0.1 ns)
- Based on your results, what can you deduce about the different models?
  - Which of them has uncorrelated data points?
  - What can you determine about the difference between the two models with uncorrelated data points?
  - Which one of the models has the longest autocorrelation time?
 
    
