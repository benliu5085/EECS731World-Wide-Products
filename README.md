# EECS731World-Wide-Products

This is the project of EECS 731 Data science.

(1) Content

|-READ.ME 
|-forecast.ipynb 
|-data 
| |-Historical Product Demand.csv

NOTE: for transfering, I zipped Historical Product Demand.csv. Unzip it first before running the notebook!!!

(2) Ideas 
First, I plotted the trends of total demand orders with warehouse/product category, of the year 2012 and 2016, but no obvious trend can be identified, so I assume they are not core factor in forecast demand order of some product.

To forecast the orders of particular product, I construct the time series of total orders monthly. Then based on the assumption that current state is more likely influenced by close previous state, I will use the total orders of last 12 months to predict the order of next month, for each product.

To save time, I picked 3 products to showcase the performance of forecast model. I use linear regression, neural network and gradient boost regressor to perform the task. NN outperforms other methods, GBR overfited.
