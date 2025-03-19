[[lists vs tuples]]

#TuplesVsLists #TuplesInPython #ListsInPython #ImmutableVsMutable #TupleProperties #PythonDataTypes #TupleConcatenation #PythonExamples #TupleAssignment #ModifyingTuples #TupleWorkaround #TupleModification #PythonCollections #TupleVsList

## Creating an Empty Tuple

```python
tuple1 = ()
```

## Properties of Tuples

Tuples are similar to lists but are **immutable**, meaning you cannot modify them after creation.

### Creating a Tuple with Elements

```python
tuple2 = (1, 2, 3, 4, 5)
```

### Accessing Elements

```python
print(tuple2[0])  # Output: 1
```

### Tuples with Different Data Types

```python
tuple3 = (1, "hello", 3.14)
```

### Concatenating Tuples

```python
tuple4 = tuple2 + tuple3
```

### Multiple Assignment with Tuples

```python
a, b, c = (1, 2, 3)
print(a, b, c)  # Output: 1 2 3
```

---

## Difference Between Lists and Tuples

### Lists Can Be Modified

```python
list1 = [1, 2, 3]
list1[0] = 10  # Allowed
print(list1)  # Output: [10, 2, 3]
```

### Tuples Cannot Be Modified

```python
try:
    tuple2[0] = 10  # This will raise an error
except TypeError as e:
    print(e)  # Output: 'tuple' object does not support item assignment
```

---

## Modifying a Tuple (Workaround)

Since tuples are immutable, to "modify" them, convert them to a list, change the list, and convert it back to a tuple.

### Appending to a Tuple

```python
list2 = list(tuple2)
list2.append(6)
tuple2 = tuple(list2)
print(tuple2)  # Output: (1, 2, 3, 4, 5, 6)
```

### Removing an Element from a Tuple

```python
list2.remove(3)
tuple2 = tuple(list2)
print(tuple2)  # Output: (1, 2, 4, 5, 6)
```

---

## Concatenating Tuples

```python
tupleConcat = tuple2 + tuple3
print(tupleConcat)
```



