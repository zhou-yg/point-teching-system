# overview

A animation renderer for demonstrate changes in data structutre. And it also supports custom plugin between changes.

# logical steps

example: 

> [1,2,3] -> [2,3,4,5,6]


1.find difference

```
removed = [1]
append = [4, 5, 6]
```

2.determine the changes order

collect effect and build list based on difference

```
[
 removed = [1],
 append = [4],
 append = [5],
 append = [6]
]
```

3.commit

traverse the effect list to perform rendering

x.extra

every step should support custom plugin

# supported data structure

## Array

example: 

> [1,2,3] -> [2,3,4,5,6]


