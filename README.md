# Ex03-Univariate-Analysis

#AIM
To read the given dataset and perform univariate analysis.

#Explanation
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

#Algorithm
Step1 Read the given data.

Step2 Get the information about the data.

Step3 Remove the null values from the data.

Step4 Mention the datatypes from the data.

Step5 Count the values from the data.

Step6 Do plots like boxplots,countplot,distribution plot,histogram plot.

#PROGRAM
```
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
```

#OUTPUT
Dataset
Dataset info
Null value
Data types
Value count
Boxplot
Count plot
Distribution plot
Histogram plot
