## ASSIGNMENT 2 A
Click here for [Jupyter Notebook Link](https://github.com/keepcalmncode/mlblr/blob/master/CS231n-python-numpy-tutorial.ipynb "github link")<br>

## ASSIGNMENT 2 B
Code to generate random numbers for preparing __backprop table__
```python
import random
import numpy as k

wh=k.random.rand(4,3)
wout=k.random.rand(3,1)
bh=k.random.rand(1,3)
bout=k.random.rand(1,1)

print(wh,wout,bh,bout)

```
#### Click here for [Jupyer Notebook Link](https://github.com/keepcalmncode/mlblr/blob/master/backpropagationtable.ipynb "github link") for backprop table calculations.
The section below represents all the values tabulated by calculating them using suitable formulae and the link to the notebook is given above.

| X ||||wh||| bh|||hidden_layer_input|||hidden_layer_activation|||wout|bout|output|Y|Error|
|-|-|-|-|--|--|--|--|-|-|-|-|-|-|---|-|-|-|-|-|-|-|-|-|
|1|0|1|0| 0.65|0.03|0.73| 0.28|0.65|0.84| 1.38|1.38|2.44|0.79|0.79|0.91|0.28|0.87|0.93|1|0.06|
|1|0|1|1| 0.97|0.84|0.77|    |||2.08|1.96|2.48|                 0.88|0.87|0.92|0.90|      |0.93|1|0.06|
|0|1|0|1| 0.43|0.69|0.86|        |||1.96|2.08|1.66|             0.87|0.88|0.84|0.88|      |0.93|0|-0.93|
|||| |0.70|0.58|0.48

<br>

| Slope hidden layer ||| slope  output | delta output |error at hidden layer||| delta hidden layer |||
|-|-|-|-|-|-|-|-|-|-|-|                                  
|0.21| 0.21| 0.20|0.20|0.00|0.001|0.001|0.001|0.00008|0.00002|0.00002|
|0.20|0.20|0.20|0.20|0.01|0.001|0.001|0.001|0.00007|0.00002|0.00002|
|0.20|0.20|0.21|0.20|-0.01|-0.001|-0.017|-0.014|-0.00003|-0.00001|-0.00001|

<br>

##### Updated weight and biases values

| X ||||wh||| bh|||hidden_layer_input|||hidden_layer_activation|||wout|bout|output|Y|Error|
|-|-|-|-|--|--|--|--|-|-|-|-|-|-|---|-|-|-|-|-|-|-|-|-|
|1|0|1|0| 0.65|0.03|0.73| 0.28|0.65|0.84| 1.38|1.38|2.44|0.79|0.79|0.91|0.28|0.87|0.93|1|0.06|
|1|0|1|1| 0.97|0.84|0.77|    |||2.08|1.96|2.48|                 0.88|0.87|0.92|0.89|      |0.93|1|0.06|
|0|1|0|1| 0.43|0.69|0.86|        |||1.96|2.08|1.66|             0.87|0.88|0.84|0.88|      |0.93|0|-0.93|
|||| |0.70|0.58|0.48
