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
# Step 1: Get input from the user
num = int(input("Enter a number: "))

# Step 2: Assign the value to a temporary variable
temp = num

# Step 3: Initialize rev to 0
rev = 0

# Step 4: Reverse the digits using a while loop
while temp > 0:
    rev = (10 * rev) + (temp % 10)
    temp = temp // 10

# Step 5: Check if the number is a palindrome
if rev == num:
    print("The number is a palindrome.")
else:
    print("The number is not a palindrome.")

```
## Output
![image](https://github.com/user-attachments/assets/3c5bdfc7-8d19-45bf-bf2f-727cd0827496)

## Result
Program executed successfully.
