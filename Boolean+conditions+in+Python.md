
# Here I am going to review the basics conditional statments in Python:



```python
import numpy as np
num = 35
if num > 100:
    print('greater than 100')
else: 
    print('not greater than 100')
print('done')
```

    not greater than 100
    done


We can also chain together several tests using the elif, short for else if.



```python
num = 3
if num > 0:
    print(num, 'is positive')
elif num == 0:
    print(num, 'is zero')
else:
    print(num, 'is negative')
```

    3 is positive



```python
if(1<0)|(1>=1): # here I can use 'or' or '|' to indicate the or operation.
    print('true')
```

    true


Let's now practice some operations on vectors.


```python
x = np.random.randn(4,4) # now we are creating a matrix 4x4 with random gaussian variables
x
```




    array([[ 1.38822345, -0.55196049,  0.05688873, -0.27571327],
           [-0.99855207,  1.66887432,  2.31332369,  0.26682269],
           [ 0.52679932, -2.1795156 , -0.6566527 ,  1.14838234],
           [-1.22679337, -2.50966217, -0.20882285, -1.6882439 ]])



# Here is an interesting use-case for conditional statements:
Say we want to condition our data so outliers are not used. 


```python
if (2.5 > np.max(x, axis = 0))[1] or np.max(x, axis = 0)[1]  > 1.5 :
    print('This is in the range of expected values')
```

    This is in the range of expected values



```python

```


```python

```
