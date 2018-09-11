
# Numpy


```python
import numpy as np
```

## Python List to Numpy Arrays


```python
my_list = [1, 2, 3]
arr = np.array(my_list)
arr 
```




    array([1, 2, 3])




```python
my_mat = [[1,2,3],[4,5,6],[7,8,9]]
mat = np.array(my_mat)
mat
```




    array([[1, 2, 3],
           [4, 5, 6],
           [7, 8, 9]])



## Creating Arrays Programmatically

Simple Range


```python
np.arange(10)
```




    array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])




```python
np.arange(0,11,2)
# start, end, step size
```




    array([ 0,  2,  4,  6,  8, 10])



Ones and Zeroes


```python
np.zeros(10)
```




    array([0., 0., 0., 0., 0., 0., 0., 0., 0., 0.])




```python
np.ones(10)
```




    array([1., 1., 1., 1., 1., 1., 1., 1., 1., 1.])



Linear Space


```python
np.linspace(1,10,15)
# start, end, size
# 15 evenly-spaced numbers from 1 to 10
```




    array([ 1.        ,  1.64285714,  2.28571429,  2.92857143,  3.57142857,
            4.21428571,  4.85714286,  5.5       ,  6.14285714,  6.78571429,
            7.42857143,  8.07142857,  8.71428571,  9.35714286, 10.        ])



Identity Matrix


```python
np.eye(5)
```




    array([[1., 0., 0., 0., 0.],
           [0., 1., 0., 0., 0.],
           [0., 0., 1., 0., 0.],
           [0., 0., 0., 1., 0.],
           [0., 0., 0., 0., 1.]])

