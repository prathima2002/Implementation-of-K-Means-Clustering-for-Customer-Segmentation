# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: prathima
RegisterNumber:  212220040156
import pandas as pd
import matplotlib.pyplot as plt
data = pd.read_csv("/content/Mall_Customers (1).csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.cluster import KMeans
wcss = []
for i in range(1,11): 
  kmeans = KMeans(n_clusters = i,init = "k-means++")
  kmeans.fit(data.iloc[:,3:])
  wcss.append(kmeans.inertia_)
  plt.plot(range(1,11),wcss)
plt.xlabel("No. of Clusters")
plt.ylabel("wcss")
plt.title("Elbow Method")
km = KMeans(n_clusters = 5)
km.fit(data.iloc[:,3:])
y_pred = km.predict(data.iloc[:,3:])
y_pred
data["cluster"] = y_pred
df0 = data[data["cluster"]==0]
df1 = data[data["cluster"]==1]
df2 = data[data["cluster"]==2]
df3 = data[data["cluster"]==3]
df4 = data[data["cluster"]==4]
plt.scatter(df0["Annual Income (k$)"],df0["Spending Score (1-100)"],c="red",label="cluster0")
plt.scatter(df1["Annual Income (k$)"],df1["Spending Score (1-100)"],c="black",label="cluster1")
plt.scatter(df2["Annual Income (k$)"],df2["Spending Score (1-100)"],c="blue",label="cluster2")
plt.scatter(df3["Annual Income (k$)"],df3["Spending Score (1-100)"],c="green",label="cluster3")
plt.scatter(df4["Annual Income (k$)"],df4["Spending Score (1-100)"],c="magenta",label="cluster4")
plt.legend()
plt.title("Customer Segments")
*/
```
## Output:
![image](https://github.com/prathima2002/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/blob/bbf3f523bcc0ecbe8184eb57558eb1af87f7de99/WhatsApp%20Image%202022-11-10%20at%2008.55.34.jpeg)
![image](https://github.com/prathima2002/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/blob/558ed069e0f9e838954d8474c0a567bfdcbef3c7/WhatsApp%20Image%202022-11-10%20at%2008.55.43.jpeg)
![image](https://github.com/prathima2002/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/blob/aa4e3a2015f5b21df5944995e3acd4e342637e8b/WhatsApp%20Image%202022-11-10%20at%2008.56.06.jpeg)
![image](https://github.com/prathima2002/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/blob/ba15c342f1d58b730bb63a719bf97490948bae99/WhatsApp%20Image%202022-11-10%20at%2008.56.29.jpeg)
![image](https://github.com/prathima2002/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/blob/41cb883df6a8a5fc781dab8f8c7c0b714290efb3/WhatsApp%20Image%202022-11-10%20at%2008.56.39.jpeg)
![image](https://github.com/prathima2002/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/blob/5e001b9f266c9875b94bf2d61f6dee8548293d28/WhatsApp%20Image%202022-11-10%20at%2008.56.50.jpeg)
![image](https://github.com/prathima2002/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/blob/7d0b4c4696ee26eb6eb1df2e4081d4f8452e0837/WhatsApp%20Image%202022-11-10%20at%2008.57.07.jpeg)

## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
