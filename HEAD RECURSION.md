# 🔁 Types of Recursion: Head Recursion in Python

## 🎯 AIM:
To write a Python program to demonstrate **Head Recursion** by finding and printing the sequence based on the sum of all digits (even or odd adjusted input).

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `fun(n)`
3. In the function:
   - Create a recursive call at the **beginning** (Head Recursion)
   - Print the result after the recursive call
4. Take input from the user
5. If input is odd, convert it to the next even number
6. Call the recursive function
7. **Stop**

## 💻 PROGRAM:
```
def sum_of_digits(num):
    """Helper function to calculate sum of digits of a number."""
    return sum(int(digit) for digit in str(num))

def fun(n):
    if n <= 0:
        return
    fun(n - 1)
    print(f"Current value: {n}, Sum of digits: {sum_of_digits(n)}")


num = int(input("Enter a positive integer: "))

if num % 2 != 0:
    num += 1

print(f"Adjusted input (even number): {num}\nSequence (head recursion):")
fun(num)
```

## OUTPUT
<img width="1254" height="256" alt="image" src="https://github.com/user-attachments/assets/7178a3ee-4bbf-4572-a585-fbc5814a037f" />

## RESULT
Hence  demonstrated **Head Recursion** by finding and printing the sequence based on the sum of all digits (even or odd adjusted input).
