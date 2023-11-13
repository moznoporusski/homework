№1
```python
 for i in range(100, 500):
    s = str(i)
    n1 = int(s[0]) + int(s[1])
    n2 = int(s[1]) + int(s[2])
    first = str(max(n1, n2))
    second = str((min(n1, n2)))
    s1 = first + second
    if s1 == '1412':
        print(i)
        break
```
395

№2
```python
 for i in range(10000, 1000, -1):
    s = str(i)
    n1 = int(s[0]) + int(s[1])
    n2 = int(s[2]) + int(s[3])
    first = str(min(n1, n2))
    second = str((max(n1, n2)))
    s1 = first + second
    if s1 == '117':
        print(i)
        break
```
9810

№3
```python
 for i in range(100, 1000):
    s = str(i)
    n1 = int(s[0]) + int(s[1])
    n2 = int(s[1]) + int(s[2])
    first = str(min(n1, n2))
    second = str((max(n1, n2)))
    s1 = first + second
    if s1 == '1115':
        print(i)
        break
```
296

№4
```python
 for i in range(100, 1000):
    s = str(i)
    n1 = int(s[0]) + int(s[1])
    n2 = int(s[1]) + int(s[2])
    first = str(max(n1, n2))
    second = str(min(n1, n2))
    s1 = first + second
    if s1 == '159':
        print(i)
        break
```
187

№5
```python
 for i in range(1000, 10000):
    s = str(i)
    n1 = int(s[0]) * int(s[1])
    n2 = int(s[2]) * int(s[3])
    first = str(max(n1, n2))
    second = str((min(n1, n2)))
    s1 = first + second
    if s1 == '124':
        print(i)
        break
```
1426
