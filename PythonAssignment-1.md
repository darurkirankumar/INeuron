## Assignment Part-1
Q1. Why do we call Python as a general purpose and high-level programming language?

	Python is a general-purpose language, meaning it can be used to create a variety of different programs and isn't specialized for any specific problems.
	It is not written in machine readable language. Python program needs to be processed before a machines can run them as it is an Interpreted language. It means every time a program runs, the interpreter has to translate the python code to machine readable byte-code.

Q2. Why is Python called a dynamically typed language?

	Dynamic typing means that the type of the variable is determined at run time. Even if we don't specify the type of the variable, python determines the type at the run time bases on the value of variable at that time.
	Because of dynamic typing, the same variable can have different types at diffrent times during execution.
	Dynamic typing typing aloows flexibility in programming but at cost of performance.

Q3. List some pros and cons of Python programming language?

	Advantages:
		1. Easy to learn - It is a high-level programming language, and its syntax is like the English language. These reasons make the language easy to learn and adapt to. Compared to Java and C, in Python, the same task can be performed using fewer lines of code. 
		2. Increased Productivity - As Python is simple in nature it helps the developers to concentrate, understand the syntax and behavior of the programming language easily, so that the users do not have to spend hours, so more work is done.
		3. Flexibility - Python does not restrict the user from trying something different. Other programming languages do not provide this type of flexibility and freedom, and hence Python is more preferred when comes to flexibility.
		4. Extensive Library - Python provides the user with a vast library. Python’s standard library is massive, and just about every function one needs to perform is available in its library. This is because it has a hugely supportive community and corporate sponsorship. External libraries 		are not used by users while working with Python.
		5. Supportive community - There are enough guides, tutorials, and documentation available on the Python programming language, which helps the developers to understand the language faster and better.

	Disadvantages:
		1. Performance - When compared to Java or C, the rate of execution Python is slower. As it is an interpreted language that is dynamically typed, each line of written code has to be interpreted befor processing. This is time-consuming, and hence it slows down the process of execution. The dynamic structure of Python also slows its speed because while executing the code, the excess work also needs to be completed. Therefore, in cases where fast acceleration is required, Python is not used there very commonly.
		2. Database connectivity - Python has a very high memory consumption. This is because it is flexible to the data types. It uses large amounts of memory. Python is not a good choice for tasks where the user wants to optimize memory, i.e., a memory-intensive language.
		3. Memory COnsumption - Python is not appropriate for mobile development as it is a fragile language. Since it is not memory efficient and has a prolonged power for processing, due to these reasons, Python does not have many built-in mobile applications.
		4. Mobile development - Python provides easy programming. However, when it interacts with the database, some issues arise. Compared to technologies like JDBC and ODBC, which are pretty famous, the database access layer of the Python programming language is primitive and underdeveloped.
		5. Run time errors - Since the language of Python is dynamically typed, there can be changes in the data type of a variable at any time. Therefore, it needs to be tested more often, and also, there are errors in the language displayed during runtime.

Q4. In what all domains can we use Python?

	Web Development
	Game Development
	Machine Learning and Artificial Intelligence
	Data Science and Data Visualization
	Desktop GUI
	Web Scraping Applications
	Business Applications
	Audio and Video Applications
	CAD Applications
	Embedded Applications

Q5. What are variable and how can we declare them?

	* Variable is a name given to a memory location. It is like a container to store values.
	* Variable names are case-sensitive and it can be alpha-numerical. Variable should not have special characters except '_' and a variable name can start with _. 
	* String variables can be declared either by using single or double quotes.
	* A variable is created the moment you first assign a value to it. Variables in Python do not need to be declared with any particular type, and can even change type after they have been set.
	Syntax - variable_name = value
	Ex:
		x = 4       # x is of type int
		x = "Sally" # x is now of type str
	* Type of variable can be checked using type() funtion
	type(variable-name)
		
	Q6. How can we take an input from the user in Python?

	input() is used to take input from the user through the console in Python.
		Ex: name = input()
			print("Name is ", name)
		
	We can also include some text to appear in the console to make it easy for the user as follows:
		Ex: name = input("Please enter your name to proceed further")
		This will appear in the console as follows 'Please enter your name to proceed further'

Q7. What is the default datatype of the value that has been taken as an input using input() function?

	String the default datatype of the value that has been taken as an input using input() function

