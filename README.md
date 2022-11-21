# Ex03-Univariate-Analysis

# Aim
To read the given data and perform the univariate analysis with different types of plots.
 
# Explanation
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.
    
# Algorithm

## Step1
Read the given data.
    
## Step2
Get the information about the data.
    
## Step3
Remove the null values from the data.

## Step4
Mention the datatypes from the data.
    
## Step5
Count the values from the data.
    
## Step6
Do plots like boxplots,countplot,distribution plot,histogram plot.
    
# Program
```
Developed by : S Adithya Chowdary.
Registration Number : 212221230100.
```
```
import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv('superstore.csv')
df

df.head()
df.info()
df.describe()
df.isnull().sum()

df.dtypes

df['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x='Postal Code',data=df)
```

# Output:

# DATA

![image](https://user-images.githubusercontent.com/93427248/203040842-653b1f06-49ac-456f-bdb5-c5119cd60a11.png)
 
# DATA HEAD

![image](https://user-images.githubusercontent.com/93427248/203040882-54758445-8c9d-4776-807f-10512b5d974f.png)

# DATA INFORMATION

![image](https://user-images.githubusercontent.com/93427248/203040921-9dee42d6-fac5-44aa-b2de-6f25a6a4788c.png)

# DATA DESCRIBE

![image](https://user-images.githubusercontent.com/93427248/203040963-8baea588-5a6e-458a-9301-eed45a355492.png)

# DATA NULL VALUES

![image](https://user-images.githubusercontent.com/93427248/203041024-a167ffd2-cece-40d3-b50c-e5c1abbefb78.png)

# DATA'S DATATYPES

![image](https://user-images.githubusercontent.com/93427248/203041070-f963bb21-8768-4c1d-90da-fe0f5c6388ce.png)

# DATA'S VALUECOUNT
![image](https://user-images.githubusercontent.com/93427248/203041773-c8c71414-ba78-4b7f-87e8-3cc5229f248e.png)



# BOXPLOT
![image](https://user-images.githubusercontent.com/93427248/203041100-390742d8-5c0f-4740-80ab-f55d6f8927f4.png)



# COUNTPLOT
![image](https://user-images.githubusercontent.com/93427248/203041136-6ca60951-fd86-42d3-8c7f-19bb5018473a.png)


# DISTRIBUTION PLOT
![image](https://user-images.githubusercontent.com/93427248/203041162-19362d65-9774-46d5-aa78-a1c1a2b53df2.png)



# HISTOGRAM PLOT

![image](https://user-images.githubusercontent.com/93427248/203041205-4385c730-b18a-462c-9e50-fbba96f2ce2d.png)
# Result
Thus we have read the given data and performed the univariate analysis with different types of plots.
