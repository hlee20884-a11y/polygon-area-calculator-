# Build a Polygon Area Calculator

A Python program to calculate properties of rectangles and squares.  
This project allows you to calculate area, perimeter, diagonal, visualize the shape with ASCII art, and determine how many squares fit inside a rectangle.

## Features
- Calculate area, perimeter, and diagonal of rectangles and squares
- Draw a visual representation of the shape using asterisks
- Update dimensions of shapes
- Determine how many smaller shapes can fit inside a larger rectangle
- Object-oriented implementation with inheritance (Square inherits from Rectangle)

## Example Usage
```python
from polygon_calculator import Rectangle, Square

# Rectangle example
rect = Rectangle(4, 5)
print("Rectangle area:", rect.get_area())            # 20
print("Rectangle perimeter:", rect.get_perimeter())  # 18
print("Rectangle diagonal:", rect.get_diagonal())    # ~6.403
print("Rectangle picture:\n", rect.get_picture())
print("Rectangle __str__:", rect)                    # Rectangle(width=4, height=5)

# Square example
sq = Square(4)
print("\nSquare area:", sq.get_area())               # 16
print("Square perimeter:", sq.get_perimeter())       # 16
print("Square diagonal:", sq.get_diagonal())         # ~5.657
print("Square picture:\n", sq.get_picture())
print("Square __str__:", sq)                         # Square(side=4)

# Update square side
sq.set_side(6)
print("\nUpdated Square area:", sq.get_area())       # 36
print("Updated Square __str__:", sq)                # Square(side=6)

# Check how many squares fit inside rectangle
rect2 = Rectangle(10, 12)
print("\nHow many squares fit inside rectangle:", rect2.get_amount_inside(sq))  # 2

Class Structure
	•	Rectangle
	•	width, height
	•	Methods: set_width, set_height, get_area, get_perimeter, get_diagonal, get_picture, get_amount_inside, __str__
	•	Square (inherits Rectangle)
	•	side
	•	Methods: set_side, overrides set_width and set_height, __str__

Objectives
	•	Practice object-oriented programming in Python
	•	Understand inheritance (Square inherits from Rectangle)
	•	Calculate geometric properties programmatically
	•	Learn to draw simple ASCII shapes
	•	Handle shape fitting and dimension updates