Q8. What is type casting?

	The conversion of one data type into the other data type is known as type casting or type conversion.
	Ex:
	Consider a variable of type int.
	var_int = 6
	Now, it can be type casted to float as follows:
	typecasted_var_int = float(var_int)
	Now, typecasted_var_int is of type float which returns value as 6.0

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?

	We cannot take more than one input from the user using single input() function because python user input() function takes only one argument.

	If we want to take multiple inputs from user, we can do with the help of the following
		-Using split() method
			This function helps in getting multiple inputs from users. It breaks the given input by the specified separator. If a separator is not provided then any white space is a separator. Generally, users use a split() method to split a Python string but one can use it in taking multiple inputs.
			
			syntax: input().split(separator, maxsplit)
			Ex:	# taking two inputs at a time
				x, y = input("Enter two values: ").split()
				print("Number of boys: ", x)
				print("Number of girls: ", y)
				print("Number of boys: {} and Number of girls: {}".format(x, y))

		-Using List comprehension
			List comprehension is an elegant way to define and create list in Python. We can create lists just like mathematical statements in one line only. It is also used in getting multiple inputs from a user. 
			
			Ex:	# taking two input at a time
				x, y = [int(x) for x in input("Enter two values: ").split()]
				print("First Number is: ", x)
				print("Second Number is: ", y)
		

Q10. What are keywords?

	Keywords are a set of reserved words that have specific meanings and purposes and can’t be used for anything but those specific purposes. These keywords are always available—you’ll never have to import them into your code.

	As of Python 3.8, there are thirty-five keywords in Python. They are as follows:
	False, await, else, import, pass, None, break, except, in, raise, True, class, finally, is, return, and, continue, for, lambda, try, as, def, from, nonlocal, while, assert, del, global, not, with, async, elif, if, or, yield

	* All the keywords except True, False and None are in lowercase and they must be written as they are.
	Q11. Can we use keywords as a variable? Support your answer with reason.

	We cannot use a keyword as a variable name, function name, or any other identifier. They are used to define the syntax and structure of the Python language and hence we cannot use them as a variable name.

Q12. What is indentation? What's the use of indentaion in Python?

	Indentation refers to the spaces at the beginning of a code line.
	Where in other programming languages the indentation in code is for readability only, the indentation in Python is very important.
	Python uses indentation to indicate a block of code. Python will give you an error if you skip the indentation.
	The number of spaces is up to you as a programmer, but it has to be at least one.
		Ex: if 5 > 2:
			 print("Five is greater than two!") 
			if 5 > 2:
				print("Five is greater than two!") 
	You have to use the same number of spaces in the same block of code, otherwise Python will give you an error.
		Ex: if 5 > 2:
				print("Five is greater than two!")
					print("Five is greater than two!")


Q13. How can we throw some output in Python?

	Python print() function prints the message to the screen or any other standard output device.
	Syntax: 
	print(value(s), sep= ' ', end = '\n', file=file, flush=flush)

	Parameters: 
	value(s): Any value, and as many as you like. Will be converted to a string before printed
	sep=’separator’ : (Optional) Specify how to separate the objects, if there is more than one.Default :’ ‘
	end=’end’: (Optional) Specify what to print at the end.Default : ‘\n’
	file : (Optional) An object with a write method. Default :sys.stdout
	flush : (Optional) A Boolean, specifying if the output is flushed (True) or buffered (False). Default: False

	Return Type: It returns output to the screen.

