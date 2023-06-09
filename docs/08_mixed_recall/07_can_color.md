# can color

## Description

Write a function, can_color, that takes in a dictionary representing the adjacency list of an undirected graph. The function should return a boolean indicating whether or not it is possible to color nodes of the graph using two colors in such a way that adjacent nodes are always different colors.

```text
For example, given this graph:

x-y-z

It is possible to color the nodes by using red for x and z,
then use blue for y. So the answer is True.

For example, given this graph:

    q
   / \
  s - r

It is not possible to color the nodes without making two
adjacent nodes the same color. So the answer is False.
```

## Test Cases

test_00:

```text
can_color({
  "x": ["y"],
  "y": ["x","z"],
  "z": ["y"]
}) # -> True
```

test_01:

```text
can_color({
  "q": ["r", "s"],
  "r": ["q", "s"],
  "s": ["r", "q"]
}) # -> False
```

test_02:

```text
can_color({
  "a": ["b", "c", "d"],
  "b": ["a"],
  "c": ["a"],
  "d": ["a"],
}) # -> True
```

test_03:

```text
can_color({
  "a": ["b", "c", "d"],
  "b": ["a"],
  "c": ["a", "d"],
  "d": ["a", "c"],
}) # -> False
```

test_04:

```text
can_color({
  "h": ["i", "k"],
  "i": ["h", "j"],
  "j": ["i", "k"],
  "k": ["h", "j"],
}) # -> True
```

test_05:

```text
can_color({
  "z": []
}) # -> True

```

test_06:

```text
can_color({
  "h": ["i", "k"],
  "i": ["h", "j"],
  "j": ["i", "k"],
  "k": ["h", "j"],
  "q": ["r", "s"],
  "r": ["q", "s"],
  "s": ["r", "q"]
}) # -> False
```
