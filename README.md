Assignment: Introduction to Python

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

   Python is an interpreted, object-oriented, high-level programming language with dynamic semantics.

   key features that make it popular among developers:

   a) Readability: Python uses indentation and a clean syntax, making it easy to read and write.

   b) Versatility: It supports multiple programming paradigms, including procedural, object-oriented, and functional programming.

   c) Large Standard Library: Python comes with a comprehensive standard library, reducing the need for external dependencies.

   d) Extensive Third-Party Packages: The Python Package Index (PyPI) offers a vast collection of additional libraries and frameworks.

   e) Cross-platform Compatibility: Python runs on various operating systems, including Windows, macOS, and Linux.

   f) Interpreted Nature: Python code is executed line by line, making debugging easier.

   g) Dynamic Typing: Variables don't need to be declared with specific types, increasing flexibility.

   (Python Software Foundation, 2024)
   
   Examples of use cases where Python is particularly effective:

   a) Web Development: Python frameworks like Django and Flask make it easy to build robust web applications:
   
   from flask import Flask
   
   app = Flask(__name__)

   @app.route('/')

   def hello_world():
    
      return 'Hello, World!'

   if __name__ == '__main__':
      
      app.run()
   
   b) Data Analysis and Visualization: Libraries like Pandas, NumPy, and Matplotlib are powerful tools for data manipulation and visualization:

   import pandas as pd

   import matplotlib.pyplot as plt

   data = pd.read_csv('data.csv')

   data.plot(kind='bar')

   plt.show()

   c) Machine Learning and AI: Libraries such as TensorFlow and scikit-learn make implementing machine learning algorithms straightforward.
   
   from sklearn.model_selection import train_test_split
   
   from sklearn.linear_model import LogisticRegression

   X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
   
   model = LogisticRegression()
   
   model.fit(X_train, y_train)
   
   d) Automation and Scripting: Python's simplicity makes it ideal for writing scripts to automate tasks.

   import os

   for filename in os.listdir('.'):

      if filename.endswith('.txt'):

         print(f"Processing {filename}")

         # Add your file processing logic here
   
   e) Scientific Computing: Libraries like SciPy make Python suitable for complex scientific and mathematical computations.

   from scipy import optimize

   def f(x):

      return x**2 + x + 2

   minimum = optimize.fmin(f, 0)

   print(f"The minimum of the function is at x = {minimum[0]}")

   
   (BoTree Technologies, 2023; Inc, 2021)
   

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   1. Installing Python on Windows:
   
   a) Go to python.org/downloads
   
   b) Download the latest Python installer for Windows.

   c) Run the installer, checking "Add Python to PATH"

   d) Click "Install Now"

   2. Verifying the installation:

   - Open a terminal or command prompt and type:

      python --version

   - This should display the installed Python version.

   3. Setting up a virtual environment:

   a) Open a terminal or command prompt.

   b) Navigate to your project directory.

   c) Install a virtual environment by typing:

      python -m pip install virtualenv

   d) Name the virtual environment by typing:

      python -m virtualenv "name"

   e) Activate the virtual environment by typing:

      source "name"/Scripts/activate

   f) The verification of activation is through seeing the name of virtual environment in the prompt

   g) To deactivate the virtual environment type:

      deactivate

(Sphinx & Furo, 2017)


3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

   Here is the python program that prints "Hello,World!"

      print("Hello, World!")

   Explanation of the basic syntax elements:

   a) Function call: print() is a built-in Python function used to output text to the console.

   b) Parentheses: The parentheses () are used to enclose the arguments passed to a function.

   c) String literal: "Hello, World!" is a string literal enclosed in double quotes. Python also allows single quotes for strings.

   d) Statement: This single line is a complete Python statement.In Python, most simple statements are written on a single line.

   e) No semicolon: Unlike some other programming languages, Python doesn't require semicolons at the end of statements.

   f) Indentation: While not visible in this one-line example, Python uses indentation to define code blocks in more complex structures (like loops or functions).

   To run this program:

   a) Save it in a file with a .py extension, e.g., hello.py.

   b) Open a terminal or command prompt.

   c) Navigate to the directory containing the file.

   d) Run the program using the command:

      python hello.py

   e) This will output:

      Hello, World!

