# Ex03-Univariate-Analysis

### Aim

To read the given data and perform the univariate analysis with different types of plots.

### Explanation

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

### Algorithm

### Step1

Read the given data.

### Step2

Get the information about the data.

### Step3

Remove the null values from the data.

### Step4

Mention the datatypes from the data.

### Step5

Count the values from the data.

### Step6

Do plots like boxplots,countplot,distribution plot,histogram plot.

### PROGRAM
```
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv("SuperStore.csv")
df
df.head()
df.info()
df.describe()
df.isnull().sum()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x="Postal Code", data=df)
sns.countplot(x="Postal Code", data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x="Postal Code", data=df)
```
### OUTPUT

### DATA

![image](https://user-images.githubusercontent.com/120443233/228538901-c8e279f7-42bf-4b78-9506-e951bb69632a.png)

### DATA HEAD

![image](https://user-images.githubusercontent.com/120443233/228539094-b26d4eb3-83d6-4a8f-bdff-9166ad27ee07.png)

### DATA INFORMATION

![image](https://user-images.githubusercontent.com/120443233/228539357-e1ac025f-02c0-4687-aa7e-c7cbb6bd94ab.png)

### DATA DESCRIBE

![image](https://user-images.githubusercontent.com/120443233/228539564-5c9d0584-02af-4694-b5c2-28f59dcd032b.png)

### DATA NULL VALUES

![image](https://user-images.githubusercontent.com/120443233/228539859-19f9fca5-4a5b-4c2d-9dc2-e94f66ff77dd.png)

### DATA'S DATA TYPES

![image](https://user-images.githubusercontent.com/120443233/228540176-63d66f41-fea6-4d01-862d-7d4068fea1fc.png)

### DATA VALUE COUNT

![image](https://user-images.githubusercontent.com/120443233/228540384-7f838539-4ec1-481c-8bc2-d6b01ecef34d.png)

### BOXPLOT

![image](https://user-images.githubusercontent.com/120443233/228540576-d470c46b-dc25-4952-af7a-4a8f5ad7d550.png)

### COUNTPLOT

![image](https://user-images.githubusercontent.com/120443233/228540699-a9dd3f16-7866-46b8-b744-920c24c9b6d5.png)

### DISTRIBUTION PLOT

![image](https://user-images.githubusercontent.com/120443233/228540857-264bf4aa-2dcf-40e0-86de-043e4716323b.png)

### HISTOGRAM PLOT

![image](https://user-images.githubusercontent.com/120443233/228540994-64e9d3a7-752a-4591-a36c-dd8495bd3b03.png)

### RESULT

Thus we have read the given data and performed the univariate analysis with different types of plots.
