---
ns: ENTITY
---
## GET_ENTITY_SPEED_VECTOR

```c
// 0x9A8D700A51CB7B0D 0x3ED2B997
Vector3 GET_ENTITY_SPEED_VECTOR(Entity entity, BOOL relative);
```

```
Relative can be used for getting speed relative to the frame of the vehicle, to determine for example, if you are going in reverse (-y speed) or not (+y speed).  
```

Here are the values for each vector in the output:
[When relativity is set to 'true' (body oriented)]:
X: Speed turning left / right (turning left == positve / turning right == negative)
Y: Speed moving forward / back (forward == positve / backwards == negative)
Z: Speed moving up / down (moving upwards (relative to your body) == positive / moving down (relative to your body) == negative)

[When relativity is set to 'false' (world oriented)]:
X: Speed moving East / West (East == Positive / West == Negative)
Y: Speed moving North / South (North == Positive / South == Negative)
Z: Speed moving Up / Down (Up == positive / Down == negative)


## Parameters
* **entity**: 
* **relative**: 

## Return value
