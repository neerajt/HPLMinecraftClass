# How did we build a house?

To make a big house of stone blocks, we do:

```python
for x in xrange(6):
    for z in xrange(4):
        for y in xrange(6):
            mc.setBlock(50 + x, 0 + y, -38 + z, 1)
```

To 'delete' all the blocks besides the wall, we can fill air in after the wall block, and up to the next wall block, so you'll notice we subtracted **two** from all the **xrange()** numbers:

```python
for x in xrange(4):
    for z in xrange(2):
        for y in xrange(5):
            mc.setBlock(51 + x, 0 + y, -37 + z, 1)
```

Can you think about why this works?
