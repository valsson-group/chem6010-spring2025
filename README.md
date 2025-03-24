# Chem6010 Exam Spring 2025

In this exam, you should perform two tasks related to data series analysis. 

You should return your analysis in the form of a well-annotated Jupyter notebook (I recommend using [markdown](https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Working%20With%20Markdown%20Cells.html) to add formatted text) or in the format a report. 

You must also submit all the codes and Juypter notebooks you use in your analysis. They should be given to me in such a form that I can run through the analysis myself and reproduce the results. 

Each student has their own independent datasets that are sampled differently. The dataset you should use will be given via email. 

## Task 1 

Datasets: `Datasets-#/Task-1/`

In this task, you are given 20 datasets sampled independently from two distinct models (i.e., random processes) that we call models **A** and **B**. The two models differ in their mean/average value and their correlation. We do not know from which model each dataset has been sampled. 

Your overall task is to identify for each dataset which model it belongs to, **A** or **B**. 

Note that the dataset filenames are identified with a random five-digit integer that has no meaning other than giving each data file a unique name. 

To achieve your overall task of classifying the datasets, you can think about performing some of the tasks you perform in the practice dataset and compare the datasets, including:
- Visualize and plot the time series.
- Estimate the densities using discrete histograms and kernel density estimation.
- Calculate the average (i.e., mean) and standard deviation. 
- Calculate and plot the autocorrelation function.
- Use block averaging to estimate the mean (i.e., average) and the standard error of the mean.
- Estimate the autocorrelation times
For example, I would want to see a graph comparing the means for the different datasets, with the standard error of the mean shown as an error bar. You can also perform any other analysis you think is useful to help with the overall task.

## Task 2


