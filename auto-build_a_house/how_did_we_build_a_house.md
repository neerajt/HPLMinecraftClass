# How did we build a house?

We can build a house by explicitly telling python where and how we want our blocks placed! Like this:


```python

houseslices = [
    [[1, 1, 1, 1],
     [1, 0, 0, 1],
     [1, 0, 0, 1],
     [1, 1, 1, 1]],
    [[1, 1, 1, 1],
     [1, 0, 0, 1],
     [1, 0, 0, 1],
     [1, 1, 1, 1]],
    [[1, 1, 1, 1],
     [1, 0, 0, 1],
     [1, 0, 0, 1],
     [1, 1, 1, 1]]]

def buildhouse(x, y, z):
    xi = 0
    for slice in houseslices:
        yi = 0
        for row in slice:
            zi = 0
            for blk in row:
                mc.setBlock(x + xi, y + yi, z + zi, blk)
                zi += 1
            yi += 1
        xi += 1
```
