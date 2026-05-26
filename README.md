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
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.plot(x_values,y_values)
plt.show()
```
<img width="899" height="671" alt="image" src="https://github.com/user-attachments/assets/55e24e7c-2ebd-4867-a3f6-1c8cee6eb7e8" />

```
x=[1,2,3]
y=[2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My first graph')
plt.show()
```
<img width="1397" height="751" alt="Screenshot 2026-05-26 212910" src="https://github.com/user-attachments/assets/9027ba80-0e8f-47bb-97cc-e94a133ad34a" />

```
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label="line 1")
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line 2")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph')
plt.legend()
plt.show()
```
<img width="1262" height="760" alt="Screenshot 2026-05-26 212927" src="https://github.com/user-attachments/assets/72cb5919-5ddb-47e3-acb4-7c61b948c9bd" />

```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue') # Added closing quote and a color 'blue'
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations')
plt.show()
```
<img width="1259" height="748" alt="Screenshot 2026-05-26 212936" src="https://github.com/user-attachments/assets/240455bb-4b92-4423-9d26-db5bad8ffa81" />

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
<img width="1259" height="590" alt="Screenshot 2026-05-26 213744" src="https://github.com/user-attachments/assets/4e453337-6400-4008-a7f2-642233500cbb" />

```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```
<img width="1267" height="612" alt="Screenshot 2026-05-26 213749" src="https://github.com/user-attachments/assets/7dd28299-67ee-4f1c-aebe-47d65ce02bb7" />

```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9375,0.895] 
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.895] 
plt.plot(years , apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yield(tons per hectare)');
```
<img width="1265" height="668" alt="Screenshot 2026-05-26 213757" src="https://github.com/user-attachments/assets/f758e763-a457-4dff-95c0-de2997564751" />

```
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yield(tons per hectare)')
plt.title("Crop yield in Kanto")
plt.legend(['Apples','Oranges'])
```
<img width="1266" height="710" alt="Screenshot 2026-05-26 213804" src="https://github.com/user-attachments/assets/a3147162-550f-472b-88aa-24fa33f811bc" />

```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
plt.xlabel('Year')
plt.ylabel('Yield(tons per hectare)');
```
<img width="1259" height="629" alt="Screenshot 2026-05-26 213811" src="https://github.com/user-attachments/assets/b8a55791-5637-472c-9596-e5bd1aa7b529" />

```
plt.figure(figsize=(12,6))
years=range(2000,2012)
plt.plot(years,oranges,marker='o')
plt.title("Yield of oranges (tons per hectare)");
```
<img width="1279" height="725" alt="Screenshot 2026-05-26 213837" src="https://github.com/user-attachments/assets/51c71f39-d093-45d3-a101-0013c3c2e67b" />

```
plt.plot(years,apples,marker='o')
plt.plot(years,oranges,marker='x')
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yields in kanto")
plt.legend(['Apples','Oranges'])
```
<img width="1265" height="713" alt="Screenshot 2026-05-26 213843" src="https://github.com/user-attachments/assets/7b1dc908-601c-447c-bcbb-54533588ba70" />

```
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=30,color="blue")
plt.show()
```
<img width="1260" height="611" alt="Screenshot 2026-05-26 213849" src="https://github.com/user-attachments/assets/159e8c4d-7bb4-4fb6-84ff-74593e776a2e" />

```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6,7,8,9,10]
y=[2,4,5,7,6,8,9,11,12,12]
plt.scatter(x,y,label="stars",color="green",marker="*",s=30)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My scatter plot!')
plt.legend()
plt.show()
```
<img width="1267" height="732" alt="Screenshot 2026-05-26 213904" src="https://github.com/user-attachments/assets/bb396a3a-c8d2-49a6-8af6-cae43d419bca" />

```
import numpy as np
x=np.arange(0,10)
y=np.arange(11,21)
x
```
<img width="1264" height="150" alt="Screenshot 2026-05-26 213909" src="https://github.com/user-attachments/assets/3761338a-185b-4c67-8c6d-8017ea7acf35" />

```
y
```
<img width="1260" height="90" alt="Screenshot 2026-05-26 213915" src="https://github.com/user-attachments/assets/ae6af87f-30be-4435-a2d7-f40e8b2b129e" />

```
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
<img width="1262" height="655" alt="Screenshot 2026-05-26 213924" src="https://github.com/user-attachments/assets/6a6536fa-1397-45cf-98e8-7b9ccf0b66a6" />

