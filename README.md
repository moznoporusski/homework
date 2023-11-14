№1
```python
def process_number(N):
    oct_N = oct(N)[2:]
    if N % 7 == 0:
        oct_R = oct_N + oct_N[-2:]
    else:
        remainder = N % 7
        oct_remainder = oct(remainder * 7)[2:]
        oct_R = oct_N + oct_remainder

    R_decimal = int(oct_R, 8)

    return R_decimal

count = 0
for N in range(1, 3001):
    R = process_number(N)
    if R < 3000:
        count += 1

print(count)

```
93

№2
```python
def process_number(N):
    binary_N = bin(N)[2:]
    if N % 5 == 0:
        binary_R = binary_N + binary_N[-3:]
    else:
        remainder = N % 5
        binary_remainder = bin(remainder * 5)[2:]
        binary_R = binary_N + binary_remainder

    R_decimal = int(binary_R, 2)

    return R_decimal

N = 1
while True:
    R = process_number(N)
    if R > 256:
        break
    N += 1

print(N)

```
9

№3
```python
def process_number(N):
    binary_N = bin(N)[2:]
    if N % 3 == 0:
        binary_R = '10' + binary_N[2:] + '1'
    else:
        remainder = N % 3
        binary_remainder = bin(remainder * 2)[2:]
        binary_R = binary_remainder + binary_N

    R_decimal = int(binary_R, 2)

    return R_decimal

R_target = 8000
N = 1
while True:
    R = process_number(N)
    if R > R_target:
        break
    N += 1

print(R)

```
9217
