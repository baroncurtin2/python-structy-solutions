# linked list cycle

## Description

Write a function, linked_list_cycle, that takes in the head of a linked list as an argument. The function should return a boolean indicating whether or not the linked list contains a cycle.

## Test Cases

test_00:

```text
a = Node('a')
b = Node('b')
c = Node('c')
d = Node('d')

a.next = b
b.next = c
c.next = d
d.next = b # cycle

#         _______
#       /        \
# a -> b -> c -> d

linked_list_cycle(a)  # True
```

test_01:

```text
q = Node('q')
r = Node('r')
s = Node('s')
t = Node('t')
u = Node('u')

q.next = r
r.next = s
s.next = t
t.next = u
u.next = q # cycle

#    ________________
#  /                 \
# q -> r -> s -> t -> u

linked_list_cycle(q)  # True
```

test_02

```text
a = Node('a')
b = Node('b')
c = Node('c')
d = Node('d')

a.next = b
b.next = c
c.next = d

# a -> b -> c -> d

linked_list_cycle(a)  # False
```

test_03:

```text
q = Node('q')
r = Node('r')
s = Node('s')
t = Node('t')
u = Node('u')

q.next = r
r.next = s
s.next = t
t.next = u
u.next = t # cycle

#                   __
#                 /   \
# q -> r -> s -> t -> u

linked_list_cycle(q)  # True
```

test_04:

```text
p = Node('p')

# p

linked_list_cycle(p) # False
```

test_05:

```text
linked_list_cycle(None) # False
```
