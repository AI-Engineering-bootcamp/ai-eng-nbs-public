# Object-oriented programming

<h3>Table of Contents<span class="tocSkip"></span></h3>
<div class="toc"><ul class="toc-item"><li><span><a href="#What-is-OOP---Object-Oriented-Programming?" data-toc-modified-id="What-is-OOP---Object-Oriented-Programming?-1"><span class="toc-item-num">1&nbsp;&nbsp;</span>What is OOP - Object Oriented Programming?</a></span><ul class="toc-item"><li><span><a href="#Fundamental-Principles" data-toc-modified-id="Fundamental-Principles-1.1"><span class="toc-item-num">1.1&nbsp;&nbsp;</span>Fundamental Principles</a></span></li></ul></li><li><span><a href="#Classes-and-instances" data-toc-modified-id="Classes-and-instances-2"><span class="toc-item-num">2&nbsp;&nbsp;</span>Classes and instances</a></span></li><li><span><a href="#functional-vs-OOP-(Object-oriented-programming)" data-toc-modified-id="functional-vs-OOP-(Object-oriented-programming)-3"><span class="toc-item-num">3&nbsp;&nbsp;</span>functional vs OOP (Object oriented programming)</a></span></li><li><span><a href="#---" data-toc-modified-id="----4"><span class="toc-item-num">4&nbsp;&nbsp;</span>  -</a></span></li><li><span><a href="#Definition-of-a-class" data-toc-modified-id="Definition-of-a-class-5"><span class="toc-item-num">5&nbsp;&nbsp;</span>Definition of a class</a></span><ul class="toc-item"><li><span><a href="#Self:" data-toc-modified-id="Self:-5.1"><span class="toc-item-num">5.1&nbsp;&nbsp;</span>Self:</a></span><ul class="toc-item"><li><span><a href="#Defining-a-function" data-toc-modified-id="Defining-a-function-5.1.1"><span class="toc-item-num">5.1.1&nbsp;&nbsp;</span>Defining a function</a></span></li><li><span><a href="#Calling-a-function" data-toc-modified-id="Calling-a-function-5.1.2"><span class="toc-item-num">5.1.2&nbsp;&nbsp;</span>Calling a function</a></span></li><li><span><a href="#Defining-a-class" data-toc-modified-id="Defining-a-class-5.1.3"><span class="toc-item-num">5.1.3&nbsp;&nbsp;</span>Defining a class</a></span></li><li><span><a href="#Instansiating-a-class" data-toc-modified-id="Instansiating-a-class-5.1.4"><span class="toc-item-num">5.1.4&nbsp;&nbsp;</span>Instansiating a class</a></span></li></ul></li><li><span><a href="#Exploring-a-class" data-toc-modified-id="Exploring-a-class-5.2"><span class="toc-item-num">5.2&nbsp;&nbsp;</span>Exploring a class</a></span></li><li><span><a href="#Instance-Attributes" data-toc-modified-id="Instance-Attributes-5.3"><span class="toc-item-num">5.3&nbsp;&nbsp;</span>Instance Attributes</a></span><ul class="toc-item"><li><span><a href="#Default-attributes" data-toc-modified-id="Default-attributes-5.3.1"><span class="toc-item-num">5.3.1&nbsp;&nbsp;</span>Default attributes</a></span></li></ul></li><li><span><a href="#Instance-Methods" data-toc-modified-id="Instance-Methods-5.4"><span class="toc-item-num">5.4&nbsp;&nbsp;</span>Instance Methods</a></span><ul class="toc-item"><li><span><a href="#Python-is-built-with-objects" data-toc-modified-id="Python-is-built-with-objects-5.4.1"><span class="toc-item-num">5.4.1&nbsp;&nbsp;</span>Python is built with objects</a></span></li></ul></li><li><span><a href="#Class-variables" data-toc-modified-id="Class-variables-5.5"><span class="toc-item-num">5.5&nbsp;&nbsp;</span>Class variables</a></span></li></ul></li><li><span><a href="#Before-continuing,-let's-take-a-breath-and-review-vocabulary" data-toc-modified-id="Before-continuing,-let's-take-a-breath-and-review-vocabulary-6"><span class="toc-item-num">6&nbsp;&nbsp;</span>Before continuing, let's take a breath and review vocabulary</a></span><ul class="toc-item"><li><ul class="toc-item"><li><span><a href="#Easy-exercise" data-toc-modified-id="Easy-exercise-6.0.1"><span class="toc-item-num">6.0.1&nbsp;&nbsp;</span>Easy exercise</a></span></li></ul></li></ul></li><li><span><a href="#Inheritance" data-toc-modified-id="Inheritance-7"><span class="toc-item-num">7&nbsp;&nbsp;</span>Inheritance</a></span><ul class="toc-item"><li><span><a href="#super()" data-toc-modified-id="super()-7.1"><span class="toc-item-num">7.1&nbsp;&nbsp;</span>super()</a></span></li></ul></li><li><span><a href="#Summary" data-toc-modified-id="Summary-8"><span class="toc-item-num">8&nbsp;&nbsp;</span>Summary</a></span></li><li><span><a href="#Furthermaterials" data-toc-modified-id="Furthermaterials-9"><span class="toc-item-num">9&nbsp;&nbsp;</span>Furthermaterials</a></span><ul class="toc-item"><li><span><a href="#Methods-ADVANCED-@classmethod@staticmethod" data-toc-modified-id="Methods-ADVANCED-@classmethod@staticmethod-9.1"><span class="toc-item-num">9.1&nbsp;&nbsp;</span>Methods <strong>ADVANCED</strong> @classmethod@staticmethod</a></span></li></ul></li></ul></div>

