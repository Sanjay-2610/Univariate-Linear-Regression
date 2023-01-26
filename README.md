# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
4.	Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```py
/*
Program to find the univariative linear regression
Developed by: Sanjay Ragavendar M K
RegisterNumber:22009286
/*
import numpy as np 
import matplotlib.pyplot as plt
x=np.array(eval(input()))
y=np.array(eval(input()))
x_mean=np.mean(x)
y_mean=np.mean(y)
num,den=0,0
for i in range(len(x)):
  num+= (x[i]-x_mean)*(y[i]-y_mean)
  den+= (x[i]-x_mean)**2
m=num/den
c=y_mean-m*x_mean
print(m,c)
y_pred=m*x+c
print(y_pred)
plt.scatter(x,y)
plt.plot(x,y_pred,color='orange')
plt.show
```
## Output
![image](https://user-images.githubusercontent.com/91368803/214787335-5f7912b4-4678-4090-b477-9fffb3303dce.png)
![image](https://user-images.githubusercontent.com/91368803/214787524-6e2d1ca3-e02f-41ed-8c26-75f80a17c6bc.png)



## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
