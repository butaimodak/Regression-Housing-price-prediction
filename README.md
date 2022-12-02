# Regression-Housing-price-prediction
House prices can be an ever changing trend, but it does change based on certain parameters. Let's analyse individual parameters and do a price prediction of below 
dataset.<br>
[House Sales in King County, USA](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction)
<img src="https://i.imgur.com/kCNAFTN.jpg?1" title="source: imgur.com" />

## Process flowchart:
1. Reading the csv file using pandas library.
1. EDA and visual representation (Distribution of columns) using matplotlib and seaborn.
1. Making a model using statsmodels.api and get a summary.
>- Initially model result is very poor (Adjusted $R^2=0.08$). In this model **'date'** feature has highest t-stat.
>- After removing **'date'** column model get drastically improved (Adjusted $R^2=0.70$)
4. Feature selection: 
>-Based on **`VIF`** analysis (Multi-colinearity) and model summary I removed sum features to get optimum accuracy.
5. Feature extraction:
>-Based on high correlation value among features I did **`PCA`** and reduce the dimension from 6 features to 3 principal component.
6. Linear regression: This model gives 68% accuracy.
7. Random forest: This model gives 88% accuracy