Q14. What are operators in Python?

	Operators are used to perform operations on variables and values.

	Python divides the operators in the following groups:

	Arithmetic operators:
		Operator			Description																	Syntax
			+			Addition: adds two operands														x + y
			–			Subtraction: subtracts two operands												x – y
			*			Multiplication: multiplies two operands											x * y
			/			Division (float): divides the first operand by the second						x / y
			//			Division (floor): divides the first operand by the second						x // y
			%			Modulus: returns the remainder when the first operand is divided by the second	x % y
			**			Power: Returns first raised to power second										x ** y
		
	Assignment operators:
		Assignment operators are used to assign values to the variables.
		Operator								Description																			Syntax
			=			Assign value of right side of expression to left side operand 												x = y + z
			+=			Add AND: Add right-side operand with left side operand and then assign to left operand						a+=b, a=a+b
			-=			Subtract AND: Subtract right operand from left operand and then assign to left operand						a-=b, a=a-b
			*=			Multiply AND: Multiply right operand with left operand and then assign to left operand						a*=b, a=a*b
			/=			Divide AND: Divide left operand with right operand and then assign to left operand							a/=b, a=a/b
			%=			Modulus AND: Takes modulus using left and right operands and assign the result to left operand				a%=b, a=a%b
			//=			Divide(floor) AND: Divide left operand with right operand and then assign the value(floor) to left operand	a//=b, a=a//b
			**=			Exponent AND: Calculate exponent(raise power) value using operands and assign value to left operand			a**=b, a=a**b
			&=			Performs Bitwise AND on operands and assign value to left operand											a&=b, a=a&b
			|=			Performs Bitwise OR on operands and assign value to left operand											a|=b, a=a|b
			^=			Performs Bitwise xOR on operands and assign value to left operand											a^=b, a=a^b
			>>=			Performs Bitwise right shift on operands and assign value to left operand									a>>=b, a=a>>b
			<<=			Performs Bitwise left shift on operands and assign value to left operand									a<<= b, a=a<<b
	
		
	Comparison operators:
		Operator			Description																		Syntax
			>		Greater than: True if the left operand is greater than the right						x > y
			<		Less than: True if the left operand is less than the right								x < y
			==		Equal to: True if both operands are equal												x == y
			!=		Not equal to – True if operands are not equal											x != y
			>=		Greater than or equal to True if the left operand is greater than or equal to the right	x >= y
			<=		Less than or equal to True if the left operand is less than or equal to the right		x <= y
			is 		x is the same as y																		x is y
			is not	x is not the same as y																	x is not y	
		
	Logical operators:
		Operator		Description												Syntax
			and			Logical AND: True if both the operands are true			x and y
			or			Logical OR: True if either of the operands is true 		x or y
			not			Logical NOT: True if the operand is false 				not x	
	Identity operators:
		is and is not are the identity operators both are used to check if two values are located on the same part of the memory. Two variables that are equal do not imply that they are identical. 
		
			Operator	Description	
			is          True if the operands are identical 
			is not      True if the operands are not identical 
			
	Membership operators:
		in and not in are the membership operators; used to test whether a value or variable is in a sequence.
			Operator		Description	
			in            True if value is found in the sequence
			not in        True if value is not found in the sequence
	Bitwise operators:
		Operator	Description			Syntax
			&		Bitwise AND			x & y
			|		Bitwise OR			x | y
			~		Bitwise NOT			~x
			^		Bitwise XOR			x ^ y
			>>		Bitwise right shift	x>>
			<<		Bitwise left shift	x<<

Q15. What is difference between / and // operators?

	In Python programming, you can perform division in two ways. The first one is Float Division("/") and the second is Integer Division("//") or Floor Division.

	Float Division("/"): Divides left hand operand by right hand operand.
		5/2 = 2.5
	
	Floor Division("//"): The division of operands where the result is the quotient in which the digits after the decimal point are removed. But if one of the operands is negative, the result is floored , i.e., rounded away from zero (towards negative infinity).
		5//2=2
		-11//3 = -4

Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
```
	str = "iNeuron"*4
	print(str)

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.

	num = int(input("Enter a number"))
	if(num%2==0):
		print("Number is even")
	else:
		print("Number is odd")

Q18. What are boolean operator?

	The logical operators and, or and not are also referred to as boolean operators. While and as well as or operator needs two operands, which may evaluate to true or false, not operator needs one operand evaluating to true or false.
		Boolean and operator returns true if both operands return true.
		Boolean or operator returns true if any one operand is true
		The not operator returns true if its operand is a false expression and returns false if it is true.

Q19. What will the output of the following?
```
1 or 0

0 and 0

True and False and True

1 or 0 or 0
```
	1
	0
	False
	1

Q20. What are conditional statements in Python?

	Python supports the usual logical conditions from mathematics:

		Equals: a == b
		Not Equals: a != b
		Less than: a < b
		Less than or equal to: a <= b
		Greater than: a > b
		Greater than or equal to: a >= b
		These conditions can be used in several ways, most commonly in "if statements" and loops.

Q21. What is use of 'if', 'elif' and 'else' keywords?

	An "if statement" is is used to check a condition witht he help of conditional statements.
	The elif keyword is pythons way of saying "if the previous conditions were not true, then try this condition".
	The else keyword catches anything which isn't caught by the preceding conditions.

Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".

	age = int(input("Enter your age"))
	if(age>=18):
		print("I can vote")
	else:
		print("I cannot vote")

Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
	mylist= [12, 75, 150, 180, 145, 525, 50]
	sum=0
	i=0
	while i < len(mylist):
		if(mylist[i] % 2 ==0):
			sum=sum+mylist[i]
		i = i + 1
	print(sum)

Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.

	x, y, z = [int(x) for x in input("Enter three values with spaces between each number").split()]
	if(x>y & x>z):
		print(x," is greater")
	elif(y>x & y>z):
		print(y, " is greater")
	else:
		print(z," is greater")

Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
	numbers = [12, 75, 150, 180, 145, 525, 50]
	i=0
	while i < len(numbers):
		if(numbers[i] > 500):
			break

		if(numbers[i] % 5 ==0):
			if(numbers[i]<=150):
				print(numbers[i])
		i = i + 1
