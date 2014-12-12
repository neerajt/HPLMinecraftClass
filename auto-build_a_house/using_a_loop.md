# Using a "loop"

To make a big house of stone blocks, we will make a 6x6x4 block of stone blocks, then we want to 'delete' all the blocks inside. To do this we can fill air (**blockid: 0**) in between the 'outside wall' blocks. You'll notice we subtracted **two** from all the **xrange()** numbers:

Can you think about why this works?


```python
def buildhouse(x, y, z):
    for xi in xrange(6):
        for zi in xrange(4):
            for yi in xrange(6):
                mc.setBlock(x + xi, y + yi, z + zi, 1)
    for x in xrange(4):
        for z in xrange(2):
            for y in xrange(5):
                mc.setBlock(x + 1 + xi, y + yi, z + 1 + zi, 0)
```
