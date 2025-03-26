# Chem 6010 Exam Spring 2025

In this exam, you should perform two tasks related to data series analysis. 

You should return your analysis in the form of a well-annotated Jupyter notebook (I recommend using [markdown](https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Working%20With%20Markdown%20Cells.html) to add formatted text) or in the format of a report. 

You must also submit all the codes and Juypter notebooks you use in your analysis. They should be given to me in such a form that I can run through the analysis myself and reproduce the results. 

Each student has their own independent datasets that are sampled differently. The dataset you should use will be given via email. 

## Task 1 

Datasets: `Datasets-#/Task-1/`

In this task, you are given 20 time series sampled independently from two distinct models (i.e., random processes) that we call models **A** and **B**. The two models differ in their mean/average value and their correlation. We do not know from which model each dataset has been sampled. 

Your overall task is to identify for each dataset which model it belongs to, **A** or **B**. 

Note that the dataset filenames are identified with a random five-digit integer that has no meaning other than giving each data file a unique name. 

To achieve your overall task of classifying the datasets, you can think about performing some of the tasks you perform in the practice dataset and compare the datasets, including:
- Visualize and plot the time series.
- Estimate the densities using discrete histograms and kernel density estimation.
- Calculate the average (i.e., mean) and standard deviation. 
- Calculate and plot the autocorrelation function.
- Use block averaging to estimate the mean (i.e., average) and the standard error of the mean.
- Estimate the autocorrelation times
For example, I would want to see a graph comparing the means for the different datasets, with the standard error of the mean shown as an error bar. You can also perform any other analysis that you think is useful to help with the overall task.

## Task 2

Datasets: `Datasets-#/Task-2/`

In this task, you are given a time series sampled from a two-dimensional distribution $P(x,y)$. You have three different time series sampled from independent runs. 

You should analyze the three times series, including: 
- Plot and visualize the time series of the $x$ and $y$ variables. 
- Estimate the one-dimensional densities $P(x)$ and $P(y)$ by using discrete histograms or kernel density estimation (KDE).
- Estimate the two-dimensional density $P(x,y)$ by using histogramming or KDE.
- Consider the correlation between the $x$ and $y$ variables by visualizing the two-dimensional density.

You will notice that the two-dimensional distribution $P(x,y)$ is composed of two modes (i.e., density peaks or metastable states). Estimate the averages and standard deviations of the $x$ and $y$ values separately for each mode and use block averaging to estimate the standard error of the mean. 

Use the [mutual information](https://en.wikipedia.org/wiki/Mutual_information) $I(X,Y)$ (see Eq 2) to quantify the correlation between the two variables. 

Another useful metric is the following distance function $D$, which is a variant of the mutual information normalized over the range $[0,1]$
```math
D = 1 - \frac{I(X,Y)}{H(X,Y)}
```
where $H(X,Y)$ is the joint entropy, defined as 
```math
H(X,Y) = -\int P(x,y) \, \log P(x,y) dx dy
```
This metric has the value of one if there is no correlation and goes to zero as the correlation increases. 

Implement this distance function and use it to quantify the correlation between the two variables further. 

Optional: you can also consider the correlation within each of the two modes by considering the distance function for them separately. 

Note that the $x$ and $y$ variables are labeled as `p.x` and `p.y` in the data files. 

Note that the dataset filenames are identified with a random four-digit integer that has no meaning other than giving each data file a unique name. 


