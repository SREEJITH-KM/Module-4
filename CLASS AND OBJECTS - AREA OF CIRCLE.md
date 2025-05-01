# Exp.No:19  
## CLASS AND OBJECTS - AREA OF CIRCLE

---

### AIM  
Write Python Program to take the radius from the user and find the area of the circle using class name 'umbrella' and function name 'rain'

---

### ALGORITHM

1. Begin the program.  
2. Create a class named `umbrella`.  
3. Define a method `rain(self, r)` inside the class `umbrella` that accepts a radius `r` as an argument.  
4. Inside the `rain` method:  
   - Calculate the area of a circle using the formula:  
     \[ \text{Area} = \pi \times r^2 \]  
   - Use the `math.pi` constant to get the value of π and perform the calculation.  
   - Print the result, formatted to two decimal places.  
5. Prompt the user for an integer input to represent the radius of the circle.  
6. Create an instance of the `umbrella` class and store it in the variable `u`.  
7. Call the `rain` method of the `umbrella` class, passing the user-provided radius `r` as an argument.  
8. Terminate the program.

---

### PROGRAM

```
import math

class pen:

    @staticmethod

    def stationary(radius):

        area=math.pi*radius**2

        return area

radius=float(input())

area=pen.stationary(radius)

print(f"Area of circle: {area:.2f}")



```

### OUTPUT
![image](https://github.com/user-attachments/assets/ec183f51-71e7-4170-acf8-2287cb0b3f62)



### RESULT
Thus the program is executed successfully


