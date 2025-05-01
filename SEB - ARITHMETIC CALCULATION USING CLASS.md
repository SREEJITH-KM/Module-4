# Exp.No:20  
## SEB - ARITHMETIC CALCULATION USING CLASS

---

### AIM  
To write a Python program to perform addition and division operations using a class. The class should be named `Saveetha`, and the function names should be `setvalues` (to set `a` and `b` values), `add`, and `div`. The program should handle the following cases:  
- `choice 1` → Perform addition  
- `choice 2` → Perform division  
- `choice 0` → Exit  
- For other choices, print 'Invalid choice'

---

### ALGORITHM

1. Begin the program.  
2. Create a class `Saveetha`.  
3. Define the following methods inside the `Saveetha` class:  
   - `__init__(self)`: Initializes `a` and `b` to zero.  
   - `setvalues(self, a, b)`: Sets the values of `a` and `b`.  
   - `add(self)`: Performs the addition operation.  
   - `div(self)`: Performs the division operation. If `b` is zero, returns an error message for division by zero.  
4. Create a `main()` function.  
5. Take input from the user for the values of `a` and `b` using `setvalues(a, b)` method.  
6. Use a `while True` loop to repeatedly ask the user for a choice:  
   - If the choice is 1, call the `add()` method and print the result.  
   - If the choice is 2, call the `div()` method and print the result. Handle division by zero.  
   - If the choice is 0, print "Exiting!" and exit the loop.  
   - If the choice is not 1, 2, or 0, print "Invalid choice".  
7. Terminate the program.

---

### PROGRAM

```
class Saveetha:
    def __init__(self):
        self.a = 0
        self.b = 1  # Default to 1 to avoid division by zero

    def setvalues(self, a, b):
        self.a = a
        self.b = b

    def add(self):
        return self.a + self.b

    def div(self):
        try:
            return self.a / self.b
        except ZeroDivisionError:
            return "Error: Division by zero is not allowed."

# Main program
if __name__ == "__main__":
    obj = Saveetha()

    while True:
        print("\nMenu:")
        print("1 → Perform addition")
        print("2 → Perform division")
        print("0 → Exit")

        try:
            choice = int(input("Enter your choice: "))
        except ValueError:
            print("Invalid input. Please enter a number.")
            continue

        if choice == 0:
            print("Exiting program.")
            break
        elif choice in [1, 2]:
            try:
                a = int(input("Enter value for a: "))
                b = int(input("Enter value for b: "))
            except ValueError:
                print("Invalid input. Please enter integer values.")
                continue

            obj.setvalues(a, b)

            if choice == 1:
                result = obj.add()
                print("Addition result:", result)
            elif choice == 2:
                result = obj.div()
                print("Division result:", result)
        else:
            print("Invalid choice")


```

### OUTPUT
![image](https://github.com/user-attachments/assets/c0bfd6fb-b2e6-43d6-80ba-39ca0a35c89a)


### RESULT
Thus the program is executed successfully
