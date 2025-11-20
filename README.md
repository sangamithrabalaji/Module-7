# PYTHON PROGRAMMMINDG MODULE 5

### NAME : SANGAMITHRA B
### REGISTER NUMBER : 212224060035
# Types of Recursion: Head Recursion in Python

##  AIM:
To write a Python program to demonstrate **Head Recursion** by finding and printing the sequence based on the sum of all digits (even or odd adjusted input).

## ALGORITHM:

1. **Start**
2. Define a recursive function `fun(n)`
3. In the function:
   - Create a recursive call at the **beginning** (Head Recursion)
   - Print the result after the recursive call
4. Take input from the user
5. If input is odd, convert it to the next even number
6. Call the recursive function
7. **Stop**

##  PROGRAM:
```
def even(n):
    if n==0:
        return
    even(n-1)
    if n%2==0:
        print(n,end=" ")
n=int(input())
even(n)
```

## OUTPUT
<img width="1027" height="270" alt="image" src="https://github.com/user-attachments/assets/4b79b245-6a38-4373-b1fa-eaddb61fd329" />


## RESULT
Thus, the program demonstrates how to print all even numbers from 1 to n using a recursive function and has been executed successfully.
#  Recursion:Palindrome Checker Using Recursion in Python

##  AIM:
To write a Python program to check whether a given string is a **palindrome** using **recursion**.

---

##  ALGORITHM:

1. **Start**
2. Define a recursive function `is_palindrome(word)`
   - **Base Case:** If the string length is less than 1, return `True`
   - **Recursive Case:** If the first and last characters match, call the function recursively on the substring without first and last characters
   - Else, return `False`
3. Get input from the user
4. Call the recursive function
5. Print whether the string is a palindrome
6. **Stop**

---

##  PROGRAM:
```
def is_palindrome(s):
    if len(s) <= 1:
        return True
    if s[0] != s[-1]:
        return False
    return is_palindrome(s[1:-1])
text = input()
cleaned = ''.join(text.split()).lower()
if is_palindrome(cleaned):
    print("Palindrome")
else:
    print("Not a Palindrome")
```
## OUTPUT

<img width="331" height="166" alt="image" src="https://github.com/user-attachments/assets/ab776b6b-c34e-4a6f-b76f-ab3b78ef462b" />

## RESULT
Thus, the program has been successfully executed.
# Recursion:Sum of Digits using Recursion in Python

## AIM:
To write a Python program to calculate the **sum of all digits** in a number using **recursion**.

##  ALGORITHM:

1. **Start**
2. Define a recursive function `sum_digit(n)` that:
   - Returns 0 if `n <= 0` (Base Case)
   - Else, returns `n % 10 + sum_digit(n // 10)` (Recursive Case)
3. Take integer input from the user.
4. Call the recursive function and store the result.
5. Print the result.
6. **Stop**

## PROGRAM:
```
def sum(n):
    n=abs(n)
    if n==0:
        return 0
    else:
        return n%10 +sum(n//10)
n=int(input())
print(sum(n))
```

## OUTPUT
<img width="1045" height="305" alt="image" src="https://github.com/user-attachments/assets/8575ddf3-95d9-45c7-8000-bb5fe3599c6c" />

## RESULT
Thus, the program has been successfully executed.
#  Taylor Series Using Recursion in Python

## AIM:
To write a Python program to evaluate a **Taylor Series** using **recursion**, where values of `x` and `n` are taken from the user.

## ALGORITHM:

1. **Start**
2. Create variables `x` and `n`
3. Get values for `x` and `n` from the user
4. Define a recursive function `series(x, n)`
   - **Base case:** If `n == 0`, return 1
   - **Recursive case:** Return `x**n / n + series(x, n-1)`
5. Print the result
6. **Stop**

## PROGRAM:
```
def series(x,n):
    if n==0:
        return 1
    else:
        return x**n+series(x,n-1)
x=int(input())
n=int(input())
print(series(x,n))
    
```

## OUTPUT
<img width="947" height="261" alt="image" src="https://github.com/user-attachments/assets/be9b72a1-cf7c-4dca-b9c5-aaa3f75bee26" />


## RESULT
Thus, the program has been successfully executed.
# Taylor Series:sinh(x) Evaluation using Recursion in Python

##  AIM:
To write a Python program to evaluate the value of **sinh(x)** for **n terms** using recursion.

---

## ALGORITHM:

1. **Start**
2. Read input for variable `x` (angle or number)
3. Read input for variable `n` (number of terms)
4. Define a function `fact(n)`:
   - If `n <= 1`, return 1
   - Else, return `n * fact(n - 1)` (recursive factorial)
5. Define a function `sinh(x, n)`:
   - If `n == 0`, return `x`
   - Else, return `(pow(x, 2*n + 1) / fact(2*n + 1)) + sinh(x, n - 1)`
6. Call the `sinh(x, n)` function and print the result
7. **Stop**

---

##  PROGRAM:
```
def series(x,n):
    if n==0:
        return x
    return x**(2*n+1)/fact(2*n+1)+series(x,n-1)
def fact(n):
    if n==0:
        return 1
    return n*fact(n-1)
x=int(input())
n=int(input())
result=series(x,n)
print(result)
```

## OUTPUT
<img width="1137" height="269" alt="image" src="https://github.com/user-attachments/assets/295b8bd9-7aa5-4471-9f38-6df4675a5aaf" />


## RESULT
Thus, the program has been successfully executed.
