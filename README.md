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
