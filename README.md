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

![](https://github.com/rohitkumar20700000/Ex03-Univariate-Analysis/blob/main/01.jpg)

Dataset info

![](https://github.com/rohitkumar20700000/Ex03-Univariate-Analysis/blob/main/02.jpg)

Dataset describe

![](https://github.com/rohitkumar20700000/Ex03-Univariate-Analysis/blob/main/03.jpg)

Null value

![](https://github.com/rohitkumar20700000/Ex03-Univariate-Analysis/blob/main/04.jpg)

Data types

![](https://github.com/rohitkumar20700000/Ex03-Univariate-Analysis/blob/main/05.jpg)

Value count

![](https://github.com/rohitkumar20700000/Ex03-Univariate-Analysis/blob/main/06.jpg)

Boxplot

![](https://github.com/rohitkumar20700000/Ex03-Univariate-Analysis/blob/main/07.jpg)

Count plot

![](https://github.com/rohitkumar20700000/Ex03-Univariate-Analysis/blob/main/08.jpg)

Distribution plot

![](https://github.com/rohitkumar20700000/Ex03-Univariate-Analysis/blob/main/09.jpg)

Histogram plot

![](https://github.com/rohitkumar20700000/Ex03-Univariate-Analysis/blob/main/10.jpg)

#Result:
Thus we have read the given data and performed the univariate analysis with different types of plots.

