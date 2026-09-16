
# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
```
class Rectangle:
    def __init__(self):
        self._length=5
        self._breath=3
    def values(self):
        print(self._length)
        print(self._breath)
        
rect=Rectangle()
rect.values()
```
## Output

<img width="757" height="202" alt="Screenshot (972)" src="https://github.com/user-attachments/assets/0c113b80-5248-4332-bdcd-57bd3bc21fee" />

## Result

Thus the program to implement Encapsulation in Python by defining a class Rectangle with private member variables __length and __breadth has been executed successfully.