```
y=x*x
y
```
<img width="1260" height="111" alt="Screenshot 2026-05-26 213930" src="https://github.com/user-attachments/assets/5b51eb13-3c6f-4f22-80d3-6aa559a643a1" />

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('x axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
```
<img width="1268" height="673" alt="Screenshot 2026-05-26 213941" src="https://github.com/user-attachments/assets/8a16b0f1-9fda-4e3e-a51a-ee64bea41af8" />

```
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```
<img width="1260" height="704" alt="Screenshot 2026-05-26 213946" src="https://github.com/user-attachments/assets/d18acfea-d357-4ddb-8129-836696451e1f" />

```
np.pi
```
<img width="1257" height="89" alt="Screenshot 2026-05-26 213953" src="https://github.com/user-attachments/assets/17f77044-d04b-498a-9870-5c3d81bd74ea" />

```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
<img width="1261" height="632" alt="Screenshot 2026-05-26 214002" src="https://github.com/user-attachments/assets/86f4a5b1-6698-44e9-9e2f-d96856df33f4" />

```
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
<img width="1256" height="705" alt="Screenshot 2026-05-26 214010" src="https://github.com/user-attachments/assets/124ecb5b-ee4d-47ee-a617-c4fd7949ce02" />

```
plt.stackplot(x,y1,y2,y3,labels=['Line 1','Line 2','Line 3'])
plt.legend(loc='upper left')
plt.title('Stacked Line Chart')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.show()
```
<img width="1264" height="676" alt="Screenshot 2026-05-26 214023" src="https://github.com/user-attachments/assets/3f59223b-be62-4d50-9619-4a5ebd0629aa" />

```
import numpy as np
import matplotlib.pyplot as plt
from scipy.interpolate import make_interp_spline
x=np.array([1,2,3,4,5,6,7,8,9,10])
y=np.array([2,4,5,7,8,8,9,10,11,12])
spl=make_interp_spline(x,y)
x_smooth=np.linspace(x.min(),x.max(),100)
y_smooth=spl(x_smooth)
plt.plot(x,y,'o',label='data')
plt.plot(x_smooth,y_smooth,'-',label='Spline')
plt.legend()
plt.show()
```
<img width="1253" height="741" alt="Screenshot 2026-05-26 214038" src="https://github.com/user-attachments/assets/eee0cf5c-2255-4428-a4e1-11aaf5e04499" />

```
import matplotlib.pyplot as plt
values=[5,6,3,7,2]
names=["A","B","C","D","E"]
plt.bar(names,values,color="green")
plt.show()
```
<img width="1260" height="607" alt="Screenshot 2026-05-26 214045" src="https://github.com/user-attachments/assets/52633f72-8a9b-4161-879f-53c99c62cd16" />

```
values=[5,6,3,7,2]
names=["A","B","C","D","E"]
plt.barh(names,values,color="yellowgreen")
plt.show()
```
<img width="1267" height="590" alt="Screenshot 2026-05-26 214049" src="https://github.com/user-attachments/assets/65184d98-0741-4c4d-b960-b75aa351f776" />

```
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My Bar Chart!')
plt.show()
```
<img width="1264" height="736" alt="Screenshot 2026-05-26 214056" src="https://github.com/user-attachments/assets/c3305810-4e57-4f22-838e-d6df09c6cf8e" />

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
<img width="1263" height="757" alt="Screenshot 2026-05-26 214103" src="https://github.com/user-attachments/assets/6dbcc45d-208e-49fe-9c70-e1723ff3d6a4" />

```
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
```
<img width="1266" height="717" alt="Screenshot 2026-05-26 214109" src="https://github.com/user-attachments/assets/d412183f-aade-4032-9445-6710c8540b20" />

```
x=[2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='blue',alpha=0.5)
plt.show()
```
<img width="1262" height="572" alt="Screenshot 2026-05-26 214117" src="https://github.com/user-attachments/assets/d0ce6c8f-06b1-441d-8eda-f79fa5572f5b" />

```
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
<img width="1270" height="509" alt="Screenshot 2026-05-26 214125" src="https://github.com/user-attachments/assets/c3f0bac0-16d5-487d-b87f-e0ca3eb3ad41" />

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Value')
ax.set_title('Box Plot')
```
<img width="1257" height="689" alt="Screenshot 2026-05-26 215212" src="https://github.com/user-attachments/assets/c88454e0-53eb-4e6b-84ac-7f62401cebbb" />

```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','g','b','y']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode = (0, 0.1, 0, 0))
plt.legend()
plt.show()
```
<img width="1261" height="601" alt="Screenshot 2026-05-26 215218" src="https://github.com/user-attachments/assets/da642a12-e201-44d4-acbd-1ea849509058" />

```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%') # Added closing parenthesis
plt.axis('equal')
plt.show()
```
<img width="1270" height="627" alt="Screenshot 2026-05-26 215229" src="https://github.com/user-attachments/assets/9bb822cc-6cac-4526-8a5d-8788c43be46f" />


# Result:
Thus, all the data visualization techniques of matplotlib has been implemented.