(geeksforgeeks, 2023)


4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

   Basic Data Types in Python:

   - Text type: strings

   - Numeric types: integers, float, complex

   - Sequence types: list, tuple, range

   - Mapping type: dictionaries

   - Set types: set, frozenset

   - Boolean type: booleans

   - Binary types: bytes, bytearray, memoryview

   - None Type: NoneType

   a) Integers (int): Whole numbers, positive or negative.

   b) Floating-point numbers (float): Numbers with decimal points.

   c) Strings (str): Sequences of characters, enclosed in quotes.

   d) Booleans (bool): True or False values.

   e) Lists: Ordered, mutable sequences of elements.

   f) Tuples: Ordered, immutable sequences of elements.

   g) Dictionaries (dict): Key-value pairs.

   h) Sets: Unordered collections of unique elements.

(W3schools, 2023)

   script demonstrating the creation and use of variables with these data types:

   # Integers

   age = 30

   print(f"Age (int): {age}")

   # Floating-point numbers

   height = 1.75
   
   print(f"Height (float): {height}")

   # Strings

   name = "Alice"
   
   print(f"Name (str): {name}")

   # Booleans

   is_student = True
   
   print(f"Is student? (bool): {is_student}")

   # Lists

   hobbies = ["reading", "swimming", "coding"]
   
   print(f"Hobbies (list): {hobbies}")

   # Tuples

   coordinates = (10, 20)

   print(f"Coordinates (tuple): {coordinates}")

   # Dictionaries

   person = {"name": "Bob", "age": 25, "city": "New York"}

   print(f"Person (dict): {person}")

   # Sets
   
   unique_numbers = {1, 2, 3, 4, 5, 5}  # Note: duplicate 5 will be removed

   print(f"Unique numbers (set): {unique_numbers}")

   # Demonstrating type checking
   
   print(f"Type of age: {type(age)}")
   
   print(f"Type of height: {type(height)}")
   
   print(f"Type of name: {type(name)}")
   
   print(f"Type of is_student: {type(is_student)}")
   
   print(f"Type of hobbies: {type(hobbies)}")
   
   print(f"Type of coordinates: {type(coordinates)}")
   
   print(f"Type of person: {type(person)}")
   
   print(f"Type of unique_numbers: {type(unique_numbers)}")

   This script demonstrates:

   a) Creating variables of different types
   
   b) Using f-strings for formatted output
   
   c) Basic operations with each data type
   
   d)Using the type() function to check the data type of a variable

   When you run this script, it will output information about each variable and its type. This showcases how Python's dynamic typing allows you to easily work with different data types without explicit declarations.


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

   Conditional statements and loops are fundamental control structures in Python that allow you to control the flow of your program.

   a) Conditional Statements (if-else):

   Conditional statements allow you to execute different code blocks based on certain conditions. The basic structure is:

   if condition:

    # code to execute if condition is True

   elif another_condition:
    
    # code to execute if another_condition is True

   else:
    # code to execute if all conditions are False


   Example of an if-else statement:

   age = 20

   if age < 18:
      
      print("You are a minor.")

   elif age >= 18 and age < 65:
      
      print("You are an adult.")

   else:
    
    print("You are a senior citizen.")

   # Output: You are an adult.


   In this example:

   - If age is less than 18, it prints "You are a minor."

   - If age is between 18 and 64 (inclusive), it prints "You are an adult."

   - If age is 65 or greater, it prints "You are a senior citizen."

   b) Loops:

   Loops allow you to repeat a block of code multiple times. Python has two main types of loops: for and while. Let's focus on the for loop.

   The for loop is used to iterate over a sequence (like a list, tuple, string, or range) or other iterable objects. The basic structure is:

   for item in iterable:
    
    # code to execute for each item

   Example of a for loop:

   fruits = ["apple", "banana", "cherry"]

   for fruit in fruits:
      
      print(f"I like {fruit}.")

   # Output:

   # I like apple.

   # I like banana.
   
   # I like cherry.

   In this example:

   - The loop iterates over each item in the fruits list.
   
   - For each iteration, the current item is assigned to the variable fruit.
   
   - The print statement is executed for each fruit.


   Another common use of for loops is with the range() function:

   for i in range(5):
      print(f"Iteration {i}")

   # Output:

   # Iteration 0

   # Iteration 1
   
   # Iteration 2
   
   # Iteration 3
   
   # Iteration 4

   This loop iterates 5 times, with i taking values from 0 to 4.

   Both conditional statements and loops can be combined and nested to create more complex program logic. For example:

   numbers = [1, 2, 3, 4, 5]

   for num in numbers:
      
      if num % 2 == 0:
         
         print(f"{num} is even")
      
      else:
         
         print(f"{num} is odd")

   # Output:

   # 1 is odd
   
   # 2 is even
   
   # 3 is odd
   
   # 4 is even
   
   # 5 is odd

   This example combines a for loop with an if-else statement to categorize numbers as even or odd.

   These control structures are essential for writing dynamic and responsive Python programs. They allow you to make decisions and repeat actions based on the state of your program and its data.

