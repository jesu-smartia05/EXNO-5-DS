# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
 ```
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
x = [1, 2, 3, 4, 5]
y = [3, 6, 2, 7, 1]

plt.plot(x,y,label='line1')
```
![download](https://github.com/user-attachments/assets/6ced1689-d283-435f-a92d-ff7e5bc14449)
```
x1 = [1,2,3]
y1 = [2,4,1]
x2 = [1,2,3]
y2 = [4,1,3]

plt.plot(x1,y1,label='line1')
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```
![download](https://github.com/user-attachments/assets/bdf260da-944d-48dc-99b9-edbd4f39ee83)
```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()
```
![download](https://github.com/user-attachments/assets/f5b963bd-5c73-4ad7-b3a4-35c62d406249)
```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
![download](https://github.com/user-attachments/assets/cd7389da-e66c-4414-b762-1f10fd792f7b)
```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```
![download](https://github.com/user-attachments/assets/8f6a2203-ddcf-4888-bff3-fca0453fe73d)
```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges']);
```
![download](https://github.com/user-attachments/assets/94ad51f5-e6fd-49f2-91dc-66a9c3f11253)
```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```
![download](https://github.com/user-attachments/assets/0438915d-2a1d-4e58-b235-a16a703d0c91)
```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```
```
y
```
![Screenshot 2025-05-06 060045](https://github.com/user-attachments/assets/2e063e8a-5aa7-4d62-8fef-688ba9b0fc44)
```
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![download](https://github.com/user-attachments/assets/6ccd7692-9884-4fa5-a422-e2ab4b96f1f0)
```
y=x*x
y
```
![Screenshot 2025-05-06 060210](https://github.com/user-attachments/assets/cc99eb1f-d61f-4bcd-b52c-c749ce31afd9)
```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.legend(['y-values']);
```
![download](https://github.com/user-attachments/assets/ceb029d5-5ec2-499b-8c0b-4df764a137bc)
```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
![download](https://github.com/user-attachments/assets/e212f4e3-4ad2-4daa-b442-8f28bb92008e)
```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
```
![download](https://github.com/user-attachments/assets/9217dc46-c0f3-4f0f-99c0-c7f68eac93dc)
```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```
![download](https://github.com/user-attachments/assets/1f71c11b-d522-47b2-9894-85aa8fca3257)
```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
```
![download](https://github.com/user-attachments/assets/ab7e2d57-7a2c-4382-b41a-5f30aa657ee0)
```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
![download](https://github.com/user-attachments/assets/b6491ee4-95eb-4f44-a500-76be58d066c4)
```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
```
![download](https://github.com/user-attachments/assets/925fdf18-b913-4992-adcb-72b877143a8b)
```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![Screenshot 2025-05-06 060430](https://github.com/user-attachments/assets/b0ddfaa2-3c3e-4d5b-b033-f7c679a84fca)
```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![download](https://github.com/user-attachments/assets/60161281-33c7-4d26-b434-693e52e611a3)
```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```
![download](https://github.com/user-attachments/assets/90029346-3e72-4c1a-874b-697edc018477)

# Result:
 Thus the program executed successfully.
