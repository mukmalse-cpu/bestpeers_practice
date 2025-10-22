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

# filter()



```python
#     16. Use filter() to extract even numbers from a list.
# Example Input: [1, 2, 3, 4, 5, 6]
# Expected Output: [2, 4, 6]

def even_only(num):
    return num if num%2==0 else None

arr = [1, 2, 3, 4, 5, 6]

ans = list(filter(even_only, arr))
print(ans)
```

```python
#     17. Use filter() to get numbers greater than 10.
# Example Input: [5, 10, 15, 20]
# Expected Output: [15, 20]

def greater_than_10(num):
    return num if num>10 else None

arr = [5, 10, 15, 20]
ans = list(filter(greater_than_10, arr))

print(ans)
```

```python
#     18. Use filter() to remove empty strings.
# Example Input: ['apple', '', 'banana', '', 'cherry']
# Expected Output: ['apple', 'banana', 'cherry']

arr = ['apple', '', 'banana', '', 'cherry']
ans = list(filter(lambda x: len(x)>0, arr))
print(ans)
```

```python
#     19. Use filter() to find numbers divisible by 3.
# Example Input: [1, 3, 4, 6, 9]
# Expected Output: [3, 6, 9]

def div_by_3(num):
    return num if num%3==0 else None

arr = [1, 3, 4, 6, 9]
ans = list(filter(div_by_3, arr))

print(ans)
```

```python
#     20. Use filter() to remove negative numbers.
# Example Input: [-2, -1, 0, 1, 2]
# Expected Output: [0, 1, 2]

def positive_num(num):
    if num==0:
        return '0'
    return num if num>0 else None

arr = [-2, -1, 0, 1, 2]
ans = list(filter(positive_num, arr))
print(ans)
```

```python
#     21. Use filter() to get words starting with 'a'.
# Example Input: ['apple', 'banana', 'avocado']
# Expected Output: ['apple', 'avocado']

def check_first_char(s):
    return s if s[0].lower()=='a' else None

arr = ['apple', 'banana', 'avocado']
ans = list(filter(check_first_char, arr))
print(ans)
```

```python
#     22. Use filter() to find prime numbers.
# Example Input: [2, 3, 4, 5, 6, 7]
# Expected Output: [2, 3, 5, 7]

def check(n):
    i = 2
    if n==1:
        return False
    if n==2:
        return True
    
    last = n//2
    while i<=last:
        if n%i==0:
            return False
        else:
            i+=1
    
    return True

def prime(num):
    return num if check(num) else None

arr = [2, 3, 4, 5, 6, 7]
ans = list(filter(prime, arr))
print(ans)
```

```python
#     23. Use filter() to find strings longer than 4 characters.
# Example Input: ['cat', 'tiger', 'lion']
# Expected Output: ['tiger']

def check_len(s):
    return s if len(s)>4 else None

arr = ['cat', 'tiger', 'lion']
ans = list(filter(check_len, arr))

print(ans)
```

```python
#     24. Use filter() to remove None values.
# Example Input: [1, None, 2, None, 3]
# Expected Output: [1, 2, 3]

def check_none(val):
    return val if val!= None else None

arr = [1, None, 2, None, 3]
ans = list(filter(check_none, arr))
print(ans)
```

```python
#     25. Use filter() to select people older than 18.
# Example Input: [('John', 15), ('Emma', 22)]
# Expected Output: [('Emma', 22)]

arr = [('John', 15), ('Emma', 22)]
ans = list(filter(lambda x: x[1]>18, arr))
print(ans)
```

```python
#     26. Use filter() to extract float values from a mixed list.
# Example Input: [1, 2.3, 'a', 4.5]
# Expected Output: [2.3, 4.5]

arr = [1, 2.3, 'a', 4.5]
ans = list(filter(lambda x: type(x)==float, arr))
print(ans)
```

```python
#     27. Use filter() to find palindromes.
# Example Input: ['madam', 'cat', 'level']
# Expected Output: ['madam', 'level']

arr = ['madam', 'cat', 'level']
ans = list(filter(lambda x: x==x[::-1], arr))
print(ans)
```

```python
#     28. Use filter() with lambda to get numbers between 10 and 20.
# Example Input: [5, 12, 18, 25]
# Expected Output: [12, 18]

arr = [5, 12, 18, 25]
ans = list(filter(lambda x: x>=10 and x<=20, arr))
print(ans)
```

```python
#     29. Use filter() to keep only uppercase strings.
# Example Input: ['HELLO', 'World', 'PYTHON']
# Expected Output: ['HELLO', 'PYTHON']

def check_uppercase(s):
    return s if s==s.upper() else None

arr = ['HELLO', 'World', 'PYTHON']
ans = list(filter(check_uppercase, arr))
print(ans)
```

```python
#     30. Use filter() to remove duplicates from a list.
# Example Input: [1, 2, 2, 3, 3, 4]
# Expected Output: [1, 2, 3, 4]


def check_elem(num):
    if num in seen:
        return False
    else:
        seen.add(num) 
        return True
    
arr = [1, 2, 2, 3, 3, 4]
seen = set()
ans = list(filter(check_elem, arr))
print(ans)
```
