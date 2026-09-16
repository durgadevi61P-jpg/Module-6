# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
```
from abc import ABC, abstractmethod

# Abstract base class
class type_shape(ABC):
    @abstractmethod
    def area(self):
        pass

# Rectangle subclass
class Rectangle(type_shape):
    def __init__(self, length, width):
        self.length = length
        self.width = width

    def area(self):
        return self.length * self.width

# Square subclass
class Square(type_shape):
    def __init__(self, side):
        self.side = side

    def area(self):
        return self.side * self.side

# Circle subclass using π = 3.14
class Circle(type_shape):
    def __init__(self, radius):
        self.radius = radius

    def area(self):
        return round(3.14 * self.radius ** 2, 2)  # Use 3.14 for π to match the expected output

# Triangle subclass
class Triangle(type_shape):
    def __init__(self, base, height):
        self.base = base
        self.height = height

    def area(self):
        return 0.5 * self.base * self.height

# Creating instances
rect = Rectangle(6, 4)
circle = Circle(7)
square = Square(4)
triangle = Triangle(4, 5)

# Output results
print("Area of a rectangle:", rect.area())
print("Area of a circle:", circle.area())
print("Area of a square:", square.area())
print("Area of a triangle:", triangle.area())
```
## Output
<img width="744" height="250" alt="Screenshot (971)" src="https://github.com/user-attachments/assets/de40769d-6f32-4457-b618-b73fb581c3fa" />

## Result
Thus the program of abstract class has been executed successfully.
