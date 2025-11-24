# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
4. Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: Ramnithish.R
RegisterNumber:  212224230219

import numpy as np
import matplotlib.pyplot as plt
x=np.array(eval(input()))
y=np.array(eval(input()))
x_mean=np.mean(x)
y_mean=np.mean(y)
num=0
demo=0
for i in range(len(x)):
    num+=(x[i]-x_mean)*(y[i]-y_mean)
    demo+=(x[i]-x_mean)**2
m=num/demo
b=y_mean-m*x_mean
print('Register number:212224040280')
print('Name:Rogith J')
print('Slope:',m)
print('Y-intercept:',b)
y_predicted=m*x+b
print('Predicted value:',y_predicted)
plt.scatter(x,y)
plt.plot(x,y_predicted,color='red')
plt.show()

```

## Output:

8,2,11,6,5,4,12,9,6,1 3,10,3,6,8,12,1,4,9,14 Register number:212224040280 Name:Rogith J Slope: -1.1064189189189189 Y-intercept: 14.08108108108108 Predicted value: [ 5.22972973 11.86824324 1.91047297 7.44256757 8.54898649 9.65540541 0.80405405 4.12331081 7.44256757 12.97466216]

<img width="543" height="413" alt="475380368-b040fc15-d7de-40a3-bced-a37651ba04c2" src="https://github.com/user-attachments/assets/0e5b30f1-2563-49b8-9594-e48acb22dc41" />




## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
