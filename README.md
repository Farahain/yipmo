# FFB-YiPMo: Fresh Fruit Bunch (FFB) Yield Prediction Model

These Jupyter notebooks are developed to predict FFB yield.
This project is part of Yield Prediction Challenge organized by Sime Darby Plantation.

## Viewing and running

Copies of the notebooks are hosted here on [Github](https://github.com/Farahain/yipmo).

To open these notebooks in an executable environment, please go to https://mybinder.org/v2/gh/Farahain/yipmo/master

## Data

We considered the data from May 2014 until December 2017. 
Location for the model considered based on Field 1 (F1) until Field 5 (F5).

## Variables

The dependent variable is yield.

The independent variables are rainfall, foliar, prunning time, prunning cost, manuring time, manuring cost, P&D time and P&D cost.

Definition:
- Yield = CPB tonnage.
- Rainfall = Rainfall in mm.
- Foliar = Number of month after foliar sampling month.
- Prunning time = Frequency of prunning per month.
- Prunning cost = Total of prunning cost per month.
- Manuring time = Frequency of manuring per month.
- Manuring cost = Total of manuring cost per month.
- P&D time = Frequency of P&D per month.
- P&D cost = Total of P&D cost per month.

## Assumption

1. In the case of no data, we substitute the data with 0.
2. In the case of no data, we perform the imputation method.

For prediction 2018, we resample the data for independent variables from the year 2014 until 2017. We assume the pattern of the data is similar with the past. 

## Workflow
1.	Declare the variables.
2.	Test correlation of the variables on the yield (CPB tonnage). 
3.	Variable selection.
4.	Modelling with the selected variables.
5.	Estimate the yield prediction.
6.	Evaluate the yield (CPB tonnage) in monthly, quarterly and half yearly.


## Outputs
1. Monthly yield = CPB tonnage per month.
2. Quarterly yield = Average of CPB tonnage for 3 months.
3. Half yearly yield = Average of CPB tonnage for 6 months.

## Notebooks
### Regression model A: Based on Assumption 1
- [Field 1 (F1)](https://github.com/Farahain/yipmo/blob/master/model-a-f1.ipynb)
- [Field 2 (F2)](https://github.com/Farahain/yipmo/blob/master/model-a-f2.ipynb)
- [Field 3 (F3)](https://github.com/Farahain/yipmo/blob/master/model-a-f3.ipynb)
- [Field 4 (F4)](https://github.com/Farahain/yipmo/blob/master/model-a-f4.ipynb)
- [Field 5 (F5)](https://github.com/Farahain/yipmo/blob/master/model-a-f5.ipynb)

### Regression model B: Based on Assumption 2
- [Field 1 (F1)](https://github.com/Farahain/yipmo/blob/master/model-b-f1.ipynb)
- [Field 2 (F2)](https://github.com/Farahain/yipmo/blob/master/model-b-f2.ipynb)
- [Field 3 (F3)](https://github.com/Farahain/yipmo/blob/master/model-b-f3.ipynb)
- [Field 4 (F4)](https://github.com/Farahain/yipmo/blob/master/model-b-f4.ipynb)
- [Field 5 (F5)](https://github.com/Farahain/yipmo/blob/master/model-b-f5.ipynb)

### Time series model C with seasonal factors. For this model, the independent variable is time.
- [Field 1 (F1)](https://github.com/Farahain/yipmo/blob/master/model-c-f1.ipynb)
- [Field 2 (F2)](https://github.com/Farahain/yipmo/blob/master/model-c-f2.ipynb)
- [Field 3 (F3)](https://github.com/Farahain/yipmo/blob/master/model-c-f3.ipynb)
- [Field 4 (F4)](https://github.com/Farahain/yipmo/blob/master/model-c-f4.ipynb)
- [Field 5 (F5)](https://github.com/Farahain/yipmo/blob/master/model-c-f5.ipynb)

## Authors

These notebooks are developed by Nurul Farahain Mohammad and Hafizah Bahaludin.

## Acknowledgements

Thank you to Sime Darby Plantation for giving us the opportunity to join this Yield Prediction Challenge.

