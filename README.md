# Ex03-Univariate-Analysis
# Aim:
To read the given data and perform the univariate analysis with different types of plots.

# Explanation:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

# Algorithm:
# Step1:
Read the given data.

# Step2:
Get the information about the data.

# Step3:
Remove the null values from the data.

# Step4:
Mention the datatypes from the data.

# Step5:
Count the values from the data.

# Step6:
Do plots like boxplots,countplot,distribution plot,histogram plot.

# Program:
```
DEVELOPED BY : YUVABHARATHI.B

REG NO : 212222230181

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
# Dataset:
![image](https://user-images.githubusercontent.com/113497404/228884996-1c9269af-bd65-4589-bfeb-3e921027344d.png)

# Head:
![image](https://user-images.githubusercontent.com/113497404/228885586-458064b4-f1f6-409a-b4eb-1e5c6068d287.png)


# Info:
![image](https://user-images.githubusercontent.com/113497404/228885507-f31cf591-0cce-4a15-a29f-8f143f35b53e.png)\

# Describe:
![image](https://user-images.githubusercontent.com/113497404/228886273-09403205-65c2-4d32-beda-444fa330d73c.png)

# Isnull:
![image](https://user-images.githubusercontent.com/113497404/228886445-20d2bb66-5940-4dd0-bd85-f13b230b8da8.png)

# Dtypes:
![image](https://user-images.githubusercontent.com/113497404/228886896-22903122-c50f-4c69-9b08-adcc0c1c16e4.png)

# Valuecount:
![image](https://user-images.githubusercontent.com/113497404/228887187-5d19321b-ded2-4349-b8bc-7acf9cd9aa39.png)

# Boxplot:
![image](https://user-images.githubusercontent.com/113497404/228887527-1e14b827-04e5-4e05-93c0-eb9086345770.png)

# Countplot:
![image](https://user-images.githubusercontent.com/113497404/228887806-c58d03ca-a472-41a0-a51e-f352ae18357c.png)

# Distribution plot:
![image](https://user-images.githubusercontent.com/113497404/228887973-8fa50f79-6789-4872-9438-9aa1166bad26.png)

# Histogram plot:
![image](https://user-images.githubusercontent.com/113497404/228888187-65bc50e9-72f0-4776-8563-ebfc350aa2d3.png)

# Result:
Thus we have read the given data and performed the univariate analysis with different types of plots.

