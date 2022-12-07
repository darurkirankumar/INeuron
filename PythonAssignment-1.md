## Python OOP Assignment
Q1. What is the purpose of Python's OOP?

	In Python, object-oriented Programming (OOPs) is a programming paradigm that uses objects and classes in programming. It aims to implement real-world entities like inheritance, polymorphisms, encapsulation, etc. in the programming. 
	The main concept of OOPs is to bind the data and the functions that work on that together as a single unit so that no other part of the code can access this data.

	The concept of OOP in Python focuses on creating reusable code. This concept is also known as DRY (Don't Repeat Yourself).

Q2. Where does an inheritance search look for an attribute?

	An inheritance search looks for an attribute first in the instance object, then in the class the instance was created from, then in all higher superclasses, progressing from left to right (by default). The search stops at the first place the attribute is found.

Q3. How do you distinguish between a class object and an instance object?

	Class variables are declared inside a class but outside of any function. Instance variables are declared inside the constructor which is the __init__method.
	Class variables affect the entire class. Thus, when a class variable is updated, all the instances are updated. This comes in very handy but we also need to careful. If used carelessly, undesired consequences may occur.
	Instance variables take unique values for each instance. We assign the values for them when creating the instance.

Q4. What makes the first argument in a class’s method function special?

	Self is the first argument to be passed in Constructor and Instance Method.
	self represents the instance of the class. By using the “self”  we can access the attributes and methods of the class in python. It binds the attributes with the given arguments.
	The reason you need to use self. is because Python does not use the @ syntax to refer to instance attributes.
	self is parameter in Instance Method and user can use another parameter name in place of it. But it is advisable to use self because it increases the readability of code, and it is also a good programming practice.

Q5. What is the purpose of the init method?

	The __init__ method is the Python equivalent of the C++ constructor in an object-oriented approach. The __init__ function is called every time an object is created from a class. The __init__ method lets the class initialize the object's attributes and serves no other purpose. It is only used within classes.

Q6. What is the process for creating a class instance?

	To create instances of a class, you call the class using class name and pass in whatever arguments its __init__ method accepts.

	Ex:
	def __init__(self, name, salary):
		  self.name = name
		  self.salary = salary
		  Employee.empCount += 1
	   
	   def displayCount(self):
		 print "Total Employee %d" % Employee.empCount

	   def displayEmployee(self):
		  print "Name : ", self.name,  ", Salary: ", self.salary
		
		#This would create first object of Employee class
		emp1 = Employee("Zara", 2000)

Q7. What is the process for creating a class?

	The class statement creates a new class definition. The name of the class immediately follows the keyword class followed by a colon as follows −

	class ClassName:
	   'Optional class documentation string'
	   class_suite
	   
	 Ex:
	 class Employee:
	   'Common base class for all employees'
	   empCount = 0

	   def __init__(self, name, salary):
		  self.name = name
		  self.salary = salary
		  Employee.empCount += 1
	   
	   def displayCount(self):
		 print "Total Employee %d" % Employee.empCount

	   def displayEmployee(self):
		  print "Name : ", self.name,  ", Salary: ", self.salary

Q8. How would you define the superclasses of a class?

The super() function is used to give access to methods and properties of a parent or sibling class.

The super() function returns an object that represents the parent class.

Q9. What is the relationship between classes and modules?

Classes in python are templates for creating objects. They contain variables and functions which define the class objects. At the same time, modules are python programs that can be imported into another python program. Importing a module enables the usage of the module’s functions and variables into another program.


Q10. How do you make instances and classes?

	A class can b created with the help of class keyword.
	Ex:
	class Person:
	  def __init__(self, name, age):
		self.name = name
		self.age = age
	To create instances of a class, you call the class using class name and pass in whatever arguments its __init__ method accepts.
	Ex:
	class Person:
	  def __init__(self, name, age):
		self.name = name
		self.age = age

	p1 = Person("John", 36)

	print(p1.name)
	print(p1.age)

Q11. Where and how should be class attributes created?

To define a class attribute, you place it outside of the __init__() method. For example, the following defines pi as a class attribute:
Ex:
class Circle:
    pi = 3.14159

    def __init__(self, radius):
        self.radius = radius


Q12. Where and how are instance attributes created?

Instance Attributes are unique to each object, (an instance is another name for an object). Here, any Dog object we create will be able to store its name and age. We can change either attribute of either dog, without affecting any other dog objects we’ve created.
class Dog:

    def __init__(self, name, age):
        self.name = name
        self.age = age
This __init__ is called the initializer. It is automatically called when we instantiate the class. It’s job is to make sure the class has any attributes it needs. It’s sometimes also used to make sure that the object is in a valid state when it’s instantiated, like making sure the user didn’t enter a negative age for the dog.

We have to include the self parameter so that our initializer has a reference to the new object being instantiated.

Q13. What does the term "self" in a Python class mean?

The self parameter is a reference to the current instance of the class, and is used to access variables that belongs to the class.

Q14. How does a Python class handle operator overloading?

The operator overloading in Python means provide extended meaning beyond their predefined operational meaning. Such as, we use the "+" operator for adding two integers as well as joining two strings or merging two lists. We can achieve this as the "+" operator is overloaded by the "int" class and "str" class. The user can notice that the same inbuilt operator or function is showing different behaviour for objects of different classes. This process is known as operator overloading.

Ex:
print (14 + 32)  
   
# Now, we will concatenate the two strings  
print ("Operator" + "Overloading")  

Q15. When do you consider allowing operator overloading of your classes?

Suppose the user has two objects which are the physical representation of a user-defined data type class. The user has to add two objects using the "+" operator, and it gives an error. This is because the compiler does not know how to add two objects. So, the user has to define the function for using the operator, and that process is known as "operator overloading". The user can overload all the existing operators by they cannot create any new operator. 

Q16. What is the most popular form of operator overloading?

The most popular form of operator overloading in python is using + operator to add two integers and to concatenate two strings.
Ex:
class example:  
    def __init__(self, X):  
        self.X = X  
   
    # adding two objects  
    def __add__(self, U):  
        return self.X + U.X  
object_1 = example( int( input( print ("Please enter the value: "))))  
object_2 = example( int( input( print ("Please enter the value: "))))  
print (": ", object_1 + object_2)  
object_3 = example(str( input( print ("Please enter the value: "))))  
object_4 = example(str( input( print ("Please enter the value: "))))  
print (": ", object_3 + object_4)   

Output:
Please enter the value: 23
Please enter the value: 21
:  44
Please enter the value: Operator
Please enter the value: Overloading
:  OperatorOverloading

Q17. What are the two most important concepts to grasp in order to comprehend Python OOP code?



Q18. Describe three applications for exception processing.

Q19. What happens if you don't do something extra to treat an exception?

Q20. What are your options for recovering from an exception in your script?

Q21. Describe two methods for triggering exceptions in your script.

Q22. Identify two methods for specifying actions to be executed at termination time, regardless of  
whether or not an exception exists.

Q23. What is the purpose of the try statement?

Q24. What are the two most popular try statement variations?

Q25. What is the purpose of the raise statement?

Q26. What does the assert statement do, and what other statement is it like?

Q27. What is the purpose of the with/as argument, and what other statement is it like?

Q28. What are *args, **kwargs?

Q29. How can I pass optional or keyword parameters from one function to another?

Q30. What are Lambda Functions?

Q31. Explain Inheritance in Python with an example?

Q32. Suppose class C inherits from classes A and B as class C(A,B).Classes A and B both have their own versions of method func(). If we call func() from an object of 
class C, which version gets invoked?

Q33. Which methods/functions do we use to determine the type of instance and inheritance?

Q34.Explain the use of the 'nonlocal' keyword in Python.

Q35. What is the global keyword?
