# Supermarket-Store-Branches-Analysis

![Supermarket](https://unsplash.com/s/photos/supermarket)

A supermarket is a self-service shop offering a wide variety of food, beverages and household products, organized into sections. This kind of store is larger and has a wider selection than earlier grocery stores, 
but is smaller and more limited in the range of merchandise than a hypermarket or big-box market. In everyday U.S. usage, however, "grocery store" is synonymous 
with supermarket, and is not used to refer to other types of stores that sell groceries.  

In the dataset, You'll get data of different stores of a supermarket company as per their store IDs which for ease has been converted to positive integers.  
Store_ID: (Index) ID of the particular store.  

Store_Area: Physical Area of the store in yard square.  
Items_Available: Number of different items available in the corresponding store.  
Daily_Customer_Count: Number of customers who visited to stores on an average over month.  
Store_Sales: Sales in (US $) that stores made.  

The data is obtained from the project from the University after seeking proper permission.

The analysis is done to investigate the most dominant factor, among Store_Area, Items_Available and Daily_Customer_Count that contributes to Store Sales (in US $).

The whole analysis was done by using Jupyter Notebook.

Reference Link: https://www.kaggle.com/datasets/surajjha101/stores-area-and-sales-data

Before analysis can be done, relevant libraries must be imported which are Pandas, Numpy, Matplotlib, seaborn, scikitlearn and os:

import pandas as pd

import numpy as np

import matplotlib.pyplot as plt

import seaborn as sns

import os

from sklearn.linear_model import LinearRegression


A dataframe named 'stores' was created to store data from the CSV file imported from the operating system (you may download it from this repository):

stores = pd.read_csv('C:/Users/user/Downloads/archive (1)/Stores.csv') 

The variables that describe each column in the dataset are:

x_area = np.array(stores['Store_Area'])

x_items = np.array(stores['Items_Available'])

x_cust = np.array(stores['Daily_Customer_Count'])

y_sales = np.array(stores['Store_Sales'])

y_sales is considered as the responding variable, whereas x_area, x_items, and x_cust are the independent variables.

Through linear regression, we visualize the relationship between y_sales against x_area, x_items and x_cust, including the lines of best fit, correlation matrices, and R2 values.

For more details on the process of analyzing this data as well as its results, you may click this link: https://github.com/shaheer26/Supermarket-Store-Branches-Analysis/blob/main/Supermarket%20Store%20Branches%20Portfolio.ipynb
