# Working with Dictionaries in Python

## Creating a Dictionary

A dictionary stores key-value pairs.

```python
my_dict = {
    "name": "Alice",
    "age": 25,
    "city": "New York"
}
```

## Accessing Values

```python
print("Name:", my_dict["name"])  # Output: Alice
print("Age:", my_dict["age"])    # Output: 25
```

## Adding a New Key-Value Pair

```python
my_dict["email"] = "alice@example.com"
print("Updated dictionary:", my_dict)
```

## Updating an Existing Value

```python
my_dict["age"] = 26
print("Updated age:", my_dict["age"])
```

## Removing a Key-Value Pair

```python
del my_dict["city"]
print("Dictionary after deletion:", my_dict)
```

## Using `.get()` to Access Values Safely

```python
print("Phone:", my_dict.get("phone", "Key not found"))
```

## Removing a Key-Value Pair Using `.pop()`

```python
removed_value = my_dict.pop("age", "Key not found")
print("Removed value:", removed_value)
print("Dictionary after pop:", my_dict)
```

## Iterating Through a Dictionary

- **Keys:**

```python
for key in my_dict:
    print("Key:", key)
```

- **Values:**

```python
for value in my_dict.values():
    print("Value:", value)
```

- **Key-Value Pairs:**

```python
for key, value in my_dict.items():
    print(f"Key: {key}, Value: {value}")
```

## Checking if a Key Exists

```python
if "name" in my_dict:
    print("Name is a key in the dictionary")
```

## Getting the Length of a Dictionary

```python
print("Length of dictionary:", len(my_dict))
```

## Using `.keys()` and `.values()`

```python
keys_list = list(my_dict.keys())
values_list = list(my_dict.values())
print("Keys:", keys_list)
print("Values:", values_list)
```

## Copying a Dictionary

```python
new_dict = my_dict.copy()
print("Copied dictionary:", new_dict)
```

## Merging Dictionaries

```python
another_dict = {"country": "USA", "age": 27}
my_dict.update(another_dict)
print("Updated dictionary after merging:", my_dict)
```

## Clearing a Dictionary

```python
my_dict.clear()
print("Cleared dictionary:", my_dict)
```

## Using `dict()` Constructor

```python
new_dict = dict(name="Bob", age=30, city="San Francisco")
print("New dictionary:", new_dict)
```

## Dictionary Comprehension

```python
squared_numbers = {x: x**2 for x in range(1, 6)}
print("Squared numbers dictionary:", squared_numbers)
```