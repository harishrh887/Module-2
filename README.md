# Built-in Functions -Binary Conversion Using Built-in Functions in Python

## 🎯 Aim
To write a Python program to convert the number **16** into its **binary representation** using built-in Python functions.

## 🧠 Algorithm
1. Assign the value `16` to a variable `a`.
2. Use the built-in `bin()` function to convert the number to binary.
3. Print the result.

## 🧾 Program
```
a=int(input())
n=bin(a)
print(n)
```
## Output
<img width="256" height="163" alt="image" src="https://github.com/user-attachments/assets/109b5b91-1b43-4a95-9a22-dcd31fa471c7" />



## Result
Thus, the python program was executed successfully

# Functions in Python: Modulo Calculator

## 🎯 Aim
To write a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator.

## 🧠 Algorithm
1. Define a function called `result` that takes two arguments `a` and `b`.
2. Inside the function, compute the modulo using `a % b`.
3. Print the result of the modulo operation.
4. Get two integer inputs from the user.
5. Call the `result` function with the user-provided values.

## 🧾 Program
```
def result(a,b):
        return a%b
try:
    a=int(input())
    b=int(input())    
    
    if b==0:
        print("a is not allowed to divide by b")
    else:
        modulo=result(a,b)
        print("modulo is",modulo)
except value:        
           print("please enter the correct value")
```

## Output

<img width="561" height="234" alt="image" src="https://github.com/user-attachments/assets/8af44cf3-760f-4f7e-86b1-e44a907b7b7d" />



## Result

Thus, the python program was executed successfully

# Lambda Function in Python: Addition of Two Numbers

## 🎯 Aim
To write a Python program that defines a **lambda function** which takes two arguments `a` and `b`, and returns their sum.

## 🧠 Algorithm
1. Get two integer inputs from the user.
2. Use a **lambda function** to define a function `f` that returns `a + b`.
3. Call the function with the user inputs and print the result.

## 🧾 Program
```
add = lambda a, b, c: a + b + c
x = int(input())
y = int(input())
z = int(input())
result = add(x, y, z)
print(result)
```

## Output

<img width="561" height="234" alt="image" src="https://github.com/user-attachments/assets/271ebe87-a466-4e38-9e56-7757b46824d5" />



## Result
Thus, the python program was executed successfully

# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
```
def pascal_triangle(n):
    for i in range(n):
        row=[1]
        for j in range(1,i):
            row.append(prev_row[j-1]+prev_row[j])
        if i>0:
            row.append(1)
        print(" ".join(map(str,row)))
        prev_row=row
n=int(input())
pascal_triangle(n)
```

## Sample Output
<img width="452" height="406" alt="image" src="https://github.com/user-attachments/assets/426b3cf4-55f0-4c5c-b2d5-a32638a5474a" />


## Result
Thus,the Python program that generates Pascal's Triangle using numbers. The number of rows is accepted from the user is created successfully.

## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
```
num=int(input())
temp=num
rev=0
while temp>0:
    digit=temp%10
    rev=rev*10+digit
    temp//=10
    
if rev==num:
    print(f"The given number {num} is a Palindrome".format(num))
else:
    print(f"The given number {num} is not a palindrome".format(num))

```
## Output
<img width="705" height="174" alt="image" src="https://github.com/user-attachments/assets/c5fa4a50-32d3-421a-a69a-1745748996c8" />


## Result
Thus,the Python program that checks whether a given number is a palindrome using loops is created successfully