(W3Schools, 2019)

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   Functions in Python are reusable blocks of code that perform a specific task.

   They are useful for several reasons:

   a) Code reusability: You can write a function once and use it multiple times.
   
   b) Modularity: Functions help break down complex problems into smaller, manageable parts.

   c) Abstraction: They allow you to hide complex implementations behind a simple interface.

   d) Organization: Functions help structure your code logically.

   Here's a Python function that takes two arguments and returns their sum, followed by an example of how to call it:

   def add_numbers(a, b):

      """
      This function takes two numbers and returns their sum.
    
      Parameters:
    
      a (int or float): The first number
      
      b (int or float): The second number
    
      Returns:
      
      int or float: The sum of a and b
      
      """
    return a + b

   # Example of calling the function

   result = add_numbers(5, 3)

   print(f"The sum of 5 and 3 is: {result}")

   # Another example with different numbers
   
   print(f"The sum of 10.5 and 7.3 is: {add_numbers(10.5, 7.3)}")

   Detailed explanantion:

   a) Function Definition:

   - def keyword is used to define a function.
   
   - add_numbers is the function name.
   
   - (a, b) are the parameters the function accepts.

   b) Docstring:

   - The triple-quoted string right after the function definition is a docstring.

   - It provides a description of what the function does, its parameters, and what it returns.

   c) Function Body:

   - The return statement specifies what the function should output.

   - In this case, it returns the sum of a and b.

   d) Calling the Function:

   - We call the function by using its name followed by parentheses containing the arguments.

   - add_numbers(5, 3) calls the function with 5 and 3 as arguments.

   - The result is stored in the result variable.

   e) Printing the Result:

   - We use f-strings to format the output nicely.

   f) Direct Use in Print:

   - In the second example, we call the function directly within the print statement.

   - This demonstrates that you can use functions wherever you need their return value.

   
   When you run this script, it will output:

   The sum of 5 and 3 is: 8
   
   The sum of 10.5 and 7.3 is: 17.8

   
   This function demonstrates several key concepts:

   - Taking multiple parameters

   - Performing a calculation

   - Returning a value

   - Flexibility in handling both integers and floats

   - Usage of docstrings for documentation

   Functions like this can be used as building blocks for more complex programs, allowing you to write cleaner, more organized, and more reusable code.

(Simplilearn, 2024)


