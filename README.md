# jupyterhack

A data browser which has a tree structure. This browser also controls matplotlib graphs embedded in PyQt5 windows. It can pickle all the data added to a file. So, data to be added to this browser have to be able to be pickeled.

## Installation

	conda install -c threemeninaboat3247 jupyterhack
	
## Usage

```python
%gui qt ### necessary when using in Jupyter
import jupyterhack as jh

r=jh.getRoot()

a='This is a string'
r.cur.add(a)

graph=MyGraphWindow()
graph.plot([1,2,3],[1,2,1])
r.cur.add(graph)

r.save()
```

![](https://github.com/threemeninaboat3247/jupyterhack/blob/master/jupyterhack.png)
