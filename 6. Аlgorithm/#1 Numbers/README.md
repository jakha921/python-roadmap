# Algorithm

## Numbers

+ What is algorithm?
    + definite input & gite definite output
    + algorithm is need to break(stop)

- Number system
    - System, Base, Digits
        - Binary, 2, 0 1
        - Octal, 8, 0 1 2 3 4 5 6 7
        - Decimal, 10, 0 1 2 3 4 5 6 7 8 9
        - Hexadecimal, 16, 0 1 2 3 4 5 6 7 8 9 A B C D

> Find binary number
> ![alt text](https://i2.paste.pics/IQ19T.png "Title")
> ![alt text](https://i2.paste.pics/IQ1BJ.png "Title")

    165 = 128+32+4 = 2^7 + 2^5 + 2^2

    2^0 = 0             2^6 = 64
    2^1 = 2             2^7 = 128
    2^2 = 4             2^8 = 256
    2^3 = 8             2^9 = 512
    2^4 = 16            2^10 = 1024
    2^5 = 32

| 8 | 7 | 6 | 5 | 4 | 3 | 2 | 1 |
|---|---|---|---|---|---|---|---|
| 0 | 1 | 0 | 1 | 0 | 0 | 1 | 1 |

## Bitwise Operations

> & = AND <br />
> a&b returns True(1) or False(0)
>> ![alt text](https://i2.paste.pics/IQDSQ.png "Title")

> | = OR <br />
> a|b check one of given parameters is True
> > ![alt text](https://i2.paste.pics/IQE0U.png "Title")

> ^ = XOR <br />
> a^b check for different parameters
> > ![alt text](https://i2.paste.pics/IQE4K.png "Title")>

> << / >> = SHIFTING <br />
> 1024 >> 1 = 102 move to given position <br />
> 1024 >> 2 = 10 <br />
> 1024 >> 3 = 1 <br />
> 1024 >> 4 = 0 <br />
> 1024 << 1 = 10240 <br />
> 1024 << 2 = 102400 <br />
> 1024 << 2 = 1024000 <br />
> ![alt text](https://i2.paste.pics/IQEJ1.png "Title")

## Practice

### print_digits

> <img src="https://i2.paste.pics/IQFJX.png" width="566" height="90" alt="Screenshot">

 ```python
# Code
# We can also reverse the code turning to str

def print_digits(numb: int) -> None:
    """given numb is 154"""
    if numb == 0:
        print(0)
        return

    while numb != 0:
        digit = numb % 10  # 4 Возмет остаток ex: numb % 2 
        print(digit)
        numb //= 10  # Возвращает только целую часть 15 ex: numb >> 1 = 15
```

### reverse_digits

> <img src="https://i2.paste.pics/IQFN5.png" width="668" height="195" alt="Screenshot">

```python
def reverse_digits(num: int) -> int:
    """given numb is 154"""
    result = 0

    while num != 0:
        result *= 10  # result == 0 * 0
        digit = num % 10  # give 4
        result += digit  # result = 0 + 4
        num //= 10  # give 15

    return result  # 451

```

### convert_to_binary

<img src="https://i2.paste.pics/IQG0F.png" width="599" height="186" alt="Screenshot">

```python
def convert_to_binary(num: int) -> str:
    """given numb 154"""
    result = ""

    while num != 0:
        digit = num % 2  # give 0 % 2 because need to find binary
        result += str(digit)
        num //= 2
    return result
```

### is_power_of_two

<img src="https://i2.paste.pics/IQGOJ.png" width="750" height="162" alt="Screenshot">

```python
def is_power_of_two(num: int) -> bool:
    """given numb 15"""
    bit_count = 0  # 1, 2, 3, 4

    while num != 0:
        bit_count += num & 1  # ex: num % 2, ans: 1, 1, 1, 1
        num = num >> 1  # ex: num //= 2, ans: 7, 3, 1, 0

    return bit_count == 1  # ex: 4 == 1, ans: False 
```

### is_power_of_two

<img src="https://i2.paste.pics/IQGOJ.png" width="750" height="162" alt="Screenshot">

```python
def is_power_of_two(num: int) -> bool:
    """given numb 15"""
    bit_count = 0  # 1, 2, 3, 4

    while num != 0:
        bit_count += num & 1  # ex: num % 2, ans: 1, 1, 1, 1
        num = num >> 1  # ex: num //= 2, ans: 7, 3, 1, 0

    return bit_count == 1  # ex: 4 == 1, ans: False 
```

### factorial

<img src="https://i2.paste.pics/IQHC5.png" width="66" height="434" alt="Screenshot">
<img src="https://i2.paste.pics/IQHB8.png" width="655" height="496" alt="Screenshot">

```python
import math


def count_factorial(n):
    return math.factorial(n)


def create_factorial(n: int) -> int:
    result = 1
    for i in range(1, (n + 1)):
        result *= i
    return result
```

### sum_of_odd_numbers

<img src="https://i2.paste.pics/IQOOL.png" width="855" height="191" alt="Screenshot">

```python
def sum_of_odd_numbers(num: int) -> int:
    return sum(el for el in range(num + 1) if el % 2 == 1)
```
