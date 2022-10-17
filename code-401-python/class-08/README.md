# Pandas

### Pandas is a game-changer for data science and analytics, particularly if you came to Python because you were searching for something more powerful than Excel and VBA. Pandas uses fast, flexible, and expressive data structures designed to make working with relational or labeled data both easy and intuitive.

### Pandas is an open source Python package that is most widely used for data science/data analysis and machine learning tasks. It is built on top of another package named Numpy, which provides support for multi-dimensional arrays.

## Object creation in pandas:
### Creating a Series by passing a list of values, letting pandas create a default integer index.

## Viewing data:
### DataFrame.to_numpy() gives a NumPy representation of the underlying data. Note that this can be an expensive operation when your DataFrame has columns with different data types, which comes down to a fundamental difference between pandas and NumPy: NumPy arrays have one dtype for the entire array, while pandas DataFrames have one dtype per column. When you call DataFrame.to_numpy(), pandas will find the NumPy dtype that can hold all of the dtypes in the DataFrame.

## Missing data
### pandas primarily uses the value np.nan to represent missing data.

## Merge
### Concat
## pandas provides various facilities for easily combining together Series and DataFrame objects with various kinds of set logic for the indexes and relational algebra functionality in the case of join / merge-type operations.


## Getting started with pandas :

### What kind of data does pandas handle?
## Pandas is best for handling or manipulating tabular data because it has a DataFrame object which has more functions. DataFrame is a 2-dimensional data structure that stores tabular data that can be in any form (integer values, characters, floating values, categorical, and more).

### How do I read and write tabular data?
## Pandas provides the read_csv() function to read data stored as a csv file into a pandas DataFrame.

### How do I select a subset of a DataFrame?
## To select a single column, use square brackets [] with the column name of the column of interest. Each column in a DataFrame is a Series.

### How do I create plots in pandas?
## To plot a specific column, use the selection method of the subset data tutorial in combination with the plot() method.

### How to create new columns derived from existing columns?
## Create a new column by assigning the output to the DataFrame with a new column name in between the [] . Operations are element-wise, no need to loop over rows. Use rename with a dictionary or function to rename row labels or column names.

### How to calculate summary statistics?
## The describe() function computes a summary of statistics pertaining to the DataFrame columns. This function gives the mean, std and IQR values.

### How to reshape the layout of tables?
## The numpy. reshape() function shapes an array without changing the data of the array.

### How to combine data from multiple tables?
## Pandas merge() function is used to merge multiple Dataframes. We can use either pandas.merge() or DataFrame.merge() to merge multiple.

### pandas is one of the reason why Python is such a great language
## pandas is

- simple to use, hiding all the complex and abstract computations behind
- (generally) intuitive
- fast, if not the fastest data analysis package (it highly optimized in C)
- It is THE tool that helps a data scientist to quickly read and understand data and be more efficient at his role.

