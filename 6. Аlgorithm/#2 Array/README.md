# Array

###                       

> if from list(array) i(index) remove which in the beginning or middle it do many operations, because array need to
> shift other el to this free space

### is_palindrome

<img src="https://i2.paste.pics/IQPEI.png" width="664" height="216" alt="Screenshot">

```python
# palindrome is words which is same if reverse
def is_palindrome(word: str) -> bool:
    """aziza , kiyik || anora"""
    # O(n) RAM, O(2n) = O(n) Time
    # return word == word[::-1]
    low, high = 0, len(word) - 1

    while low < high:
        if word[low] == word[high]:
            return False
        low += 1
        high += 1
    # O(1) RAM, O(n/2) Time
    return True
```

### merge_two_arrays

<img src="https://i2.paste.pics/IQPJ4.png" width="662" height="216" alt="Screenshot">
<img src="https://i2.paste.pics/IQPMA.png" width="390" height="392" alt="Screenshot">

```python
def merge_two_arrays(arr1: list[int], arr2: list[int]) -> list:
    i = j = 0
    n, m = len(arr1), len(arr2)
    result = []

    while i < n and j < m:
        if arr1[i] < arr2[j]:
            result.append(arr1[i])
            i += 1
        else:
            result.append(arr2[j])

    while i < n:
        result.append(arr1[i])
        i += 1

    while j < m:
        result.append(arr2[j])
        j += 1

    return result

```