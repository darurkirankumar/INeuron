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

Q9. What is the relationship between classes and modules?

Q10. How do you make instances and classes?

Q11. Where and how should be class attributes created?

Q12. Where and how are instance attributes created?

Q13. What does the term "self" in a Python class mean?

Q14. How does a Python class handle operator overloading?

Q15. When do you consider allowing operator overloading of your classes?

Q16. What is the most popular form of operator overloading?

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
