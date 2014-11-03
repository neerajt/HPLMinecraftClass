# Talking to Minecraft

We need to open a connection between our Python console and the Minecraft game we just started. We'll do this by using an *API*.

```python
In [1]: import mcpi.minecraft as minecraft
In [2]: mc = minecraft.Minecraft.create()
```

*API* is short for application programming interface, but what you really need to know is that it lets us connect our Python code to another program, in this case Minecraft.

