#ListsVsTuples #NestedStructures #Mutability #TupleWithList #PythonTuples #PythonLists #TupleImmutability #ModifyingNestedLists #ListInsideTuple #PythonBasics #ReferenceVsCopy #PythonExamples

## Lists Inside Tuples and Mutability

```python
clientL = ["Jean", "Pierre", 19]
print("liste:")
print(f"nom : {clientL[0]}, prenom : {clientL[1]}, age : {clientL[2]}")
clientT = tuple(clientL)
print("tuple:")
print(f"nom : {clientT[0]}, prenom : {clientT[1]}, age : {clientT[2]}")
print()

print("pierre devient Ives")
print()

clientL[1] = "Ives"
print("liste:")
print(f"nom : {clientL[0]}, prenom : {clientL[1]}, age : {clientL[2]}")
print("tuple:")
print(f"nom : {clientT[0]}, prenom : {clientT[1]}, age : {clientT[2]}")
```

## Nested Lists Inside Tuples

```python
listedl = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
tupledl = tuple(listedl)
print("liste:")
print(listedl)
print("tuple:")
print(tupledl)

listedl[1][1] = 999
print("liste:")
print(listedl)
print("tuple:")
print(tupledl) 
 #output : [1, 2, 3, 4, 5, 6, 7, 8, 8]
```

## Explanation:

If a **list inside a tuple** is modified, the tuple remains unchanged, but the modifications inside the nested list are reflected. This happens because the tuple stores a reference to the list, not a copy.