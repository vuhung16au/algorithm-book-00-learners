

---

### Slide 1: Introduction
- **Title: Lecture 10: Data Abstraction**
- **Introduction:**
  - Data abstraction allows you to handle complex data structures by representing them in a simplified manner using classes and structs.
  - Understanding and applying data abstraction helps in managing and organizing code effectively, making it more maintainable and scalable.

---

### Part 2: Write a Program(s) (in Python) that Demonstrates <Outline>
- **Program 1: Student Information Management using Class**
  ```python
  class Student:
      def __init__(self, name, age, grade):
          self.__name = name
          self.__age = age
          self.__grade = grade

      # Getter for name
      def get_name(self):
          return self.__name

      # Setter for name
      def set_name(self, name):
          self.__name = name

      # Getter for age
      def get_age(self):
          return self.__age

      # Setter for age
      def set_age(self, age):
          self.__age = age

      # Getter for grade
      def get_grade(self):
          return self.__grade

      # Setter for grade
      def set_grade(self, grade):
          self.__grade = grade

  # Example usage
  student = Student("John Doe", 16, "10th Grade")
  print(student.get_name())  # Output: John Doe
  student.set_age(17)
  print(student.get_age())  # Output: 17
  ```

- **Program 2: Find the Farthest Point in 2D Coordinate System**
  ```python
  class Point:
      def __init__(self, x, y):
          self.x = x
          self.y = y

      def distance_from_origin(self):
          return (self.x**2 + self.y**2)**0.5

  def farthest_point(points):
      max_distance = 0
      farthest = None
      for point in points:
          distance = point.distance_from_origin()
          if distance > max_distance:
              max_distance = distance
              farthest = point
      return farthest

  # Example usage
  points = [Point(1, 2), Point(3, 4), Point(-5, -6)]
  farthest = farthest_point(points)
  print(f"Farthest Point: ({farthest.x}, {farthest.y})")  # Output: Farthest Point: (-5, -6)
  ```

---

### Part 3: Takeaways for Students
- **Important Notes:**
  - Data abstraction through classes and structs helps encapsulate data and behavior.
  - Using getters and setters provides control over how data attributes are accessed and modified.
  - Proper abstraction can lead to better code organization and maintainability.

---

### Part 4: Assignments for Students
- **Assignment 1: Employee Information Management**
  - Write a class to manage employee information, including attributes like name, ID, and department. Implement getters and setters for each attribute.
  
- **Assignment 2: Closest Point to Origin**
  - Write a program to find the point closest to the origin in a 2D coordinate system using a class.

---

### Part 5: "Did You Know?"
- **Interesting Fact:**
  - The concept of data abstraction in programming is inspired by abstract data types in mathematics, which define operations without specifying implementation details.
  - In many programming languages, the use of classes and objects helps implement data abstraction, promoting reusability and modularity.

---

### Part 6: "Interesting Fact"
- **Fact:**
  - The first high-level programming language to introduce data abstraction concepts was Simula, developed in the 1960s. Simula laid the foundation for modern object-oriented programming languages.

---

### Part 7: "Fun Challenge"
- **Challenge:**
  - Create a class representing a geometric shape (e.g., Circle, Rectangle). Implement methods to calculate area and perimeter. Extend the class to handle different types of shapes and their properties.

---