7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   Lists and dictionaries are both essential data structures in Python, but they have different characteristics and use cases.

   Lists:

   - Ordered collection of items

   - Items accessed by index

   - Mutable (can be modified after creation)

   - Can contain duplicate elements

   - Use square brackets []

   Dictionaries:

   - Unordered collection of key-value pairs

   - Items accessed by key

   - Mutable

   - Keys must be unique (values can be duplicate)

   - Use curly braces {}

   Here's a script that creates a list of numbers and a dictionary, then demonstrates basic operations on both:

   # Creating a list of numbers
   
   numbers = [1, 2, 3, 4, 5]

   # Creating a dictionary
   person = {
      
      "name": "Alice",
      
      "age": 30,
      
      "city": "New York"
   
   }

   # List operations

   print("List Operations:")
   
   print(f"Original list: {numbers}")

   # Accessing elements

   print(f"First element: {numbers[0]}")
   
   print(f"Last element: {numbers[-1]}")

   # Adding an element
   
   numbers.append(6)
   
   print(f"After append: {numbers}")

   # Inserting an element
   
   numbers.insert(2, 10)
   
   print(f"After insert: {numbers}")

   # Removing an element
   
   numbers.remove(4)
   
   print(f"After remove: {numbers}")

   # Slicing
   
   print(f"Slice [1:4]: {numbers[1:4]}")

   # List comprehension
   
   squares = [x**2 for x in numbers]
   
   print(f"Squares: {squares}")

   print("\nDictionary Operations:")
   
   print(f"Original dictionary: {person}")

   # Accessing values
   
   print(f"Name: {person['name']}")

   # Adding a new key-value pair
   
   person['job'] = 'Engineer'
   
   print(f"After adding 'job': {person}")

   # Modifying a value
   
   person['age'] = 31
   
   print(f"After modifying 'age': {person}")

   # Removing a key-value pair
   
   del person['city']
   
   print(f"After deleting 'city': {person}")

   # Checking if a key exists
   
   print(f"'name' in person: {'name' in person}")
   
   print(f"'city' in person: {'city' in person}")

   # Getting all keys and values
   
   print(f"Keys: {list(person.keys())}")
   
   print(f"Values: {list(person.values())}")

   # Getting items as tuples
   
   print(f"Items: {list(person.items())}")

   # Using get() method with a default value
   
   print(f"Salary (default 0): {person.get('salary', 0)}")

   This script demonstrates:

   For lists:

   a) Creating a list
   
   b) Accessing elements by index
   
   c) Adding elements with append() and insert()
   
   d) Removing elements with remove()
   
   e) Slicing
   
   f) List comprehension

   For dictionaries:

   a) Creating a dictionary

   b) Accessing values by key
   
   c) Adding new key-value pairs
   
   d) Modifying values

   e) Removing key-value pairs

   f) Checking for key existence

   g) Getting all keys, values, and items

   h) Using the get() method with a default value

   When you run this script, it will output the results of these operations, showing how lists and dictionaries behave differently.

   Key differences highlighted in the script:

   a) Lists use numeric indices, while dictionaries use keys

   b) Lists maintain order, while dictionaries don't guarantee order

   c) List operations often involve changing the structure (adding/removing elements), while dictionary operations often involve manipulating key-value pairs

   This script provides a practical demonstration of how these two data structures are used in Python, highlighting their unique characteristics and common operations.

(Singh, 2023)

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

   Exception handling in Python is a mechanism to deal with errors and unexpected situations that may occur during program execution. It allows you to gracefully handle errors, prevent your program from crashing, and provide meaningful error messages or alternative actions when something goes wrong.

   The key components of exception handling in Python are:

   a) try: The code block where an exception might occur.

   b) except: The code block that handles the exception if it occurs.

   c) finally: The code block that always executes, regardless of whether an exception occurred or not.

   d) else: (optional) The code block that executes if no exception occurs.

   Here's an example that demonstrates the use of try, except, and finally blocks:

   def divide_numbers(a, b):
      
      try:
         
         result = a / b
         
         print(f"The result of {a} divided by {b} is: {result}")
      
      except ZeroDivisionError:
         
         print("Error: Cannot divide by zero!")
      
      except TypeError:
         
         print("Error: Please provide numeric values!")
      
      else:
         
         print("Division operation completed successfully.")
      
      finally:
         
         print("This block always executes, regardless of exceptions.")

   # Test cases

   print("Case 1:")
   
   divide_numbers(10, 2)

   print("\nCase 2:")
   
   divide_numbers(10, 0)

   print("\nCase 3:")
   
   divide_numbers("10", 2)

   print("\nCase 4:")

   divide_numbers(10, "2")


   Detailed explanation of the example:

   a) We define a function divide_numbers that attempts to divide two numbers.
   
   b) The try block contains the code that might raise an exception (the division operation).

   c) We have two except blocks:

   - One catches ZeroDivisionError, which occurs when trying to divide by zero.

   - Another catches TypeError, which occurs when trying to perform division with non-numeric types.

   d) The else block executes if no exception occurs, confirming successful division.

   e) The finally block always executes, demonstrating code that runs regardless of exceptions.

   f) We test the function with different inputs to showcase various scenarios.

   When you run this script, it will output:

   Case 1:
   
   - The result of 10 divided by 2 is: 5.0

   - Division operation completed successfully.
   
   - This block always executes, regardless of exceptions.

   Case 2:
   
   - Error: Cannot divide by zero!
   
   - This block always executes, regardless of exceptions.

   Case 3:

   - Error: Please provide numeric values!

   - This block always executes, regardless of exceptions.

   Case 4:
   
   - Error: Please provide numeric values!

   - This block always executes, regardless of exceptions.


   This example demonstrates several key concepts of exception handling:

   a) Multiple except blocks to handle different types of exceptions.

   b) Specific exception handling (ZeroDivisionError, TypeError) rather than catching all exceptions, which is generally a good practice.
   
   c) The else block to execute code when no exception occurs.
   
   e) The finally block to execute cleanup or finalization code, regardless of whether an exception occurred.

   Exception handling is crucial for writing robust Python programs that can gracefully handle errors and unexpected situations. It allows you to provide better user experiences, log errors for debugging, and ensure that your program behaves predictably even when things go wrong.

   (Satyam, 2020)

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

   Modules and packages are fundamental concepts in Python for organizing and reusing code.

   Modules:

   - A module is a Python file containing functions, classes, and variables that can be used in other Python scripts. It helps in organizing related code into a single file.

   Packages:

   - A package is a collection of related modules organized in a directory hierarchy. It's essentially a directory containing a special file called init.py, which marks the directory as a Python package.

