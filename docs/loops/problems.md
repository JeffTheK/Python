# Problems

## Question 1

Write a function to print all letters in a string except `a` and `b`.

Solution

```python
for item in 'abhishekveeramalla':
    if letter == 'a' or letter == 'b':
        continue
    print(item)
```

## Question 2

Write a python program to print the below pattern. While it might look silly at the very first place but for a beginner such creative problems are very useful.

```txt
* 
* * 
* * * 
* * * * 
* * * * * 
```

Solution

```python
from __future__ import print_function
def pyramid(n):
    # number of rows
    for x in range(n):
        # number of columns
        for y in range(x+1):
            print("* ", end='')

        # new line
        print("\r")
 

if __name__ == '__main__':
    n = 5
    pyramid(n)
```

## Try by yourself

Write a python function to print the below pattern.

```txt
1 
1 2 
1 2 3 
1 2 3 4 
1 2 3 4 5 
```

Solution

```python
from __future__ import print_function
def pyramid(n):

    num = 1
    # number of rows
    for x in range(n):
        num = 1
        # number of columns
        for y in range(x+1):
            print(num, end=" ")
            # increment
            num = num + 1

        # new line
        print("\r")
 
# Driver code
n = 5
pyramid(n)
```
