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
import math
rows = int(input("Enter the number of rows: "))
for n in range(rows):
    # Step 4a: Print spaces to shape the triangle
    print(" " * (rows - n), end="")

    # Step 4b: Compute and print values using the formula C(n, k)
    for k in range(n + 1):
        value = math.comb(n, k)  # C(n, k) using math module in Python 3.8+
        print(f"{value} ", end="")

    # Move to the next line after each row
    print()

```


## Sample Output
![image](https://github.com/user-attachments/assets/52701a4b-d65f-44a7-a0f2-09e3de59fe1d)

## Result
Program executed successfully