(Singh, 2023a)

   Importing and Using Modules:
   
   You can import modules using the import statement. There are several ways to import modules:

   a) Import the entire module by typing:

         import module_name

   b) Import specific items from a module by typing:

         from module_name import item_name

   c) Import all items from a module (not recommended for large modules):

         from module_name import *

   d) Import with an alias by typing:

         import module_name as alias

   Example using the math module:

   Let's create a script that demonstrates how to import and use the math module:

   # Importing the entire math module

   import math

   # Importing specific functions from math

   from math import sqrt, pi

   # Importing with an alias

   import math as m

   def circle_calculations(radius):
      # Using the full module name
      
      area = math.pi * radius**2
    
      # Using the imported pi constant
      
      circumference = 2 * pi * radius
    
      # Using the imported sqrt function
      
      diameter = 2 * sqrt(area / pi)
    
      # Using the aliased module
      
      volume = (4/3) * m.pi * radius**3
    
      return area, circumference, diameter, volume

   # Test the function
   radius = 5
   
   area, circumference, diameter, volume = circle_calculations(radius)

   print(f"Circle with radius {radius}:")
   
   print(f"Area: {area:.2f}")
   
   print(f"Circumference: {circumference:.2f}")
   
   print(f"Diameter: {diameter:.2f}")
   
   print(f"Volume of sphere: {volume:.2f}")

   # Using other math functions
   
   angle = 45
   
   print(f"\nSine of {angle} degrees: {math.sin(math.radians(angle)):.4f}")
   
   print(f"Cosine of {angle} degrees: {math.cos(math.radians(angle)):.4f}")

   # Demonstrating math constants
   
   print(f"\nValue of pi: {math.pi:.6f}")
   
   print(f"Value of e: {math.e:.6f}")


   This script demonstrates:

   a) Importing the entire math module.
   
   b) Importing specific functions (sqrt and pi) from the math module.
   
   c) Importing the math module with an alias m.
   
   d) Using various functions and constants from the math module in different ways.
   
   e) Creating a function that utilizes these imported items.


   When you run this script, it will output:

   Circle with radius 5:
   
   Area: 78.54
   
   Circumference: 31.42
   
   Diameter: 10.00
   
   Volume of sphere: 523.60

   Sine of 45 degrees: 0.7071
   
   Cosine of 45 degrees: 0.7071

   
   Value of pi: 3.141593
   
   Value of e: 2.718282


   This example showcases how modules like math provide a wealth of pre-defined functions and constants that you can easily import and use in your Python scripts. It also demonstrates different importing techniques and how they affect the way you use the imported items in your code.

   Using modules and packages helps in:

   a) Code organization and reusability
   
   b) Namespace management (avoiding naming conflicts)
   
   c) Enhancing readability by grouping related functionality
   
   d) Leveraging existing code and standard libraries



