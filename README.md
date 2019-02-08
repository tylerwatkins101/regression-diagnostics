# regression_diagnostics

# Summary of the Package

This package can be found at https://pypi.org/project/regression-diagnostics/.

This package is meant to be used for doing regression diagnostics on the output of your regression model.

It takes two lists or numpy arrays as input.

1. A  list of actual values (i.e. y-test)
2. A list of predicted values from your model (i.e. y-predicted)

# Motivation

In R, fast regression diagnostics are as easy as typing `plot(model)`.

In python, quickly analyzing your regression diagnostics takes way longer than it should. For that reason i decided to build this package. To get very fast diagnostics for my regression analysis.

# Files

This repository contains the file:

- regression_diagnostics.py

This file contains the code for using the RegressionDiagnostics class methods and retrieving the class attributes

# Installation

Packages that this package requires to be installed in your environment:

- numpy
- pandas
- matplotlib
- seaborn
- scipy
- statsmodels

After installing the above packages install regression_diagnostics with pip

`pip install regression-diagnostics`

# How to Use the Package

After importing the RegressionDiagnostics class to your working environment with:

`from regression_diagnostics import RegressionDiagnostics`

Instantiate an object as:

`rd = RegressionDiagnostics(actual_values, predicted_values)`

Use the functions:

- rd.shapiro()
- rd.fit_residplot()
- rd.pred_actualplot()
- rd.qqplot()

Get the attributes

- rd.residuals
- rd.standard_residuals
