
# Array Creation


```python
import numpy as np
```

#### Python List to Numpy Arrays


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



#### Creating Arrays Programmatically

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



#### Random Values


```python
np.random.seed(1234) 
# DO NOT DO THIS IN PROD
# I just need to have consistent values
# for this notebook
```


```python
np.random.rand(5)
# number of values
```




    array([0.19151945, 0.62210877, 0.43772774, 0.78535858, 0.77997581])




```python
np.random.randn(5)
# n random with normal distribution
```




    array([-0.94029827, -0.95658428, -0.33060682,  0.87412791,  2.00254961])




```python
np.random.rand(5,5)
# n x n random values
```




    array([[0.71270203, 0.37025075, 0.56119619, 0.50308317, 0.01376845],
           [0.77282662, 0.88264119, 0.36488598, 0.61539618, 0.07538124],
           [0.36882401, 0.9331401 , 0.65137814, 0.39720258, 0.78873014],
           [0.31683612, 0.56809865, 0.86912739, 0.43617342, 0.80214764],
           [0.14376682, 0.70426097, 0.70458131, 0.21879211, 0.92486763]])




```python
np.random.randint(5,100,2)
# start, end (excluded), number of values
```




    array([94, 89])



#### Reshaping Existing Arrays


```python
original_array = np.random.rand(25)
original_array
```




    array([0.05980922, 0.18428708, 0.04735528, 0.67488094, 0.59462478,
           0.53331016, 0.04332406, 0.56143308, 0.32966845, 0.50296683,
           0.11189432, 0.60719371, 0.56594464, 0.00676406, 0.61744171,
           0.91212289, 0.79052413, 0.99208147, 0.95880176, 0.79196414,
           0.28525096, 0.62491671, 0.4780938 , 0.19567518, 0.38231745])




```python
reshaped = original_array.reshape(5,5)
reshaped
```




    array([[0.05980922, 0.18428708, 0.04735528, 0.67488094, 0.59462478],
           [0.53331016, 0.04332406, 0.56143308, 0.32966845, 0.50296683],
           [0.11189432, 0.60719371, 0.56594464, 0.00676406, 0.61744171],
           [0.91212289, 0.79052413, 0.99208147, 0.95880176, 0.79196414],
           [0.28525096, 0.62491671, 0.4780938 , 0.19567518, 0.38231745]])




```python
reshaped.shape
```




    (5, 5)




```python
original_array.shape
```




    (25,)


