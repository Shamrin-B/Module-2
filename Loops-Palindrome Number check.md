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
num = int(input("Enter a number: "))
temp = num
rev = 0

print("\nReversing process:")
while temp > 0:
    digit = temp % 10
    rev = (10 * rev) + digit
    print(f"Extracted digit: {digit}, Reversed so far: {rev}")
    temp = temp // 10

print(f"\nOriginal number: {num}")
print(f"Reversed number: {rev}")

if rev == num:
    print("Result: The number is a palindrome.")
else:
    print("Result: The number is not a palindrome.")
```
## Output
```
Enter a number: 121
Reversing process:
Extracted digit: 1, Reversed so far: 1
Extracted digit: 2, Reversed so far: 12
Extracted digit: 1, Reversed so far: 121

Original number: 121
Reversed number: 121
Result: The number is a palindrome.
```

## Result
Thus ,wwe have written a Python program that checks whether a given number is a **palindrome** using loops.

