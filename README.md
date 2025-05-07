![image](https://github.com/user-attachments/assets/3dc223c1-46de-4099-9c6d-213bbb90c2e4)# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:

Name: SUDHARSAN S
Reg.no: 212224040335
```
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
df=pd.read_csv("titanic_dataset.csv")
df.head()
```
![image](https://github.com/user-attachments/assets/50a1f35c-06e6-467e-b801-90f0ba43b273)

```
1.Line Plot
x=[1,2,3,4,5]
y=[3,6,2,7,1]
sns.lineplot(x=x,y=y)
plt.title('Line Plot')
```
![image](https://github.com/user-attachments/assets/b28a7d85-f070-4692-9d83-bcdb60c15ac0)

```
2.Multi Line Plot
x=[1,2,3,4,5]
y1=[3,5,2,6,1]
y2=[1,6,4,3,8]
y3=[5,2,7,1,4]
sns.lineplot(x=x,y=y1)
sns.lineplot(x=x,y=y2)
sns.lineplot(x=x,y=y3)
plt.title('Multi Line Plot')
```
![image](https://github.com/user-attachments/assets/e184cba9-1b31-4b01-a928-21c4386d1b8e)

```
TO VISUALIZE RELATIONSHIPS
1.Bar Chart
plt.figure(figsize=(8,5))
sns.barplot(x='Embarked',y='Fare',data=df,palette='rainbow')
plt.title("Fare Of Passenger By Embarked Town")
```
![image](https://github.com/user-attachments/assets/1115d7c0-b13e-4ecf-8f38-426bd2c930f9)

```
2.Scatter Plot
sns.scatterplot(x="Age", y="Fare", data=df)
plt.title('Scatterplot of Age vs Fare')
plt.show()
```
![image](https://github.com/user-attachments/assets/f6368e29-7ae3-4925-94dd-a860ff771978)
```
3.Bubble Chart
sns.scatterplot(x="Age", y="Fare", size="Pclass", data=df, sizes=(30, 200))
plt.title('Bubble Chart of Age vs Fare, Size by Passenger Class')
plt.show()
```
![image](https://github.com/user-attachments/assets/9ef3ca49-e63e-4a06-8045-59c505c444af)

```
TO CAPTURE DISTRIBUTIONS
1.Histogram
sns.histplot(data=df,x="Pclass",hue="Survived",kde=True)
```
![image](https://github.com/user-attachments/assets/e181b38b-6b77-4ee0-9b67-ee8054126407)
```
2.Box Plot
sns.boxplot(x='Pclass',y='Age',data=df,palette='rainbow')
plt.title("Age By Passenger Class")
```
![image](https://github.com/user-attachments/assets/bcc52302-7570-4b24-8a6e-67731dc3899f)

```
3.Violin Plot
sns.violinplot(x="Pclass", y="Fare", data=df)
plt.title('Violin Plot of Fare by Passenger Class')
plt.show()
```
![image](https://github.com/user-attachments/assets/adbc173d-1085-48c5-8087-c5a9b049be9c)

```
4.Density Plot
sns.kdeplot(data=df['Age'], shade=True)
plt.title('Density Plot of Passenger Ages')
plt.show()
```
![image](https://github.com/user-attachments/assets/a3854c01-3dd3-4180-8755-2bf13be44d45)

```
5.Heatmap
numeric_df = df.select_dtypes(include=['float64', 'int64'])
corr_matrix = numeric_df.corr()
sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
plt.title('Heatmap of Titanic Dataset')
plt.show()
```
![image](https://github.com/user-attachments/assets/e7633d5e-1693-4d22-9da7-90862185d050)



# Result:

Thus, the Data Visualization using seaborn python library for the given data is implemented successfully


