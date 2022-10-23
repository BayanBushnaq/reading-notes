# Linear Regressions

## What is linear regression?
### Linear regression establishes the linear relationship between two variables based on a line of best fit. Linear regression is thus graphically depicted using a straight line with the slope defining how the change in one variable impacts a change in the other.

## What is Scikit learn ?
### Scikit-learn is a free machine learning library for Python. It features various algorithms like support vector machine, random forests, and k-neighbours, and it also supports Python numerical and scientific libraries like NumPy and SciPy .

## Advantages of using Scikit learn :
- Simple and efficient tools for predictive data analysis.
- Accessible to everybody, and reusable in various contexts.
- Open source, commercially usable.
- Built on NumPy, SciPy, and matplotlib.

# What is the general equation of linear regression?
## Y = a + bX 
## A linear regression line has an equation of the form Y = a + bX, where X is the explanatory variable and Y is the dependent variable. The slope of the line is b, and a is the intercept (the value of y when x = 0)

- Y = “target” data in Python) [Response Vriable]
- X = all the other features (or independent variables / Explanatory Variable)

##  import linear regression from sci-kit learn module.
- from sklearn_liner_model import LinearRegression 

### If you want to look inside the linear regression object, you can do so by typing LinearRegression. and the press <tab> key. This will give a list of functions available inside linear regression object.

![Linear Regression](/code-401-python/class-10/linear-regression.png)

## When Do You Need Regression?
### Typically, you need regression to answer whether and how some phenomenon influences the other or how several variables are related. For example, you can use it to determine if and to what extent experience or gender impacts salaries.

### Regression is also useful when you want to forecast a response using a new set of predictors. For example, you could try to predict electricity consumption of a household for the next hour given the outdoor temperature, time of day, and number of residents in that household

## Linear Reagression Types:
- Simple Linear Regression.
- Multiple Linear Regression.
- Polynomial Regression.
- Logistic regression.
- Ordinal regression.
- Discriminant analysis.


## Polynomial Regression:
### Underfitting and Overfitting
## One very important question that might arise when you’re implementing polynomial regression is related to the choice of the optimal degree of the polynomial regression function.

## There’s no straightforward rule for doing this. It depends on the case. You should, however, be aware of two problems that might follow the choice of the degree: underfitting and overfitting.

## Underfitting occurs when a model can’t accurately capture the dependencies among data, usually as a consequence of its own simplicity. It often yields a low 𝑅² with known data and bad generalization capabilities when applied with new data.

## Overfitting happens when a model learns both data dependencies and random fluctuations. In other words, a model learns the existing data too well. Complex models, which have many features or terms, are often prone to overfitting. When applied to known data, such models usually yield high 𝑅². However, they often don’t generalize well and have significantly lower 𝑅² when used with new data.


### Simple Linear Regression With scikit-learn
## start with the simplest case, which is simple linear regression. There are five basic steps when you’re implementing linear regression:

- Import the packages and classes that you need.
- Provide data to work with, and eventually do appropriate transformations.
- Create a regression model and fit it with existing data.
- Check the results of model fitting to know whether the model is satisfactory.
- Apply the model for predictions.