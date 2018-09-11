
# Operations


```python
import numpy as np
np.random.seed(100)
```


```python
my_array = np.random.randint(10,20,5)
my_array
```




    array([18, 18, 13, 17, 17])



#### Min/Max


```python
my_array.min()
# min value
```




    13




```python
my_array.argmax()
# max value index
```




    0




```python
my_array.argmin()
```




    2


