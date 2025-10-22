# map()
```python
# 1. Use map() to double each element in a list.
# Example Input: [1, 2, 3, 4]
# Expected Output: [2, 4, 6, 8]

 def double(num):
     return num*2

 arr = [1, 2, 3, 4]
 ans = list(map(double,arr))
 print(ans)
```
```python
#2. Use map() to convert a list of integers to strings.
# Example Input: [10, 20, 30]
# Expected Output: ['10', '20', '30']

 def convert(num):
     return str(num)

 arr = [10, 20, 30]
 ans = list(map(convert, arr))
 print(ans)
```

```python
#3. Use map() to find the length of each word in a list of words.
# Example Input: ['cat', 'python', 'AI']
# Expected Output: [3, 6, 2]

 def count(s):
     return len(s)

 arr = ['cat', 'python', 'AI']
 ans = list(map(count,arr))
 print(ans)
```
```python
#4. Use map() with lambda to cube every number in a list.
# Example Input: [2, 3, 4]
# Expected Output: [8, 27, 64]

 arr = [2, 3, 4]
 ans = list(map(lambda x:x**3, arr))

 print(ans)
```
```python
#5. Convert a list of strings to uppercase using map().
# Example Input: ['a', 'b', 'c']
# Expected Output: ['A', 'B', 'C']

 def upperconvert(s):
     return s.upper()

 arr = ['a', 'b', 'c']
 ans = list(map(upperconvert, arr))
 print(ans)
```
```python
#6. Use map() to round float numbers to 2 decimals.
# Example Input: [1.234, 3.456, 5.678]
# Expected Output: [1.23, 3.46, 5.68]

 def findNum(val):
     return round(val ,2)

 arr = [1.234, 3.456, 5.678]
 ans = list(map(findNum, arr))
 print(ans)
```

```python
#7. Use map() to extract first character of each word.
# Example Input: ['apple', 'banana', 'cherry']
# Expected Output: ['a', 'b', 'c']

 def firstChar(s):
     return s[:1]

 arr = ['apple', 'banana', 'cherry']
 ans = list(map(firstChar, arr))
 print(ans)
```

```python
#8. Use map() to add elements from two lists.
# Example Input: [1, 2, 3], [4, 5, 6]
# Expected Output: [5, 7, 9]
def addlist(a, b):
    return a + b

arr1 = [1, 2, 3]
arr2 = [4, 5, 6]

ans = list(map(addlist, arr1, arr2))
print(ans)
```
```python
#9. Use map() to square even numbers only.
# Example Input: [1, 2, 3, 4]
# Expected Output: [1, 4, 3, 16]

 def square_even(num):
     return num if num%2!=0 else num**2

 arr = [1, 2, 3, 4]
 ans = list(map(square_even, arr))
 print(ans)

```
```python
#10. Use map() to find factorial of each number.
# Example Input: [3, 4, 5]
# Expected Output: [6, 24, 120]

 def fact(num):
     if num ==1:
         return 1
     return num*fact(num-1)

 arr = [3, 4, 5]
 ans = list(map(fact, arr))
 print(ans)

```

```python
#11. Use map() with str() to convert all elements to strings.
# Example Input: [True, False, None]
# Expected Output: ['True', 'False', 'None']

 def convert(elem):
     return str(elem)

 arr = [True, False, None]
 ans = list(map(convert, arr))
 print(ans)

```
```python
#12. Use map() to check if numbers are even or odd.
# Example Input: [1, 2, 3, 4]
# Expected Output: ['Odd', 'Even', 'Odd', 'Even']

 def check_num_type(num):
     return 'even' if num%2 == 0 else 'odd'

 arr = [1, 2, 3, 4]
 ans = list(map(check_num_type, arr))
 print(ans)

```

```python
#13. Use map() to concatenate fixed string to each element.
# Example Input: ['a', 'b', 'c']
# Expected Output: ['a_test', 'b_test', 'c_test']

 def add_string(s):
     return s+'_test'

 arr = ['a', 'b', 'c']
 ans = list(map(add_string, arr))
 print(ans)

```
```python
#14. Use map() to calculate the square root of numbers.
# Example Input: [4, 9, 16]
# Expected Output: [2.0, 3.0, 4.0]

 import math
 def square_root(num):
     return math.sqrt(num)

 arr = [4, 9, 16]
 ans = list(map(square_root, arr))
 print(ans)

```
```python
#15. Use map() with lambda to double list values only if greater than 5.
# Example Input: [2, 6, 8]
# Expected Output: [2, 12, 16]

 arr = [2, 6, 8]

 ans = list(map(lambda x: x*2 if x>5 else x, arr))
 print(ans)
```
