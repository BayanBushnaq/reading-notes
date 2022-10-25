# Matplotlib tutorial

![matplotlib](/code-401-python/class-11/matplotlib1.png)

## What is Matplot library and Whats used to ? 
### Matplotlib is a cross-platform, data visualization and graphical plotting library for Python and its numerical extension NumPy. As such, it offers a viable open source alternative to MATLAB. Developers can also use matplotlib's APIs (Application Programming Interfaces) to embed plots in GUI applications.

### Matplotlib comes with a set of default settings that allow customizing all kinds of properties. You can control the defaults of almost every property in matplotlib: figure size and dpi, line width, color and style, axes, axis and grid properties, text and font properties and so on. While matplotlib defaults are rather good in most cases, you may want to modify some properties for specific cases.

## Figures, Subplots, Axes and Ticks
### A figure in matplotlib means the whole window in the user interface. Within this figure there can be subplots. While subplot positions the plots in a regular grid, axes allows free placement within the figure. Both can be useful depending on your intention. 


## Figures
### A figure is the windows in the GUI that has "Figure #" as title. Figures are numbered starting from 1 as opposed to the normal Python way starting from 0. This is clearly MATLAB-style. 

## Subplots
### With subplot you can arrange plots in a regular grid. You need to specify the number of rows and columns and the number of the plot. Note that the gridspec command is a more powerful alternative.

## Axes
### Axes are very similar to subplots but allow placement of plots at any location in the figure. So if we want to put a smaller plot inside a bigger one we do so with axes.


## Ticks
## Well formatted ticks are an important part of publishing-ready figures. Matplotlib provides a totally configurable system for ticks. There are tick locators to specify where ticks should appear and tick formatters to give ticks the appearance you want. Major and minor ticks can be located and formatted independently from each other.

![matplotlib](/code-401-python/class-11/matplotlib2.png)

# Seaborn
## Seaborn is a library for making statistical graphics in Python. It builds on top of matplotlib and integrates closely with pandas data structures.

## Seaborn helps you explore and understand your data. Its plotting functions operate on dataframes and arrays containing whole datasets and internally perform the necessary semantic mapping and statistical aggregation to produce informative plots.

## A high-level API for statistical graphics
### There is no universally best way to visualize data. Different questions are best answered by different plots. Seaborn makes it easy to switch between different visual representations by using a consistent dataset-oriented API.

## How does Seaborn Works?
### Seaborn is the python library that is used to create the plot and graphical representation of the data, internally it maps our data and create an informative plot of the data, which is easy to understand the data.

![seaborn](/code-401-python/class-11/seaborn.png)
## Advantages
### We have some advantages of using seaborn in our application which is as follows;

- By using the seaborn library, we can easily represent our data on a plot.
- This library is used to visualize our data; we do not need to take care of the internal details; we just have to pass our data set or data inside the relplot() function, and it will calculate and place the value accordingly.
- Inside this, we can switch to any other representation of data using the ‘kind’ property inside it.
- It creates an interactive and informative plot to representation our data; also, this is easy for the user to understand and visualize the records on the application.
- It uses static aggregation for plot generation in python.
- As it is based on the matplotlib so while installing seaborn, we also have other libraries installed, out of which we have matplotlib, which also provides several features and functions to create more interactive plots in python.