10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

    File I/O (Input/Output) operations are common tasks in Python programming. Here are two scripts demonstrating how to read from and write to files:

    a) Reading from a file and printing to console:
    
    def read_file(filename):
      
      try:
         
         with open(filename, 'r') as file:
            
            content = file.read()
            
            print("File contents:")
            
            print(content)
      
      except FileNotFoundError:
         
         print(f"Error: The file '{filename}' was not found.")
      
      except IOError:
         
         print(f"Error: There was an issue reading the file '{filename}'.")

   # Usage
   
   filename = "sample.txt"
   
   read_file(filename)

   
   This script:

   - Uses a with statement to ensure the file is properly closed after reading.
   
   - Opens the file in read mode ('r').

   - Reads the entire content of the file using read().

   - Prints the content to the console.
   
   - Includes error handling for common file-related exceptions.

   b) Writing a list of strings to a file:

   def write_to_file(filename, data):
    
    try:
        
        with open(filename, 'w') as file:
            
            for line in data:
                
                file.write(line + '\n')
        
        print(f"Successfully wrote to {filename}")
    
    except IOError:
        
        print(f"Error: There was an issue writing to the file '{filename}'.")

   # Usage

   filename = "output.txt"
   
   lines_to_write = [
      "This is the first line.",
      
      "Here's the second line.",
      
      "And this is the third line."
   
   ]

   write_to_file(filename, lines_to_write)


   This script:

   - Opens the file in write mode ('w'), which will create the file if it doesn't exist or overwrite it if it does.
   
   - Iterates through the list of strings, writing each one to the file followed by a newline character.
   
   - Uses a with statement to ensure the file is properly closed after writing.
   
   - Includes error handling for potential IO errors.

(geeksforgeeks, 2017)


References

BoTree Technologies. (2023). What are the Top 10 Python Use Cases and Applications in The Real World? Www.linkedin.com. https://www.linkedin.com/pulse/what-top-10-python-use-cases-applications-real-world

geeksforgeeks. (2017, April 3). Reading and Writing to text files in Python - GeeksforGeeks. GeeksforGeeks. https://www.geeksforgeeks.org/reading-writing-text-files-python/

geeksforgeeks. (2023). Introduction To PYTHON. GeeksforGeeks. https://www.geeksforgeeks.org/introduction-to-python/

Inc, T. (2021, August 23). Top 12 Python Use Cases & Applications with Examples | Python Trends 2023. Web and Mobile App Development Blog - Technology News & Updates | TAFF Inc - Techaffinity Consulting. https://www.taffinc.com/blog/top-python-use-cases-and-applications/

Python Software Foundation. (2024). What Is Python? Executive Summary. Python. https://www.python.org/doc/essays/blurb/

Satyam, K. (2020, August 22). Try, Except, else and Finally in Python. GeeksforGeeks. https://www.geeksforgeeks.org/try-except-else-and-finally-in-python/

Simplilearn. (2024). Learn A to Z About Python Functions. Simplilearn.com. https://www.simplilearn.com/tutorials/python-tutorial/python-functions

Singh, V. (2023a, March 10). Difference Between Module and Package in Python - Shiksha Online. Shiksha.com; Shiksha Online. https://www.shiksha.com/online-courses/articles/difference-between-module-and-package-in-python/#:~:text=In%20simple%20terms%2C%20a%20module

Singh, V. (2023b, August 29). Difference Between List and Dictionary in Python - Shiksha Online. Shiksha.com; Shiksha Online. https://www.shiksha.com/online-courses/articles/difference-between-list-and-dictionary-in-python/#:~:text=Lists%20and%20Dictionaries%20are%20different

Sphinx, & Furo. (2017). Installing packages using pip and virtual environments — Python Packaging User Guide. Python.org. https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/

W3Schools. (2019). Python Conditions. W3schools.com. https://www.w3schools.com/python/python_conditions.asp

W3schools. (2023). Python Data Types. Www.w3schools.com. https://www.w3schools.com/python/python_datatypes.asp


