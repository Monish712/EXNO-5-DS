# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

## Aim:
  To Perform Data Visualization using matplot python library for the given datas.

## EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

## Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

## Coding and Output:
```

NAME: Pakanati Monish
REG NO: 212224240109

```
```py
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```

### Line Plot:

```py
marks=[13,45,63,78]
student=['ABC','QOR','EFB','TOB']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student name')
plt.show()

student=['A','B','C','D']
attendence=[90,85,73,88]
plt.plot(attendence,student)
plt.xlabel('Attendence')
plt.ylabel('Student name')
plt.show()
```

<img width="1374" height="635" alt="image" src="https://github.com/user-attachments/assets/50802b48-3f71-4477-b884-43654b68502e" />
<img width="1406" height="583" alt="image" src="https://github.com/user-attachments/assets/6a31bdd8-675a-4dd4-9bb8-9a442c76a1b2" />



### Scatter Plot:

```py
x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()

x=np.arange(0,15)
y=np.arange(0,15)
x
y
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('y axis')
plt.title('Scatter plot')
plt.show()
```

<img width="1412" height="658" alt="image" src="https://github.com/user-attachments/assets/4e8be771-41ca-49a4-a9f3-f33ed6e3125d" />
<img width="1431" height="569" alt="image" src="https://github.com/user-attachments/assets/a840ea81-e661-4690-97b4-ba2cec208682" />



### Pie Chart:

```py
act=['eat','sleep','work','play']
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()

feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```


<img width="1410" height="815" alt="image" src="https://github.com/user-attachments/assets/3879bdf7-f491-421d-bc60-a31673a6a28e" />
<img width="1433" height="521" alt="image" src="https://github.com/user-attachments/assets/aca855e2-450a-48e4-b12e-352096e48450" />


### Area Chart:

```py
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```

<img width="1416" height="793" alt="image" src="https://github.com/user-attachments/assets/3c20d75f-abf6-4f37-9534-a25793288ebc" />



### Bar Chart:

```py
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green'] 
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```

<img width="1393" height="819" alt="image" src="https://github.com/user-attachments/assets/d0182fb1-1f2c-4e49-920c-60e296e8595f" />



### Histogram:

```py
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```


<img width="1387" height="630" alt="image" src="https://github.com/user-attachments/assets/f0ed6c86-0610-4aaf-b87f-4e97f020579f" />




### Box Plot:

```py
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```


<img width="1371" height="556" alt="image" src="https://github.com/user-attachments/assets/8ac4410f-0b88-4877-85a5-fd356fd139a5" />



```py
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')

```

<img width="1399" height="750" alt="image" src="https://github.com/user-attachments/assets/d8d1085f-6224-4627-b947-242a47a66e42" />





## Result:

Thus, all the data visualization techniques of matplotlib has been implemented.
