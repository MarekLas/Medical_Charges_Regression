<img align="center" width ="80%" src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/Doc-And-Pat.gif" />

<br />

# Medical Charges 

## Context
Machine Learning with R by Brett Lantz is a book that provides an introduction to machine learning using R. As far as I can tell, Packt Publishing does not make its datasets available online unless you buy the book and create a user account which can be a problem if you are checking the book out from the library or borrowing the book from a friend. All of these datasets are in the public domain but simply needed some cleaning up and recoding to match the format in the book.

### Content

Columns

* age: age of primary beneficiary

* sex: insurance contractor gender, female, male

* bmi: Body mass index, providing an understanding of body, weights that are relatively high or low relative to height,
  objective index of body weight (kg / m ^ 2) using the ratio of height to weight, ideally 18.5 to 24.9

* children: Number of children covered by health insurance / Number of dependents

* smoker: Smoking

* region: the beneficiary's residential area in the US, northeast, southeast, southwest, northwest.

* charges: Individual medical costs billed by health insurance

https://www.kaggle.com/datasets/mirichoi0218/insurance

## Link to the script

https://github.com/MarekLas/Medical_Charges_Regression/blob/main/med_cost_2023.ipynb

## Modules used (not all) in the script

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/01_mc_modules.png" align="center" width ="55%"/> 

## Data sample
Most of the data are categorical.

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/03_mc_rewiev_data.JPG" align="center" width ="40%"/> 

## Data information
There are no null values.

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/04_mc_data_info.JPG" width ="30%"/> 

## Data describe
At first sight everything looks ok.

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/06_mc_describe.JPG" width ="30%"/>

## Categorical data review

* sex  

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/07_mc_sex.JPG" width ="30%"/>

* smoker

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/08_mc_smoker.JPG" width ="30%"/>

* region

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/09_mc_region.JPG" width ="30%"/>

I decided to group the age data and the bmi data into the categories. I suspected that data distribution in this datas is different in each range.

* age

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/10_mc_age_category.png" width ="60%"/>

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/11_mc_age_category_chart.JPG" width ="30%"/>

* bmi

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/12_mc_weight_category.png" width ="60%"/>

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/13_mc_weight_category_chart.JPG" width ="30%"/>

## Let's see some pairplot charts

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/14_mc_paiplot_smoker.JPG" width ="60%"/>

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/15_mc_pairplot_sex.JPG" width ="60%"/>

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/16_mc_pairplot_region.JPG" width ="60%"/>

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/17_mc_pairplot_age_cat.JPG" width ="60%"/>

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/18_mc_pairplot_weight.JPG" width ="60%"/>

## Label data

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/19_mc_charges.JPG" width ="40%"/>

## Let's see some jointplot charts

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/20_mc_jointplot_age_bmi_cat.JPG" width ="30%"/>

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/21_mc_jointplot_age_charges_cat.JPG" width ="30%"/>

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/22_mc_jointplot_age_charges_weight.JPG" width ="30%"/>

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/23_mc_jointplot_age_charges_children.JPG" width ="30%"/>

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/23_mc_jointplot_bmi_charges_smoker.JPG" width ="30%"/>

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/24_mc_jointplot_age_bmi_smoker.JPG" width ="30%"/>

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/25_mc_jointplot_charges_bmi_region.JPG" width ="30%"/>

## It's time for the one hot encoding

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/26_mc_ohe.JPG" width ="140%"/>

## Correlation matrix

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/27_mc_heatmap.JPG" width ="100%"/>

## Spliting data

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/28_mc_splitting_and_scaling.png" width ="60%"/>

## Different regression models
I decided to check what will be the results using different regression algorithms.To pick optimal hiperparmeters I used the GridSearchCV() method from scikit-learn library.

https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/29_mc_models.png" width ="60%"/>

## Let's check which algorythm is the best for this dataset

* Linear Regression

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/30_mc_linear_regression.JPG" width ="30%"/>

* Lasso Regression

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/31_mc_lasso.JPG" width ="30%"/>

* AdaBoost Regression

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/32_mc_adaboost.JPG" width ="30%"/>

* Ridge Regression

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/33_mc_ridge.JPG" width ="30%"/>

* Random Forest Regression

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/34_mc_random_forest.JPG" width ="30%"/>

* KNeighbours Regression

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/35_mc_kneighbors.JPG" width ="30%"/>

* SVR

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/36_mc_svr.JPG" width ="30%"/>

### Ranking table

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/37_mc_ranking.JPG" width ="40%"/>

### Barplot charts

* Coefficient of determination - R2-score

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/37_mc_barplot_r2.JPG" width ="40%"/>

* Mean Absolute Error - MAE

<img src="https://github.com/MarekLas/Medical_Charges_Regression/blob/main/38_mc_barplot_mae.JPG" width ="40%"/>

## Summary
It looks like the AdaBoost Regression and Random Forest Regression are the best options for this dataset.





![GitHub last commit](https://img.shields.io/github/last-commit/MarekLas/Medical_Charges_Regression)
