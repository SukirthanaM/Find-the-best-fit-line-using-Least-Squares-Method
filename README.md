# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import 'numpy' for numerical operations.
2. Import matplotlib.pyplot for plotting graphs.
3. 'x': independent variable values.
4. 'y': dependent variable values.
5. Convert the input lists into NumPy arrays for easier calculations.
6. For each index i in the range of the length of x:
       Compute the numerator: (x[i] - x_mean) * (y[i] - y_mean)
       Compute the denominator: (x[i] - x_mean) ** 2
       Accumulate both into num and denom
7. Print the values of 'm' and 'b'.
8. Plot the original data points using a scatter plot.
9. Plot the regression line in red.
10. Show the graph.
## Program:
```
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: Sukirthana.M
RegisterNumber:212224220112

import numpy as np
import matplotlib.pyplot as plt
 x=np.array(eval(input()))
y=np.array(eval(input()))
x_mean=np.mean(x)
y_mean=np.mean(y)
num=0
denom=0
for i in range(len(x)):
    num+=(x[i]-x_mean)*(y[i]-y_mean)
    denom+=(x[i]-x_mean)**2

m=num/denom

b=y_mean-m*x_mean

print("Slope{}\nY.intercept{}:".format(m,b))

y_predicted=m*x+b
print(y_predicted)
      
plt.scatter(x,y)
plt.plot(x,y_predicted, color='red')
plt.show()
*/
```

## Output:
![image](https://github.com/user-attachments/assets/74d0905e-7f59-4c36-b257-8b80c95ad63a)

![image](https://github.com/user-attachments/assets/77a16291-af1c-4af8-a7b0-3571d112baaf)


## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
