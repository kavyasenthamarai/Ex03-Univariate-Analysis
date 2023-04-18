# Ex03-Univariate-Analysis
Aim:
To read the given data and perform the univariate analysis with different types of plots.

# Theory:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

# Algorithm:
# Step 1:
Read the given data.

# Step 2:
Get the information about the data.

# Step 3:
Remove the null values from the data.

# Step 4:
Mention the datatypes from the data.

# Step 5:
Count the values from the data.

# Step 6:
Do plots like boxplots,countplot,distribution plot,histogram plot.

# Program:
Program developed by : k.kavya
Register number : 212222230065

import pandas as pd
import numpy as np
import seaborn as sns

data=pd.read_csv('SuperStore.csv')
data

data.head()

data.info()

data.describe()

data.isnull().sum()

data.dtypes

data['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=data)

sns.countplot(x='Postal Code',data=data)

sns.distplot(data["Postal Code"])

sns.histplot(x='Postal Code',data=data)

# Output:
# Dataset:
![image](https://user-images.githubusercontent.com/118668727/232675178-9ed626a5-ddf2-4bc3-84e0-c1544493e260.png)

# Head data:
![image](https://user-images.githubusercontent.com/118668727/231060264-af5b3293-9c12-4f26-be81-56e5c940ba46.png)
# Dataset Information:
![image](https://user-images.githubusercontent.com/118668727/231060368-1cd45a84-de06-42c6-bbba-6263c6c93cd5.png)
# Data Description:
![image](https://user-images.githubusercontent.com/118668727/231060405-210117a7-6a14-430f-95ef-5788ba8de54d.png)
# Null data:
![image](https://user-images.githubusercontent.com/118668727/231060451-59796828-a0d5-4d89-8a5f-154598a671a0.png)
# Datatype:
![image](https://user-images.githubusercontent.com/118668727/231060493-74141dba-3f91-4d6e-a4de-f741ee6dd98f.png)
# Value counts:
![image](https://user-images.githubusercontent.com/118668727/231060736-06d10315-9eef-4ea8-b67f-d0d537b833a4.png)
# Box plot:
![image](https://user-images.githubusercontent.com/118668727/231060782-c2729b82-1af0-40ef-99f8-4baf91f6c11a.png)
# Count plot:
![image](https://user-images.githubusercontent.com/118668727/231060820-dd524857-59f3-4548-84f6-28454121bee6.png)
# Distribution plot:
![image](https://user-images.githubusercontent.com/118668727/231060898-4f93772f-9187-47c9-bc95-b6ca82e2ee89.png)
# Histogram plot:
![image](https://user-images.githubusercontent.com/118668727/231060966-17375213-c9ad-49fc-831c-6004684819f7.png)
# Result:
Thus, we have read the given data and performed the univariate analysis with different types of plots.

