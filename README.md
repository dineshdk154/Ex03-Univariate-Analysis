# Ex03-Univariate-Analysis
# DATE:
GITHUB LINK:https://github.com/dineshdk154/Ex03-Univariate-Analysis/edit/main/README.md

COLAB LINK:https://colab.research.google.com/drive/11-3DcuKsO4wZtvL7ByC6BIbb5uCDOpXZ#scrollTo=AhZOx3boyLQJ
# Aim
To read the given dataset and perform univariate analysis.
Explanation
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means
that the data has only one kind of variable. The major reason for univariate analysis is to use the
data to describe. The analysis will take data, summarise it, and then find some pattern in the data.
# Algorithm
Step1 Read the given data.

Step2 Get the information about the data.

Step3 Remove the null values from the data.

Step4 Mention the datatypes from the data.

Step5 Count the values from the data.

Step6 Do plots like boxplots,countplot,distribution plot,histogram plot.
# Program

Developed by :M DINESH KUMAR  

Register number:212221220011

import pandas as pd

import numpy as np

import seaborn as sns

df=pd.read_csv("SuperStore.csv")

print(df)

df.info()

df.describe()

df.isnull().sum()

df.dtypes

df['Row ID'].value_counts()

sns.boxplot(x="Row ID", data=df)

sns.countplot(x="Row ID", data=df)

sns.distplot(df["Row ID"])

sns.histplot(x="Row ID", data=df)
# output
Dataset

![image](https://user-images.githubusercontent.com/104413084/231061699-de53979e-4efc-4bea-98e7-d8a1e01c78f1.png)

Dataset info

![image](https://user-images.githubusercontent.com/104413084/231061915-54330ad7-88fa-48b4-a8d0-634a0dc797e7.png)

Dataset describe

![image](https://user-images.githubusercontent.com/104413084/231062074-6112f6a7-7e88-4d2b-b7ec-e611c0a7de51.png)

Null value

![image](https://user-images.githubusercontent.com/104413084/231062174-79aee600-8551-4256-89cb-221e236f5753.png)

Data types

![image](https://user-images.githubusercontent.com/104413084/231064739-ae77fafb-e550-41de-a4cb-276426c483d8.png)


Boxplot

![image](https://user-images.githubusercontent.com/104413084/231064964-d3df16d8-0ece-4996-9ade-613fbe1015a4.png)

count plot

![image](https://user-images.githubusercontent.com/104413084/231065077-58fe3715-13a4-4870-a0e4-ad42c5c07f62.png)

Distribution plot

![image](https://user-images.githubusercontent.com/104413084/231065275-86973cee-f94f-43ef-a67b-555d8869947f.png)

Histogram plot

![image](https://user-images.githubusercontent.com/104413084/231065430-37b8450e-8cd4-4f90-afc4-1aad155402b9.png)


# Result

Thus we have read the given data and performed the univariate analysis with different types of
plots.





