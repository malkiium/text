# Comparing Sets in Python

Sets are unordered collections of unique elements. Comparing sets ignores the order and considers only the elements.

## Basic Set Comparison

```python
print({2, 1} == {1, 2})  # True, because sets are unordered collections of unique elements
print({2, 1} == {1, 2, 2})  # True, because duplicates are removed in sets
```

## Set Operations

```python
set_a = {1, 2, 3}
set_b = {3, 4, 5}
```

### Union

Combines all unique elements from both sets.

```python
print(set_a | set_b)  # Output: {1, 2, 3, 4, 5}
```

### Intersection

Finds common elements in both sets.

```python
print(set_a & set_b)  # Output: {3}
```

### Difference

Finds elements that are in one set but not the other.

```python
print(set_a - set_b)  # Output: {1, 2}
print(set_b - set_a)  # Output: {4, 5}
```

### Symmetric Difference

Finds elements that are in either set, but not in both.

```python
print(set_a ^ set_b)  # Output: {1, 2, 4, 5}
```

Sets are useful for operations requiring uniqueness and fast membership testing.