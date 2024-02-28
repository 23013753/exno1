## Exno:1
Data Cleaning Process

## AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

## Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

## Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

## Coding and 
# 1) Read and display DataFrame
import pandas as pd
df=pd.read_csv('/content/SAMPLEDS.csv')            
df

# 2) Display head
df.head()
   

# 3) Display tail
df.tail()


# 4) Info of datafram
df.info()


# 5) Describe about the dataframe
df.describe()
   



# 6) Describe about the dataframe
df.describe()
   

# 7) Shape of the datafram
df.shape
   

# 8) Checking tha NUll values
df.isnull().sum()


# 9) Drop the Null values
x=df.dropna(how='any')
x


# 10) Drop the Null values in Total
tot=df.dropna(subset=['TOTAL'],how='any')
tot
    

# 11) FIll the Null values
df.fillna(0)


# 12) Finding the mean value
mn=df.TOTAL.mean()
mn
    

# 13) Fill Null value with Mean value
df.head()


# 14) Final output
for x in df.index:
  if df.loc[x,"AVG"]>100:
    df.drop(x,inplace=True)
df
    

# 15)Cut and paste portion of image:
 import cv2
image=cv2.imread('Deepika.jpg',1)
image=cv2.resize(image,(400,400))
tag =image[150:200,110:160]
image[110:160,150:200] = tag
cv2.imshow('partimage1',image)
cv2.waitKey(0)
cv2.destroyAllWindows()
# OUTPUT:


1)![image](https://github.com/23013753/exno1/assets/145634121/2d04d117-d93b-4332-a4dd-bf9fc7228979)


2)![image](https://github.com/23013753/exno1/assets/145634121/29a0ef9c-21e1-457b-b8f2-a46bcec93d20)



3)![image](https://github.com/23013753/exno1/assets/145634121/a424497f-9032-4410-9669-39e0992b5296)




4)![image](https://github.com/23013753/exno1/assets/145634121/4209a6f6-da6b-4033-8bad-ec75a51dcbc2)



5)![image](https://github.com/23013753/exno1/assets/145634121/162b0369-f2a8-4fcb-b640-2bfe8754e434)


6)![image](https://github.com/23013753/exno1/assets/145634121/d5ab3e0c-d4c9-48fa-a72f-3b98a173b65d)


7)![image](https://github.com/23013753/exno1/assets/145634121/5f976914-1a93-40a4-9d5e-04d31693bf66)



8)![image](https://github.com/23013753/exno1/assets/145634121/a27025f7-dfd2-409d-b11c-3b655a3f82a8)


9)   ![image](https://github.com/23013753/exno1/assets/145634121/d05ad3de-c209-4cc2-b6e9-a8c0e241fa83)

10)  ![image](https://github.com/23013753/exno1/assets/145634121/11203dc0-fa96-46f6-b43b-251ccf995d0a)

11)  ![image](https://github.com/23013753/exno1/assets/145634121/cffdcac1-7f87-4d11-93b6-0b8a1ba90af0)

12)   ![image](https://github.com/23013753/exno1/assets/145634121/9fe4251c-1124-405a-9f75-3343f319f1a8)

13)  ![image](https://github.com/23013753/exno1/assets/145634121/62d98f42-b735-46d4-96a6-22c5fad67159)
 
14)  ![image](https://github.com/23013753/exno1/assets/145634121/ca229f12-551a-4a08-ad20-563e5a060b14)

15)  ![image](https://github.com/23013753/exno1/assets/145634121/a12e4e2b-a758-43e7-be5c-a69aaab9202b)

## Result:
The data clearning has beeen done successfully.
