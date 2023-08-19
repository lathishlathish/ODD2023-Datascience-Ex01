# Ex:01_DS_Data_Cleansing
## AIM
To read the given data and perform data cleaning and save the cleaned data to a file. 

# Explanation
Data cleaning is used for  process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. 
Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information. 

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Get the information about the data
### STEP 3
Remove the null values from the data
### STEP 4
Save the Clean data to the file

# CODE 

# For data_set:
```
import pandas as pd
df=pd.read_csv("/content/Data_set(1).csv")
print(df)

df.head(5)

df.info()

df.isnull()

df.isnull().sum()

df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0])
df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0])
df['original_network']=df['original_network'].fillna(df['aired_on'].mode()[0])
df.head()

df['rating']=df['rating'].fillna(df['rating'].mean())
df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean())
df.head()

df.head()

df['watchers']=df['watchers'].fillna(df['watchers'].median())
df.head()

df.info()

df.isnull().sum()
```
# For loan_data:
```
import pandas as pd
df=pd.read_csv("/content/Loan_Data(1).csv")
print(df)

df.head(5)

df.info()

df.isnull()

df.isnull().sum()

df['Loan_ID']=df['Loan_ID'].fillna(df['Education'].mode()[0])
df['Education']=df['Education'].fillna(df['Education'].mode()[0])
df['Married']=df['Married'].fillna(df['Education'].mode()[0])
df.head()

df['ApplicantIncome']=df['ApplicantIncome'].fillna(df['ApplicantIncome'].mean())
df['LoanAmount']=df['LoanAmount'].fillna(df['LoanAmount'].mean())
df.head()

df.head()

df['Loan_Amount_Term']=df['Loan_Amount_Term'].fillna(df['Loan_Amount_Term'].median())
df.head()

df.info()

df.isnull().sum()
```
# OUTPUT

# For data_set:

# DATA
![Screenshot 2023-08-18 191850](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/e4e81da7-4619-477e-b9b6-c73073b5385a)
![Screenshot 2023-08-18 193411](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/4cba6221-a830-4a20-a8cf-c8c77d6f8bb5)
# NON NULL BEFORE
![Screenshot 2023-08-18 193541](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/af9e492b-e015-47d7-b990-a1f6663a445a)
![Screenshot 2023-08-18 202420](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/2ea46ce2-f266-49b3-86da-2f5d2a1cd3a4)
![Screenshot 2023-08-18 202555](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/8f9995ce-937a-40bc-b486-d9362db0141d)
# MODE
![Screenshot 2023-08-18 202854](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/75c19325-41cb-4021-9dd7-32f7c248361e)
# MEAN
![Screenshot 2023-08-18 202943](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/ca651615-6ba5-473d-b324-dd0bc10a3980)
# MEDIAN
![Screenshot 2023-08-18 203120](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/fe92238f-e3e9-4cae-9c5f-fa3e70110d3e)

# NON NULL AFTER
![Screenshot 2023-08-18 203223](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/3356d321-5915-49e8-ae94-3455586d043f)

# For loan_data:

# DATA
![Screenshot 2023-08-18 191908](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/64758527-f9e4-4c26-a375-a32bc1590f1b)
![Screenshot 2023-08-18 203525](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/4a4c1d53-6df8-4774-b7de-c83986ee9fb1)
# NON NULL BEFORE
![Screenshot 2023-08-18 203645](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/4c591229-8ae2-4528-a27d-f0edef7a7689)
![Screenshot 2023-08-18 203722](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/2f9223ac-00ab-4e68-b61b-d90c6ef63a3f)
# MODE
![Screenshot 2023-08-18 203826](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/b7c1aa6c-2a61-4f8b-9935-d1ac84eec434)
# MEAN
![Screenshot 2023-08-18 203913](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/463f09f1-14a4-4ece-a5ff-9c793b5db7f2)
# MEDIAN
![Screenshot 2023-08-18 204003](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/75963217-7973-4703-86b3-b38b6b9f30eb)
# NON NULL AFTER
![Screenshot 2023-08-18 204233](https://github.com/Yogabharathi3/ODD2023-Datascience-Ex01/assets/118899387/86e8a726-68cc-477f-90d6-9934e7f82b3e)

# RESULT
Thus the given data is read,cleansed and the cleaned data is saved into the file.










