# Pet

Let's take that same *Trails* code and make some changes to make a gold-block pet. We want the pet to follow us around the map.

```Python
In [1]: import time
In [2]: while True:
...         blockid = 41
...         x, y, z = mc.player.getPos()
...         x = x + 3
...         mc.setBlock(x, y, z, blockid)
...         time.sleep(0.01)
...         mc.setBlock(x, y, z, 0)
```

Press enter *two* times to run the code. Go back in the game and look around for your pet! He/she should be following you around everywhere you go.