## What is OOP - Object Oriented Programming?

Object-oriented programming is a programming paradigm, a style and technique for software development that extends beyond mere code implementation. This paradigm is centered on the concept of "objects," which serve as self-contained units containing both data (referred to as "attributes") and code for manipulating that data (referred to as "methods").

The essence of OOP lies in encapsulating these attributes and methods within a unified data structure known as a "class." Think of classes as blueprints that define the structure and behavior of objects, much like a cookie cutter defines the shape of cookies.

When objects are instantiated from a class, they share a common structure and specific attributes, similar to cookies created from the same cookie cutter mold. However, just as each cookie can have its unique properties like color, texture, or flavor, objects can possess distinct attributes and behaviors.

In summary, OOP promotes modularity and code reusability by enabling developers to create and manipulate objects based on predefined classes. This approach has a profound impact on software engineering and forms the basis of various software development methodologies.

![clases](https://files.realpython.com/media/Object-Oriented-Programming-OOP-in-Python-3_Watermarked.0d29780806d5.jpg)

### Fundamental Principles


Object-Oriented Programming (OOP) is built on four fundamental principles that help structure and organize code in a more intuitive and modular way:

1. **Data Abstraction**: Human thinking naturally abstracts concrete information into broader concepts or classes. For example, when we think of a "car," we envision a vehicle with specific characteristics like four wheels, a steering wheel, and an engine. This ability to abstract concepts is crucial for language development and is mirrored in programming as well. In OOP, we refer to the abstract concept as a "class" and its concrete realizations as "objects" or "instances." Your specific car is an object, an instance of the broader "car" class.

2. **Encapsulation**:Each object in OOP contains its own data (attributes) and can be manipulated through specific actions (methods). For example, a car object might have attributes like tire pressure, color, and fuel level. These attributes are encapsulated within the object, meaning they are accessible and modifiable only through that object. This encapsulation ensures that data is self-contained, reducing the need for separate lists or variables to store related information.

3. **Inheritance**: Inheritance allows one class to specialize or derive from another. The specialized class inherits properties and behaviors from a more general class, known as the "superclass." For instance, "Car" and "Truck" classes can inherit from the "Vehicle" superclass. This approach promotes code reuse by inheriting common attributes and methods from a superior class. Python even supports "multiple inheritance," enabling a class to inherit from multiple parent classes simultaneously.

4. **Polymorphism**:Polymorphism allows objects of different classes to be treated as objects of a common superclass. This is achieved by defining methods in the superclass and allowing subclasses to override those methods with their own implementations. For example, both "Square" and "Circle" classes may be subclasses of "Shape," and all of them implement a common method like "draw()." When you call this method on an object, the specific subclass's implementation is executed. This flexibility allows functions to accept objects of the superclass as parameters, not needing to know the exact subclass, promoting code reusability and adaptability.

These four principles collectively form the foundation of OOP, enabling more organized, modular, and flexible code development.


## Classes and instances

In Python, a **class** serves as a blueprint or template for creating objects, and each object created from a class is called an **instance**. A class defines both the structure (attributes) and behavior (methods) of objects that belong to it.

- **Class Definition**: Here's a basic example of defining a class in Python:


```python
class Car:
    def __init__(self, color):
        self.color = color
        self.position = 0  # Initialize position as an attribute
    
    def move(self):
        self.position += 1  # Increment the position attribute by 1
        return self.position  # Return the updated position
```

In this example:

- We define a class named `Car`, which serves as the blueprint for creating car objects (instances).
- The `__init__` method is a special method called a constructor. It initializes the attributes of the object when it's created. In this case, we set the `color` attribute of the car and the `position` to 0.
- The `move` method is a simple function defined within the class. It simulates the car's movement and returns a new position.

**Creating Instances**, once we've defined the class, we can create instances of that class, each representing a unique car:


```python
bmw = Car("red")
```

After creating an instance, we can access its attributes and methods using dot notation:


```python
position = bmw.move()  # Call the move() method
car_color = bmw.color  # Access the color attribute
```

In this line of code, we create an instance of the `Car` class named `bmw` and specify its color as "red."

In this example, we call the `move()` method to simulate the car's movement and store its position. We also access the color attribute to retrieve the car's `color`.

Classes and instances provide a powerful way to model real-world objects and their behaviors in Python, promoting code reusability and organization.

## Recap

1. Imperative Programming:
    - **Imperative programming** is a paradigm that focuses on describing how a program operates step by step.
    - It emphasizes changing program state through a series of statements or commands.
    - Key characteristics include variables, loops, conditionals, and explicit state changes.
    - Programs written in this paradigm are often easy to understand sequentially but can become complex with increasing size and complexity.


2. Functional Programming:
    - **Functional programming** is a paradigm that treats computation as the evaluation of mathematical functions and avoids changing state and mutable data.
    - It emphasizes immutability, pure functions, and declarative expressions.
    - Key characteristics include higher-order functions, first-class functions, and the absence of side effects.
    - Functional programs are often concise, maintainable, and easier to reason about.


3. Object-Oriented Programming (OOP):
    - **Object-Oriented Programming (OOP)** is a paradigm based on the concept of "objects," which combine data (attributes) and behavior (methods) into a single unit.
    - It emphasizes modeling real-world entities and their interactions in code.
    - Key characteristics include classes, objects, inheritance, encapsulation, and polymorphism.
    - OOP promotes modularity, reusability, and abstraction.


## Functional vs. OOP:

1. **State Management**:
    - Functional programming typically avoids mutable state and encourages immutability, making it easier to reason about code. In contrast, OOP often involves changing object states.


2. **Data Structures**:
    - Functional programming relies on built-in data structures and functions, while OOP defines custom classes to represent data and behavior.


3. **Abstraction**:
    - OOP focuses on modeling real-world objects with classes, promoting a natural abstraction. Functional programming abstracts through functions and transformations.


4. **Inheritance**:
    - OOP uses inheritance to define relationships between classes. Functional programming relies on composition and higher-order functions.


5. **Side Effects**:
    - Functional programming discourages side effects and promotes pure functions. OOP may involve side effects through method calls and state changes.


6. **Modularity**:
    - Both paradigms support modularity but achieve it differently. OOP uses classes and objects, while functional programming relies on function composition.


7. **Complexity**:
    - Functional programming often results in more concise and less complex code due to immutability and purity. OOP code can become complex with deep inheritance hierarchies.


In summary, functional programming and OOP are distinct paradigms with different philosophies and trade-offs. Functional programming prioritizes immutability, pure functions, and declarative expressions, while OOP focuses on modeling real-world entities using classes and objects. The choice between them depends on the problem domain and design goals of a software project.

## A Specific Example of a Class in Python

In object-oriented programming (OOP), a **class** is like a blueprint or template for creating objects. An **instance** is a specific object created from a class. To understand instances better, let's take the example of the built-in `str` class.

### The `str` Class:

- In Python, `str` is a built-in class that represents strings (sequences of characters).
- The `str` class defines various methods and attributes that can be used with string objects.


```python
# Example 1: Creating Instances
name = "Alfons"  # Creating an instance of the str class
text = "sdsfdsxg"  # Another instance of the str class
```

### Instances of `str`:

- When you create a string, like `name = "Alfons"` or `text = "sdsfdsxg"`, you are creating instances of the `str` class.
- Each instance of `str` (e.g., "Alfons" or "sdsfdsxg") is a specific object with its own data (the characters in the string) and behavior (methods for string manipulation).

### Exploring Methods and Attributes:

- To explore the methods and attributes of a class (including built-in classes like `str`), you can use the `dir()` function.
- You can call `dir()` on either an object or the class itself to see what methods and attributes are available.


```python
# Example 2: Exploring Methods and Attributes
# Using the dir() function to see available methods and attributes
print("Methods and attributes of the str class:")
print(dir(str))
```

    Methods and attributes of the str class:
    ['__add__', '__class__', '__contains__', '__delattr__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getitem__', '__getnewargs__', '__gt__', '__hash__', '__init__', '__init_subclass__', '__iter__', '__le__', '__len__', '__lt__', '__mod__', '__mul__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__rmod__', '__rmul__', '__setattr__', '__sizeof__', '__str__', '__subclasshook__', 'capitalize', 'casefold', 'center', 'count', 'encode', 'endswith', 'expandtabs', 'find', 'format', 'format_map', 'index', 'isalnum', 'isalpha', 'isascii', 'isdecimal', 'isdigit', 'isidentifier', 'islower', 'isnumeric', 'isprintable', 'isspace', 'istitle', 'isupper', 'join', 'ljust', 'lower', 'lstrip', 'maketrans', 'partition', 'removeprefix', 'removesuffix', 'replace', 'rfind', 'rindex', 'rjust', 'rpartition', 'rsplit', 'rstrip', 'split', 'splitlines', 'startswith', 'strip', 'swapcase', 'title', 'translate', 'upper', 'zfill']


### Dunder (Magic) Methods:

- In Python, methods and attributes with names enclosed in double underscores, such as `.__str__()` or `.__len__()`, are often called **dunder methods** or **magic methods**.
- Dunder methods are meant for Python's internal use and are invoked automatically in certain situations.
- For example, when you use the `str()` function to convert an object to a string, Python internally calls the `.__str__()` dunder method if it's defined for that object.
- Dunder methods provide a way to customize the behavior of your classes when they interact with built-in Python functions and operators.

Overall, instances are specific objects created from classes, and you can explore their available methods and attributes using `dir()`. Dunder methods are special methods in Python, recognized by their double underscores, and they allow you to customize the behavior of your classes in various situations.


```python
# Example 3: Dunder Methods
# Defining a custom class with dunder methods
class CustomString:
    def __init__(self, value):
        self.value = value

    def __str__(self):
        return f"CustomString({self.value})"

    def __len__(self):
        return len(self.value)
```


```python
# Creating instances of the custom class
custom_text = CustomString("Hello, World!")
```


```python
# Using the str() function to convert an object to a string
# It internally calls the __str__() dunder method if defined
print(str(custom_text))  # Output: "CustomString(Hello, World!)"

# Using the len() function to get the length of an object
# It internally calls the __len__() dunder method if defined
print(len(custom_text))  # Output: 13
```

## Definition of a class

In Python, we can define our own classes to model real-world entities or abstract concepts. A class is like a blueprint that defines the attributes (data) and methods (functions) that objects of that class will have. Once a class is defined, we can create instances (objects) of that class, each with its own set of attributes and the ability to perform actions defined by the class's methods.

To create a class, we use the `class` keyword and define the attributes and methods within the class block. Attributes are variables that store data for each instance, and methods are functions that allow instances to perform actions or operations.

Let's explore class definition and instantiation with an example involving a `Teacher` class to represent educators in a school management system.



```python
# Definition of a class - Teacher
class Teacher:
    # Constructor method (__init__) to initialize attributes
    def __init__(self, name, subject):
        self.name = name
        self.subject = subject
        self.courses_taught = []

    # Method to add a course taught by the teacher
    def add_course(self, course_name):
        self.courses_taught.append(course_name)

    # Method to display teacher's information
    def display_info(self):
        print(f"Teacher Name: {self.name}")
        print(f"Teaching Subject: {self.subject}")
        print(f"Courses Taught: {', '.join(self.courses_taught)}")
```


```python
# Creating instances of the Teacher class
teacher1 = Teacher("Alice", "Math")
teacher2 = Teacher("Bob", "Science")
```


```python
# Adding courses taught by the teachers
teacher1.add_course("Algebra")
teacher2.add_course("Biology")
teacher2.add_course("Chemistry")
```


```python
# Displaying teacher information
teacher1.display_info()
teacher2.display_info()
```

### Self: 

In Python classes, the `self` keyword plays a crucial role. It refers to the instance of the class itself and is used to access its attributes and methods. While it might seem like an extra requirement compared to some other programming languages, understanding and using `self` correctly is fundamental to writing effective and maintainable object-oriented Python code.

The use of `self` is a Python convention and helps in distinguishing between instance variables (belonging to the object) and local variables (used only within a method). By using `self`, you make it clear that you are working with instance variables and methods.

To maintain consistency and adhere to Python's naming conventions, you can refer to resources like the Python PEP 8, [here](https://realpython.com/python-pep8/#naming-styles), style guide, which provides guidelines for naming variables, classes, functions, and more. Following these conventions can improve code readability and make your code more accessible to other Python developers.

Let's dive into the role of `self` and how it's used within Python classes.


```python
class Dog:
    def __init__(self, name, breed):
        self.name = name
        self.breed = breed

    def bark(self):
        return f"{self.name} is barking!"
```


```python
# Creating instances of the Dog class
dog1 = Dog("Buddy", "Golden Retriever")
dog2 = Dog("Max", "Labrador")
```


```python
# Accessing instance variables using self
print(dog1.name)  # Output: Buddy
print(dog2.breed)  # Output: Labrador
```


```python
# Calling a method using self
print(dog1.bark())  # Output: Buddy is barking!
print(dog2.bark())  # Output: Max is barking!
```

In this example:

- We define a `Dog` class with an `__init__` method that takes two parameters, `name` and `breed`, and initializes instance variables `self.name` and `self.breed`.

- The `bark` method uses `self` to access the `name` attribute of the instance to generate a bark message.

- We create two instances of the `Dog` class, `dog1` and `dog2`, and initialize them with different names and breeds.

- We access instance variables (`name` and `breed`) and call the `bark` method on each instance using `self`.

#### Default attributes

In Python classes, you can initialize attributes with default values. This means that if no specific value is provided when creating instances, the attributes will have these default values. This feature allows you to set sensible defaults, which can be overridden if needed.

Let's illustrate this with an example:


```python
class Dog:
    def __init__(self, name="Unknown", breed="Unknown"):
        self.name = name
        self.breed = breed

    def bark(self):
        return f"{self.name} says Woof!"
```


```python
# Creating instances with and without attribute values
dog1 = Dog("Buddy", "Golden Retriever")
dog2 = Dog()  # Using default attribute values
```


```python
print(dog1.bark())  # Output: "Buddy says Woof!"
print(dog2.bark())  # Output: "Unknown says Woof!"
```




    'laura.molas@ironhack.com'



In the `Dog` class, we provide default values for `name` and `breed` in the `__init__` method. When creating instances like `dog2`, if no values are specified, the default values are used. This flexibility makes it convenient to handle various scenarios when creating objects.

### Instance Methods

In Python, instance methods are functions associated with a class that can be called on instances (objects) created from that class. These methods can access and manipulate the attributes of an instance, making them a powerful tool for performing actions related to the class's data.

Let's explore the concept of instance methods with an example involving a `Staff` class, which represents staff members at a fictional company. We'll define attributes such as `name`, `fname`, `email`, and `time_off`, and create methods like `greetings` and `takes_days_off` to demonstrate how instance methods work within a class.


```python
class Staff ():
    
    # 1. Atributes
    def __init__ (self, name, fname):
        self.name = name
        self.fname = fname
    
        self.email = (self.name + "." + self.fname + "@ironhack.com").lower()
        
        self.time_off = 30
        
    # 2. Methods
    
    def greetings (self):
        return f"Hello!!!!!!"
    
    def takes_days_off (self, n):
        self.time_off -= n
```


```python
# Let's create the first employee
Employee_1 = Staff("Alfons", "Marques")
```


```python
# Let's access the attribute time_off
Employee_1.time_off
```


```python
# I took one day off
Employee_1.takes_days_off(1)
```


```python
# How many do I have now?
Employee_1.time_off
```


```python
# Let's do something
Employee_1.greetings()
```

**Instance methods, are functions within the classes that can save us a lot of time

**⚠️ Target Variables When Instantiating, Ignoring Defaults**

In Python, when we instantiate (create) objects from a class, we often provide values for attributes to customize each instance. However, there may be cases where we want to use the default values defined in the class's `__init__` method for certain attributes.

In the example provided, we have a `Staff` class representing staff members at a company. This class has attributes like `name`, `fname`, `email`, and `time_off`. We've also defined two instance methods: `greetings` for a friendly greeting and `takes_days_off` for managing time-off requests.

Pay attention to how we can target specific variables when instantiating `Staff` objects while ignoring the defaults for some attributes, such as the number of days off. This flexibility allows us to customize objects as needed while relying on default values when appropriate.



```python
class Staff ():
    
    # 1. Atributes
    def __init__ (self, name, fname):
        self.name = name
        self.fname = fname
    
        self.email = (self.name + "." + self.fname + "@ironhack.com").lower()
        
        self.time_off = 30
        
    # 2. Methods
    
    def greetings (self):
        return f"Hello!!!!!!"
    
    def takes_days_off (self, days=1):
        """Default: take one day unless passed oterhwise"""
        if days <= self.time_off:
            self.time_off -= days
            return f"You have these many days left: {self.time_off}"
        else: 
            return f"You only have {self.time_off} days available" 
```

**Watch Out** 👀

When modifying a class by adding new attributes or methods, it's important to be aware that existing objects created from that class won't automatically have the new attributes or methods. You'll need to recreate those objects to ensure they are initialized with the updates.

In the example provided, we have a `Staff` class representing staff members at a company. Initially, the class has attributes like `name`, `fname`, `email`, `time_off`, and `hobbies`. We've also defined methods like `greetings`, `takes_days_off`, and `hobbies_function`.

Take note of this important point, especially when you make changes to a class's structure. If you add new attributes or methods, any existing objects of that class will not automatically gain access to these changes. Recreating the objects is necessary to incorporate the updates effectively.


```python
class Staff ():
    
    # 1. Atributes
    def __init__ (self, name, fname):
        self.name = name
        self.fname = fname
    
        self.email = (self.name + "." + self.fname + "@ironhack.com").lower()
        
        self.time_off = 30
        
        self.hobbies = []
        
        
    # 2. Methods
    
    def greetings (self):
        return f"Hello!!!!!!"
    
    def takes_days_off (self, days=1):
        """Default: take one day unless passed oterhwise"""
        if days <= self.time_off:
            self.time_off -= days
            return f"You have these many days left: {self.time_off}"
        else: 
            return f"You only have {self.time_off} days available"
    
    def hobbies_function(self, hobbie):
        # adds elements to hobbies
            # 1. what should this receive: hobbie
            # 2. what should it do
            # 3. return?
        
        self.hobbies.append(hobbie)
        return f"My hobbies are {self.hobbies}"
```


```python
# Play with this class a litle bit
```

### Class Variables

In object-oriented programming, class variables are attributes shared by all instances (objects) of a class. Unlike instance variables, which are unique to each object, class variables maintain the same value across all instances of the class.

Class variables are typically defined within the class but outside of any instance methods. They are associated with the class itself, rather than with specific instances of the class. This means that any changes made to a class variable affect all objects created from that class.

Class variables are useful for storing data or properties that are common to all instances of a class, such as configuration settings, default values, or constants. They can also be accessed and modified through the class itself, making them a powerful tool for managing shared data within a class.

In Python, class variables are often denoted using a naming convention with uppercase letters to distinguish them from instance variables, which usually have lowercase names. Understanding the use of class variables is essential when designing and working with classes in object-oriented programming.


```python
class Employee:
    # Class variable
    COMPANY = "XYZ Corporation"
    
    def __init__(self, name, emp_id):
        # Instance variables
        self.name = name
        self.emp_id = emp_id
    
    def get_employee_info(self):
        return f"Name: {self.name}, Employee ID: {self.emp_id}, Company: {Employee.company}"
```


```python
# Create instances of the Employee class
employee1 = Employee("John Doe", 1001)
employee2 = Employee("Alice Smith", 1002)
```


```python
# Access and display the class variable
print("Company:", Employee.company)
```


```python
# Access and display instance-specific information
print(employee1.get_employee_info())
print(employee2.get_employee_info())
```

In general, class attributes should not be used, except to store constant values.

**Exercise: Creating a Class for Student Records**

In this exercise, we'll explore how to use classes in a data analytics context. Imagine you work at a university's data analytics department, and you're tasked with managing and analyzing student records. To streamline your work and improve data organization, you decide to create a Python class called `Student` to represent individual student records.

The `Student` class will encapsulate student attributes such as name, ID, courses, and grades. Additionally, it will provide methods to calculate the student's GPA, add courses, and display the student's information.

By creating this class, you'll demonstrate how classes can help you organize and analyze student data efficiently. This exercise is beginner-friendly and aims to illustrate the practical use of classes in a data analytics context.

Now, let's dive into the Python code to create the `Student` class and perform various operations on student records.


```python
# Define the Student class
class Student:
    def __init__(self, name, student_id):
        self.name = name
        self.student_id = student_id
        self.courses = {}
    
    def add_course(self, course_name, grade):
        self.courses[course_name] = grade
    
    def calculate_gpa(self):
        total_grade_points = sum(self.courses.values())
        num_courses = len(self.courses)
        if num_courses == 0:
            return 0.0
        else:
            return total_grade_points / num_courses
    
    def display_student_info(self):
        print(f"Student Name: {self.name}")
        print(f"Student ID: {self.student_id}")
        print("Courses and Grades:")
        for course, grade in self.courses.items():
            print(f"{course}: {grade}")
        print(f"Overall GPA: {self.calculate_gpa():.2f}")
```


```python
# Clean code example:
class Student:
    def __init__(self, name: str, student_id: str):
        """
        Initialize a Student object with name and student ID.

        Args:
            name (str): The student's name.
            student_id (str): The student's unique identifier.
        """
        self.name = name
        self.student_id = student_id
        self.courses = {}

    def add_course(self, course_name: str, grade: float):
        """
        Add a course and its grade to the student's record.

        Args:
            course_name (str): The name of the course.
            grade (float): The grade received in the course.
        """
        self.courses[course_name] = grade

    def calculate_gpa(self) -> float:
        """
        Calculate the student's GPA based on course grades.

        Returns:
            float: The calculated GPA.
        """
        total_grade_points = sum(self.courses.values())
        num_courses = len(self.courses)
        if num_courses == 0:
            return 0.0
        else:
            return total_grade_points / num_courses

    def display_student_info(self):
        """
        Display information about the student, including name, ID, courses, and GPA.
        """
        print(f"Student Name: {self.name}")
        print(f"Student ID: {self.student_id}")
        print("Courses and Grades:")
        for course, grade in self.courses.items():
            print(f"{course}: {grade}")
        print(f"Overall GPA: {self.calculate_gpa():.2f}")
```


```python
# Create instances of the Student class
student1 = Student("Alice Smith", "S12345")
student2 = Student("Bob Johnson", "S67890")
```


```python
# Add courses and grades for each student
student1.add_course("Math", 90)
student1.add_course("History", 85)
student2.add_course("Science", 92)
student2.add_course("English", 88)
```


```python
# Display student information
student1.display_student_info()
student2.display_student_info()
```

## Before continuing, let's take a breath and review vocabulary

- **Class**: Think of a class as a blueprint or a cookie mold. It defines the structure and behavior of objects. When you create a class, you're specifying how objects of that class should look and behave.

- **Object** or **Instance**: An object is a concrete, individual realization of a class, much like a freshly baked cookie from a mold. Each object created from a class shares the same structure defined by the class but can have different data and attributes.

- **Attribute**: Attributes are like the ingredients that give each object its unique characteristics. In Python, attributes are defined as arguments in the `__init__` function (the constructor) and are stored as data within each object. Think of them as variables that hold specific information for each object.

    - **Object/Instance Attribute**: These attributes are specific to each individual object. For example, in a `Student` class, the student's name and ID are instance attributes because they vary from one student object to another.

    - **Class Attribute**: Class attributes are shared among all objects created from the same class. They are constants or values that remain consistent for all instances. For instance, if you have a `School` class, the school's name can be a class attribute because it's the same for all students in that school.

- **Method**: Methods are like the actions or functions that objects can perform. They define the behavior of objects. Methods are essentially functions that operate on object data or attributes. For example, a `Student` class might have a `calculate_gpa` method that calculates the student's GPA based on their grades.

Understanding these concepts helps us structure and organize our code effectively, making it easier to create, manage, and manipulate objects in an object-oriented programming paradigm.


## Business challenge: Managing Sales Data with Python Classes

In this exercise, we'll explore how Python classes can be used to manage and analyze sales data. Imagine you work for a small retail company, and your task is to organize and analyze sales information for various products. To achieve this, we'll create a Python class called `Product` to represent individual products and another class called `SalesData` to manage sales data efficiently.

### Part 1: Create the Product Class

1. Define a class called `Product` with the following attributes and methods:
   - Attributes:
     - `name` (str): The name of the product.
     - `price` (float): The price of the product.
     - `quantity_sold` (int): The quantity of the product sold.
   - Methods:
     - `__init__(self, name, price)`: The constructor method that initializes the `name`, `price`, and sets `quantity_sold` to 0.
     - `sell(self, quantity)`: A method that increments the `quantity_sold` attribute by the given quantity when a product is sold.
     - `get_revenue(self)`: A method that calculates and returns the total revenue generated by selling this product (price * quantity_sold).

### Part 2: Create the SalesData Class

2. Define a class called `SalesData` with the following attributes and methods:
   - Attributes:
     - `products` (list): A list to store instances of the `Product` class.
   - Methods:
     - `__init__(self)`: The constructor method that initializes an empty list to store products.
     - `add_product(self, product)`: A method that adds a `Product` object to the list of products.
     - `get_total_revenue(self)`: A method that calculates and returns the total revenue generated from selling all products.
     - `get_best_selling_product(self)`: A method that identifies and returns the product with the highest quantity sold.

### Part 3: Using the Classes

3. Create instances of the `Product` class to represent different products in your inventory.

4. Create an instance of the `SalesData` class to manage your sales data.

5. Add the created product instances to the `SalesData` instance.

6. Simulate sales for each product using the `sell` method of the `Product` class.

7. Calculate the total revenue using the `get_total_revenue` method of the `SalesData` class.

8. Identify the best-selling product using the `get_best_selling_product` method of the `SalesData` class.

### Additional Challenges (Optional, only if you have time):

9. Implement error handling in your classes to ensure that negative quantities or incorrect input are handled gracefully.

10. Create a method to display the product details, including name, price, quantity sold, and revenue, for all products in the `SalesData` class.

This exercise will help you understand how classes can be used to organize and analyze sales data effectively, making it easier to manage and extract valuable insights from your data. It demonstrates the practical application of classes in a data analytics context.



```python
# Part 1: Create the Product Class
class Product:
    def __init__(self, name, price):
        self.name = name
        self.price = price
        self.quantity_sold = 0
        #[your code here...]

# Part 2: Create the SalesData Class
class SalesData:
    def __init__(self):
        self.products = []
        #[your code here...]
    

# Part 3: Using the Classes
# Create instances of the Product class
product1 = Product("Laptop", 800.0)
product2 = Product("Phone", 500.0)

#[your code here...]
```

## Inheritance

Inheritance is a fundamental concept in object-oriented programming that allows you to define new classes based on existing ones. In this relationship, the existing class is referred to as the "parent class," "superclass," or "parent," while the new class is known as the "child class" or "subclass."

The key idea behind inheritance is that a child class inherits all the properties (attributes and methods) of its parent class. This inheritance mechanism provides several advantages, with code reusability being one of the most significant benefits.

By inheriting from a parent class, a child class can reuse the attributes and methods defined in the parent class, saving developers from rewriting the same code. This promotes a more efficient and organized approach to software development, as changes or updates can be made in one place (the parent class) and automatically applied to all child classes.

In addition to inheriting attributes and methods, child classes have the flexibility to override or extend these inherited elements. This means that child classes can provide their own implementations of methods (method overriding) or introduce new attributes and methods specific to their requirements.

In summary, inheritance is a powerful concept that fosters code reusability, maintainability, and flexibility in object-oriented programming, allowing developers to build upon existing classes to create new ones with shared functionalities.



![miniyoda](https://media.giphy.com/media/j0eRJzyW7XjMpu1Pqd/giphy.gif)

- **Method Defined in the Parent Class**

When a method is defined in the parent class but not in the child class, the child class inherits the method without any need for modification. This means that the method in the child class will work exactly the same way as it does in the parent class, and there is no requirement to override it.

- **Method Defined Only in Child Class**

In some cases, a method may be defined exclusively in the child class and not in the parent class. In this scenario, the method belongs solely to the child class, and there is no inheritance in the opposite direction. This approach allows the child class to have its unique behavior and functionality.

- **Method Defined in Both Parent and Child Classes**

When a method is defined in both the parent and child classes, the child class's implementation takes precedence. This means that the method defined in the child class will override the parent class's method. However, there is a way to utilize the original method defined in the parent class while extending it in the child class.

To achieve this, Python provides the `super()` function, which allows you to call any method of the parent class from the child class. By invoking `super()`, you can access the parent class's method and add extra functionality or behavior to it in the child class. It's essential to ensure that you provide all the necessary attributes and parameters when calling the parent class's method via `super()`.

**Example 1**:


```python
# Parent class
class Shape:
    def __init__(self, name):
        self.name = name
    
    def get_name(self):
        return f"We are working with a {self.name}."
```


```python
# Child class
class Circle(Shape):
    def __init__(self, name, radius):
        super().__init__(name)
        self.radius = radius
    
    def area(self):
        return 3.14 * self.radius**2
```


```python
# Child class
class Rectangle(Shape):
    def __init__(self, name, length, width):
        super().__init__(name)
        self.length = length
        self.width = width
    
    def area(self):
        return self.length * self.width
```


```python
# Creating instances
circle = Circle("Circle", 5)
rectangle = Rectangle("Rectangle", 4, 6)
```


```python
# Calling methods
print(circle.area())       # Uses child class's area method
print(circle.get_name())   # Uses parent class's get_name method
print(rectangle.area())    # Uses child class's area method
print(rectangle.get_name())# Uses parent class's get_name method
```

**Example 2:**


```python
# Parent class
class Animal:
    def __init__(self, name):
        self.name = name
    
    def speak(self):
        return f"{self.name} makes a sound"        
```


```python
# Child class
class Dog(Animal):
    def __init__(self, name, breed):
        super().__init__(name) #taking the things from PARENT class
        self.breed = breed
    
    def speak(self):
        return f"{self.name} the {self.breed} barks loudly"
    
    def fetch(self):
        return f"{self.name} fetches the ball"
```


```python
# Child class
class Cat(Animal):
    def __init__(self, name, color):
        super().__init__(name) #taking the things from PARENT class
        self.color = color
    
    def speak(self):
        return f"{self.name} the {self.color} cat meows softly"
    
    def chase_mice(self):
        return f"{self.name} the {self.color} cat is chasing a mouse"
```


```python
# Creating instances
dog = Dog("Buddy", "Golden Retriever")
cat = Cat("Whiskers", "Gray")
```


```python
# Calling methods
print(dog.speak())         # Overrides parent's speak method
print(dog.fetch())         # Additional method in the child class
print(cat.speak())         # Overrides parent's speak method
print(cat.chase_mice())    # Additional method in the child class
```

In this example:

- We have a parent class `Animal` with an `__init__` method to initialize the `name` attribute and a `speak` method that returns a generic sound.

- We create two child classes, `Dog` and `Cat`, which inherit from the `Animal` parent class.

- Both child classes have their `__init__` methods that call the parent class's `__init__` method using `super()`. They also have their `speak` methods, which override the parent class's `speak` method to provide species-specific sounds. Additionally, each child class has its own unique method (`fetch` for `Dog` and `chase_mice` for `Cat`).

- We create instances of the `Dog` and `Cat` classes and call their methods. When we call the `speak` method on each instance, it uses the overridden method specific to that class. The additional methods (`fetch` and `chase_mice`) are also available for the respective instances.


## Summary

# Object-Oriented Programming (OOP) Simplified

- OOP is a "fascinating" programming paradigm alongside imperative and functional styles.
- In OOP, everything is an object, combining data (attributes) and behavior (methods).
- Follow naming conventions: `class Object()`, `def a_function()`, `CONSTANTS = PI`, `variables`, `one_variable`.
  
## Instances: Bringing Objects to Life

- Instances are concrete examples of a class, like Laura and Albert being instances of the Staff class.
- The class provides the blueprint, and instances embody it.
- To create instances, use `def __init__(self):` and specify what it needs when instantiating.
  
## The Power of 'self'

- `self` is the object referring to itself, enabling access to its attributes and methods.
- For example: `"sdsdsdsd".upper()`, `self.time_off`, `self.email`, where `self` represents the object itself.
  
## Methods: The Doers in OOP

- All methods take `self` as the first argument, which means they operate on the instance itself.
- Methods can also accept other arguments beyond `self`, allowing for additional functionality.
  
## Flexible Attributes

- Attributes can be passed when instantiating an object or have default values.
- For instance, an email address or holiday days can be set as default attributes.
  
## Class Inheritance: Building on Foundations

- Inheritance lets you create specialized classes from existing ones.
- For instance: `class Staff()`, `class Marketing(Staff)`, `class PaidSocialMedia(Marketing)`.
  
## Instances Receive Values

- Instances can receive values, including attributes from other objects.
- Just like Mario can acquire the power of a mushroom, objects can exchange data.
- For example, a gym can record the membership amount from a new customer.

In this simplified guide, we've explored key OOP concepts, demystifying this powerful programming paradigm. OOP brings structure and organization to code, making it easier to design, understand, and maintain. 


## Further materials

- Youtube Tutorial by [Corey Schafer](https://www.youtube.com/watch?v=ZDa-Z5JzLYM)
- [Real Python](https://docs.hektorprofe.net/python/object-oriented-programming/classes-and-objects/)
- [Interesting read](https://medium.com/@shaistha24/functional-programming-vs-object-oriented-programming-oop-which-is-better-82172e53a526) --> OOP vs Functional programming

### Methods **ADVANCED** @classmethod@staticmethod
* [Real Python - @classmethod/@stathicmethod](https://realpython.com/instance-class-and-static-methods-demystified/). Advanced Python with decorators (we'll mention them later)

## Solutions


```python
# Part 1: Create the Product Class
class Product:
    def __init__(self, name, price):
        self.name = name
        self.price = price
        self.quantity_sold = 0
    
    def sell(self, quantity):
        if quantity > 0:
            self.quantity_sold += quantity
        else:
            print("Invalid quantity. Please enter a positive number.")
    
    def get_revenue(self):
        return self.price * self.quantity_sold

# Part 2: Create the SalesData Class
class SalesData:
    def __init__(self):
        self.products = []
    
    def add_product(self, product):
        self.products.append(product)
    
    def get_total_revenue(self):
        total_revenue = 0
        for product in self.products:
            total_revenue += product.get_revenue()
        return total_revenue
    
    def get_best_selling_product(self):
        if not self.products:
            return None
        
        best_product = self.products[0]
        for product in self.products:
            if product.quantity_sold > best_product.quantity_sold:
                best_product = product
        return best_product

# Part 3: Using the Classes
# Create instances of the Product class
product1 = Product("Laptop", 800.0)
product2 = Product("Phone", 500.0)

# Create an instance of the SalesData class
sales_data = SalesData()

# Add the created product instances to the SalesData instance
sales_data.add_product(product1)
sales_data.add_product(product2)

# Simulate sales for each product
product1.sell(5)
product2.sell(8)

# Calculate the total revenue
total_revenue = sales_data.get_total_revenue()
print(f"Total Revenue: ${total_revenue:.2f}")

# Identify the best-selling product
best_selling_product = sales_data.get_best_selling_product()
if best_selling_product:
    print(f"Best Selling Product: {best_selling_product.name}")
else:
    print("No products in sales data.")
```
