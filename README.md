# Regression-Housing-price-prediction
House prices can be an ever changing trend, but it does change based on certain parameters. Let's analyse individual parameters and do a price prediction of below 
dataset.<br>
[House Sales in King County, USA](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction)
<img src="https://i.imgur.com/kCNAFTN.jpg?1" title="source: imgur.com" />

## Description:

Housing price prediction is the part of Supervised learning (regression). In this project Linear regression and Random forest are taken into consideration for model building.

Linear regresion model is based on following assumptions. Therefoe it is mandatory to check all those assumptions before building a model
1. Linear relationship
2. Homoscedasticity(Equal variance)
3. Normality (No outlier)
4. Independence (No auto correlation of Residual)
5. No relation between Residual and independet variable
6. No multi-colinearity

## Process flowchart:

<details>
    <summary>Imported libraries:</summary>
1.  numpy (for mathematical calculation)<br>
2.  pandas (for data importing and manipulation in the form of DataFrame)<br>
3.  matplotib.pyplot (for data visualization)<br>
4.  seaborn (for data visualization)<br>
5.  statsmodels.api (for model building)<br>
6.  sklearn.preprocessing.StandardScaler (for standardization)<br>
7.  sklearn.pipeline.make_pipeline (to pipeline the model building part in less time)<br>
8.  sklearn.decomposition.PCA (for dimensionlity reduction)<br>
9.  statsmodels.stats.outliers_influence.variance_inflation_factor (for multicolinearity analysis)<br>
10. sklearn.model_selection.train_test_split (for splitting dataset into training and testing)<br>
11. sklearn.linear_model.LinearRegression (for model building)<br>
12. sklearn.ensemble.RandomForestRegressor(for model building)<br>
13. sklearn.metrics.r2_score (for accuracy measurement)
</details>  
  
<details>
    <summary>EDA:</summary>
1. Null value Analysis<br>
2. Outlier Analysis
 </details> 
 
<details>
    <summary>Feature Engineering:</summary>
1. Feature Selection (correlation and VIF analysis)<br>
2. Feature Extraction (Principal Component Analysis)
 </details> 
 
<details>
    <summary>Statistical anlaysis:</summary>
  1. Testing all assumptions of linear regression.<br>
  2. Checking $t-stat$ and $p-value$ of individual features in linear model prediction<br>
  3. Checking $R^2$,  $adjusted~R^2$, $F-statistic$, $log~likelyhood$, $AIC$, $BIC$
 </details>
 
<details>
    <summary>Preprocessing:</summary>
  1. Transorming date column from object type to datetime.<br>
  2. Standardization of data before PCA<br>
 </details>
 
<details>
    <summary>Model Building:</summary>
  1. Linear regression (As such, after standardization of features, after normalization of features)<br>
  2. Random forest regression 
 </details>
 
 <details>
    <summary>Conclusion:</summary>
  1. $67\%$ of $R^2$ is explained by linear regression model and $33\%$ by residual <br>
  2. Random forest  gives 88% accuracy<br>
 </details>

