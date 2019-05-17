# FFB-YiPMo: Fresh Fruit Bunch (FFB) Yield Prediction Model

These Jupyter notebooks are developed to predict FFB yield.
This project is part of Yield Prediction Challenge organized by Sime Darby Plantation.

## Viewing and running

Copies of the notebooks are hosted here on [Github](https://github.com/Farahain/yipmo).

To open these notebooks in an executable environment, please go to https://mybinder.org/v2/gh/Farahain/yipmo/master

## Data

We considered the data from May 2015 until December 2017. The training data are from May 2015 to December 2016 whereas the test data are from January 2017 to December 2017.

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

## Workflow
1. Clean the data.
2. Declare the variables.
3. Check the correlation.
4. Variable selection.
5. Modelling with selected variables.
6. Estimate the yield prediction.
7. Calculate the root mean square error (RMSE).

## Outputs
1. Monthly yield = CPB tonnage per month.
2. Quarterly yield 1 = Total of CPB tonnage for 3 months.
3. Quarterly yield 2 = Average of CPB tonnage for 3 months.
4. Half yearly yield 1 = Total of CPB tonnage for 6 months.
5. Half yearly yield 2 = Average of CPB tonnage for 6 months.

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

## Authors

These notebooks are developed by Nurul Farahain Mohammad and Hafizah Bahaludin.

## Acknowledgements

Thank you to Sime Darby Plantation for giving us the opportunity to join this Yield Prediction Challenge.

