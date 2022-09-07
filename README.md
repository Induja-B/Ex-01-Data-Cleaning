# Ex-01_DS_Data_Cleansing
# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# ALGORITHM
## STEP 1
Read the given Data

## STEP 2
Get the information about the data

## STEP 3
Remove the null values from the data

## STEP 4
Save the Clean data to the file

# CODE
import pandas as pd 

import numpy as np 

data=pd.read_csv("/content/Data_set (2).csv")

print(df)

df.head(10)

df.info()

df.isnull()

df.isnull().sum()

df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0])

df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0])

df['original_network']=df['original_network'].fillna(df['aired_on'].mode()[0])

df.head()

df['rating']=df['rating'].fillna(df['rating'].mode())

df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mode())

df.head()

df['watchers']=df['watchers'].fillna(df['watchers'].median())

df.head()

df.info()

df.isnull().sum()


# OUPUT
![image](https://user-images.githubusercontent.com/86044259/188831298-7f35a1d9-6e31-477b-8e91-a7ac39b29c6b.png)
![image](https://user-images.githubusercontent.com/86044259/188834194-c2f00397-6cc9-437f-8865-d9adf544ba81.png)
![image](https://user-images.githubusercontent.com/86044259/188834323-555be54f-47f8-43a0-b26a-95296879056e.png)
![image](https://user-images.githubusercontent.com/86044259/188834472-06a3f7e0-31fa-4a1d-bb09-dd65e61adf5d.png)
![image](https://user-images.githubusercontent.com/86044259/188834554-59e196c7-93bd-40f1-94e1-6c9641274a0f.png)





