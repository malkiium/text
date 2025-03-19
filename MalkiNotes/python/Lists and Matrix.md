#PythonLists #ListOperations #PythonMatrices #PythonStrings #AppendingElements #CopyingLists #SortingLists #ReversingLists #UsingLoops #ListComparison #ApplyingFunctions #MatrixHandling #MatrixIteration #PythonFunctions #PythonBasics

## List Basics & Operations

### Creating a List

```python
ll = [x for x in range(0,7)]
print(ll)  # Output: [0, 1, 2, 3, 4, 5, 6]
```

### Appending Elements

- `.append(value)`: Adds a value to the end of the list.

```python
ll.append(45)
ll.append(23)
print(ll)  # Output: [0, 1, 2, 3, 4, 5, 6, 45, 23]
```

### Extending a List

- `.extend([list])`: Adds elements from another list.

```python
ll.extend([56,43])
print(ll)  # Output: [0, 1, 2, 3, 4, 5, 6, 45, 23, 56, 43]
```

### Inserting Elements

- `.insert(index, value)`: Inserts value at the given index.

```python
ll.insert(6, 5)
print(ll)  # Output: [0, 1, 2, 3, 4, 5, 5, 6, 45, 23, 56, 43]
```

### Copying Lists

- `.copy()`: Creates a duplicate list but maintains reference integrity.

```python
ll2 = ll.copy()
```

### Sorting a List

- `.sort()`: Sorts the list in-place.

```python
ll2.sort()
print(ll2)
print(ll)  # Original list remains unsorted
```

- `sorted(list)`: Returns a sorted list without modifying the original.

```python
lltri = list(sorted(ll))
print(lltri)
```

### Reversing a List

- `.reverse()`: Reverses the order of elements.

```python
ll2.reverse()
ll2 = ll2[::-1]
print(ll2)
```

the [::-1] means [start end step]. ":" means "default". the default for start is 0, and end is the whole length.
### Clearing a List

- `.clear()`: Removes all elements.

```python
ll2.clear()
print(ll2)  # Output: []
```

### Using Loops with Lists

```python
li2 = [a for a in range(0,5)]
for i in range(len(li2)):
    li2[i] = 2**i
print(li2)  # Output: [1, 2, 4, 8, 16]
```

### Applying Functions to Lists with `map()`

- `map(function, list)`: Applies a function to each element.

```python
def anyfunction(x: float):
    return 2*x

E = list(map(anyfunction, li2))
print(E)  # Output: [2, 4, 8, 16, 32]
```

## List Comparison

```python
list1 = []
list2 = []
list3 = list1

print(list1 == list2)  # True: Same content
print(list1 is list2)  # False: Different memory locations
print(list1 == list3)  # True: Same content
print(list1 is list3)  # True: Same memory reference
```

## Matrices in Python

A matrix is a list of lists.

```python
matrix = [['G', 'G', 'G', '', ''],
          ['F', 'F', '', '', ''],
          ['F', 'F', '', 'G', 'G'],
          ['', '', '', '', ''],
          ['G', 'G', 'G', 'G', 'G']]
```

### Counting Elements in a Matrix

```python
for i in range(len(matrix)):
    pers = {"garcons": 0, "filles": 0, "vide": 0}
    for j in range(len(matrix[i])):
        if matrix[i][j] == 'G':
            pers["garcons"] += 1
        elif matrix[i][j] == 'F':
            pers["filles"] += 1
        else:
            pers["vide"] += 1
    print(pers)
```

### Printing the Matrix

```python
for i in range(len(matrix)):
    for j in range(len(matrix[i])):
        if matrix[i][j] == 'G':
            print("G", end=" ")
        elif matrix[i][j] == 'F':
            print("F", end=" ")
        else:
            print("-", end=" ")
    print()
```

## String Operations

```python
ch1 = "helllllo"
print(ch1.index("l"))  # Finds first 'l'
print(ch1.count("l"))  # Counts occurrences of 'l'
print(ch1.find("l"))   # Same as index()
```