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

Q26. What is a string? How can we declare string in Python?

	String is the collection of the characters surrounded by single quotes, double quotes, or triple quotes in Python. The computer does not understand the characters; internally, it stores manipulated character as the combination of the 0's and 1's.
	Each character is encoded in the ASCII or Unicode character. So we can say that Python strings are also called the collection of Unicode characters.

	Declaration:
	string_name='string_value' or string_name="string_value" or string_name="'string_value"' (Triple quotes are generally used for represent the multiline or docstring)

Q27. How can we access the string using its index?

	The index of a string in python starts from 0. We can access the string using slice operator '[]' in Python.
	Eg:
	str='iNeuron'
	print(str[2]) 
	#Output e

	We can access the substring using : in the slice operator. It can be used as follows:
	Eg:
	str='iNeuron'
	print(str[:])
	#Output iNeuron

	print(str[0:3])
	#Output iNe

	print(str[2:5])
	#Output eur

	print(str[2:-2])
	#Output eur

	print(str[-1:])
	#Output n

	print(str[-4:-2])
	#Output ur

	print(str[-2:-4])
	#Output nothing

Q28. Write a code to get the desired output of the following
```
string = "Big Data iNeuron"
desired_output = "iNeuron"
```
	string = "Big Data iNeuron"
	print(string[9:])

Q29. Write a code to get the desired output of the following
```
string = "Big Data iNeuron"
desired_output = "norueNi"
```
	string = "Big Data iNeuron"
	print(string[-1:-8:-1])

Q30. Resverse the string given in the above question.

	string = "Big Data iNeuron"
	print(string[::-1])

Q31. How can you delete entire string at once?

	We can delete entire string at once using 'del' keyword.
	Ex:
	string = "Big Data iNeuron"
	del string

Q32. What is escape sequence?

	An escape sequence is a sequence of characters with special meaning when used inside a string or a character.

	Syntax: The characters need to be preceded by a backslash character
	Example: \n, \t etc.
	Ex:
	string = 'Hi! \'man'  
	print (string)
	#Output Hi! 'man  

Q33. How can you print the below string?
```
'iNeuron's Big Data Course'
```

	string='\'iNeuron\'s Big Data Course\''
	print(string)

	Q34. What is a list in Python?

	A list can be defined as a collection of values or items of different types. The items in the list are separated with the comma (,) and enclosed with the square brackets [].
	Python lists are mutable type its mean we can modify its element after it created.

	The list has the following characteristics:

	- The lists are ordered.
	- The element of the list can access by index.
	- The lists are mutable types.
	- A list can store the number of various elements.

Q35. How can you create a list in Python?

	A list can be define as below
	L1 = ["John", 102, "USA"]    
	L2 = [1, 2, 3, 4, 5, 6]   

	Q36. How can we access the elements in a list?

	The elements in the list can be accessed by the index.
	Eg:
	L1 = ["John", 102, "USA"]
	print(L1[0])
	#Output John

Q37. Write a code to access the word "iNeuron" from the given list.
```
lst = [1,2,3,"Hi",[45,54, "iNeuron"], "Big Data"]
``` 

	lst = [1,2,3,"Hi",[45,54, "iNeuron"], "Big Data"]
	print(lst[4][2])
#Output iNeuron

Q38. Take a list as an input from the user and find the length of the list.

	input_string = input("Enter list elements seperated by comma: ")
	lstEx  = input_string.split(",")
	print(len(lstEx))

Q39. Add the word "Big" in the 3rd index of the given list.
```
lst = ["Welcome", "to", "Data", "course"]
```

	lst = ["Welcome", "to", "Data", "course"]
	lst[3]="Big"
	print(lst)
	#Output ['Welcome', 'to', 'Data', 'Big']

Q40. What is a tuple? How is it different from list?

	A tuple is a collection of multiple items in a single variable which is ordered and unchangeable.
	Tuple items are ordered, unchangeable, and allow duplicate values.
	Tuple items are indexed, the first item has index [0], the second item has index [1] etc.

	Q41. How can you create a tuple in Python?

	my_tuple = ()
	print(type(my_tuple))
	#Output <class 'tuple'>

	thistuple = ("apple", "banana", "cherry", "apple", "cherry")
	print(thistuple)
	#Output ('apple', 'banana', 'cherry', 'apple', 'cherry')

	thistuple = ("apple",) 
	#For Tuple with single value, we should give , at the end. Otherwise, it will be considered as a String
	print(type(thistuple))
	#Output <class 'tuple'>

Q42. Create a tuple and try to add your name in the tuple. Are you able to do it? Support your answer with reason.

	As mentioned, once a tuple is created, you cannot change its values. Tuples are unchangeable, or immutable.
	But there is a workaround to edit a tuple once it is created. You can convert the tuple into a list, change the list, and convert the list back into a tuple.

	Eg:
	x = ("",)
	y = list(x)
	y[0] = "Sai Kiran"
	x = tuple(y)
	print(x)
	#Output ('Sai Kiran',)

Q43. Can two tuple be appended. If yes, write a code for it. If not, why?

	Yes, two tuples can be appended with the help of + operator.

	Eg:
	tuple1 = ("a", "b" , "c")
	tuple2 = (1, 2, 3)
	tuple3 = tuple1 + tuple2
	print(tuple3)
	#Output ('a', 'b', 'c', 1, 2, 3)

Q44. Take a tuple as an input and print the count of elements in it.

	TO take input from user, we use input function and a split function to pass a separator. If no separator is provided in split(), it defaultly takes 'space' as the separator.

	Eg:
	my_tuple = tuple(input('Enter comma-separated words: ').split(','))
	print(my_tuple)
	#Enter comma-separated words: 21,22,kiran,hi,34,sai
	#('21', '22', 'kiran', 'hi', '34', 'sai') 

	If we have not provided the split function, it will consider each character as a seperate value.
	Eg:
	my_tuple = tuple(input('Enter space separated words: '))
	print(my_tuple)
	#Output Enter space separated words: hi 21 kiran 32
	#('h', 'i', ' ', '2', '1', ' ', 'k', 'i', 'r', 'a', 'n', ' ', '3', '2') 

Q45. What are sets in Python?

	-Sets are used to store multiple items in a single variable.
	-Set is one of 4 built-in data types in Python used to store collections of data, the other 3 are List, Tuple, and Dictionary, all with different qualities and usage.
	-A set is a collection which is unordered, unchangeable*, and unindexed.
	-Set items are unchangeable, but we can remove items and add new items.
	-Sets cannot have two items with the same value.
	-You cannot access items in a set by referring to an index or a key.
	But you can loop through the set items using a for loop, or ask if a specified value is present in a set, by using the in keyword.

Q46. How can you create a set?

	Sets are represented by curly braces '{}'.

	We can create a set as follows
	thisset = {"apple", "banana", "cherry"}
	print(thisset)
	#Output
	#{'banana', 'cherry', 'apple'}

Q47. Create a set and add "iNeuron" in your set.

	setEx = {'hello', 'welcome'}
	print(setEx)
	setEx.add('iNeuron')
	print(setEx)
	#Output 
	#{'welcome', 'hello'}
	#{'iNeuron', 'welcome', 'hello'} 

Q48. Try to add multiple values using add() function.

	It is not possible to add multiple values using add() as it only takes one argument.

	setEx = {'hello', 'welcome'}
	print(setEx)
	setEx.add('iNeuron', 'hi')
	print(setEx)
	#Output
	#TypeError: add() takes exactly one argument (2 given) 

Q49. How is update() different from add()?

	add() can add only one value to a list. But update() can be used to add multiple items of any iterable object (tuples, lists, dictionaries etc.).
	Eg:
	thisset = {"apple", "banana", "cherry"}
	tropical = {"pineapple", "mango", "papaya"}
	thisset.update(tropical)
	print(thisset)
	#Output {'apple', 'banana', 'papaya', 'pineapple', 'mango', 'cherry'}

Q50. What is clear() in sets?

	clear() removes all the elements from the set.
	Eg:
	thisset = {"apple", "banana", "cherry"}
	thisset.clear()
	print(thisset)
	#Output set()

Q51. What is frozen set?

	Python frozenset() method creates an immutable Set object from an iterable. It is a built-in Python function. As it is a set object therefore we cannot have duplicate values in the frozenset.
	Syntax : frozenset(iterable_object_name)

Q52. How is frozen set different from set?

	Frozen set is just an immutable version of a Python set object. While elements of a set can be modified at any time, elements of the frozen set remain the same after creation. Due to this, frozen sets can be used as keys in Dictionary or as elements of another set.

Q53. What is union() in sets? Explain via code.

	Union() Method returns a new set which contains all the items from the original set.

	Syntax: set1.union(set2, set3, set4….)
	Parameters: zero or more sets
	Return: Returns a set, which has the union of all sets(set1, set2, set3…) with set1. It returns a copy of set1 only if no parameter is passed.

	A = {2, 4, 5, 6}
	B = {4, 6, 7, 8}
	print("A U B:", A.union(B))
	#Output {2, 4, 5, 6, 7, 8}

Q54. What is intersection() in sets? Explain via code.

	Return a set that contains the items that exist in both sets.

	A = {2, 4, 5, 6}
	B = {4, 6, 7, 8}
	print("A Intersection B:", A.intersection(B))
	#Output {4, 6}

Q55. What is dictionary in Python?

	Dictionary is the collection of key-value pairs where the value can be any Python object. In contrast, the keys are the immutable Python object, i.e., Numbers, string, or tuple.
	-Keys must be a single element
	-Value can be any type such as list, tuple, integer, etc.
	It is the ordered and mutable data-structure.

Q56. How is dictionary different from all other data structures.

	Dictionary is an unordered collection of the data values that we use for storing the data values, such as a map. Unlike the other DataTypes, which are capable of holding only a single value in the form of an element, a Dictionary is capable of holding the key:value pair.

Q57. How can we delare a dictionary in Python?

	The dictionary can be created by using multiple key-value pairs enclosed with the curly brackets {}, and each key is separated from its value by the colon (:).
	Eg:
	Dict = {"Name": "Tom", "Age": 22}

Q58. What will the output of the following?
```
var = {}
print(type(var))
```
	#Output <class 'dict'>

Q59. How can we add an element in a dictionary?

	The value can be updated along with key Dict[key] = value. The update() method is also used to update an existing value.
	Note: If the key-value already present in the dictionary, the value gets updated. Otherwise, the new keys added in the dictionary.

	Dict = {}   
	Dict[0] = 'First'  
	Dict[2] = 'Second'  
	Dict[3] = 'Third'  
	print(Dict)
	#Output {0: 'First', 2: 'Second', 3: 'Third'}

	Dict['Emp_ages'] = 20, 33, 24     
	print(Dict)
	#Output {0: 'First', 2: 'Second', 3: 'Third', Emp_ages: (20, 33, 24)}

Q60. Create a dictionary and access all the values in that dictionary.

	Dict = {
	  "brand": "Ford",
	  "model": "Mustang",
	  "year": 1964
	}
	x = thisdict.values()
	print(x)
	#Output dict_values(['Ford', 'Mustang', 1964])

Q61. Create a nested dictionary and access all the element in the inner dictionary.

	myfamily = {
	  "child1" : {
		"name" : "Emil",
		"year" : 2004
	  },
	  "parent" : "Hari"
	}
	x = myfamily["child1"]
	print(x)

	#Output {'name': 'Emil', 'year': 2004}

Q62. What is the use of get() function?

	get() method provides a convenient way of getting the value of a key from a dictionary without checking ahead of time whether the key exists, and without raising an error.

Q63. What is the use of items() function?

	items() returns a list of tuples containing the key-value pairs in a dictionary. The first item in each tuple is the key, and the second item is the key’s value

Q64. What is the use of pop() function?

	Removes a key from a dictionary, if it is present, and returns its value.

	If <key> is present in d, d.pop(<key>) removes <key> and returns its associated value:

	If <key> is not in d, and the optional <default> argument is specified, then that value is returned, and no exception is raised.
	Eg:
	dict_ex.pop('z', -1)  , here -1 is the argument specified to return if the key is not present in dictionary.

Q65. What is the use of popitems() function?

	The popitem() method removes the item that was last inserted into the dictionary. In versions before 3.7, the popitem() method removes a random item.
	The removed item is the return value of the popitem() method, as a tuple

Q66. What is the use of keys() function?

	The keys() method returns a view object which contains the keys of the dictionary, as a list.

Q67. What is the use of values() function?

	The values() method returns a view object which contains the values of the dictionary, as a list.

Q68. What are loops in Python?

	A loop is used for executing a block of statements repeatedly until a particular condition is satisfied.

Q69. How many type of loop are there in Python?

	There are two types of loops in Python.
	i. for
	ii. while
	iii. nested loops

Q70. What is the difference between for and while loops?

	while loop executes a set of statements as long as a condition is true.

	for loop is used for iterating over a sequence (that is either a list, a tuple, a dictionary, a set, or a string).

Q71. What is the use of continue statement?

	The continue statement we can stop the current iteration of the loop, and continue with the next iteration.

Q72. What is the use of break statement?

	The break statement stops the execution of the loop when it encounters break statement and comes out of the loop.

Q73. What is the use of pass statement?

	In Python programming, the pass statement is a null statement which can be used as a placeholder for future code.
	Suppose we have a loop or a function that is not implemented yet, but we want to implement it in the future. In such cases, we can use the pass statement.
	
	Eg:
	n = 10

	# use pass inside if statement
	if n > 10:
		pass

	print('Hello')
	
	#Output Hello

Q74. What is the use of range() function?

	The range() function returns a sequence of numbers, starting from 0 by default, and increments by 1 (by default), and ends at a specified number.

Q75. How can you loop over a dictionary?

	We can access a dictionary in the following ways.

	1. Access key using the build .keys() 
		Eg:
		statesAndCapitals = {
		'Gujarat': 'Gandhinagar',
		'Maharashtra': 'Mumbai',
		'Rajasthan': 'Jaipur',
		'Bihar': 'Patna'
		}
		 
		keys = statesAndCapitals.keys()
		print(keys)
		
	2. using for loop
		# Iterating over keys
		for state in statesAndCapitals:
			print(state)
		
	3. Iterate through all values using .values()
		# Iterating over values
		for capital in statesAndCapitals.values():
			print(capital)

	4. Iterate through all key, and value pairs using items()
		# Iterating over values
		for state, capital in statesAndCapitals.items():
			print(state, ":", capital)
	5. Access both key and value without using items()
		# Iterate through all values in a dictionary
		for i in statesAndCapitals:
		print(i, '->', statesAndCapitals[i])
		
	6. Print items in Key-Value in pair 
		#Iterating over key-value pairs
		keys = statesAndCapitals.items()
		print(keys)
		
	7. Access key using unpacking of dict_ex
		keys = [*statesAndCapitals]
		values = '{Gujarat}-{Maharashtra}-{Rajasthan}-{Bihar}'.format(*statesAndCapitals, **statesAndCapitals)
		print(keys)
		print(values)


### Coding problems
Q76. Write a Python program to find the factorial of a given number.

	fact_int=int(input("Please enter a number to get factorial "))
	factorial=1
	if(fact_int<0):
		print("No factorial for negative numbers")
	elif(fact_int==0 & fact_int==1):
		print("Factorial of number is 1")
	else:
		for i in range(1, fact_int+1):
			factorial=factorial*i
		print("Factorial of number is ", factorial)

Q77. Write a Python program to calculate the simple interest. Formula to calculate simple interest is SI = (P*R*T)/100

	P=float(input("Enter the Principal amount "))
	R=float(input("Enter the Interest Rate in decimal or percentage "))
	T=float(input("Enter the Time in Years "))

	simple_interest=(P*R*T)/100
	print("The Simple interest for the pprovided values is ", simple_interest)

Q78. Write a Python program to calculate the compound interest. Formula of compound interest is A = P(1+ R/100)^t.

	P=float(input("Enter the Principal amount "))
	R=float(input("Enter the Compound Interest Rate in decimal or percentage "))
	t=float(input("Enter the Time of Principal invested in Years "))

	compound_interest=P*(pow ((1+R/100),t))  
	print("The Simple interest for the pprovided values is ", compound_interest)

Q79. Write a Python program to check if a number is prime or not.

	num = int(input("Enter a number: "))

	if num > 1:
	   
	   for i in range(2,num):
		   if (num % i) == 0:
			   print(num,"is not a prime number")
			   break
	   else:
		   print(num,"is a prime number")

	else:
	   print(num,"is not a prime number")

Q80. Write a Python program to check Armstrong Number.

	num = int(input("Enter a number to check: "))
	sum = 0
	temp = num
	while temp > 0:
	   digit = temp % 10
	   sum += digit ** 3
	   temp //= 10

	if num == sum:
	   print(num,"is an Armstrong number")
	else:
	   print(num,"is not an Armstrong number")

Q81. Write a Python program to find the n-th Fibonacci Number.



Q82. Write a Python program to interchange the first and last element in a list.

	thisList = ['1', '2', '4', 'sai']
	lngth=len(thisList)
	temp1=thisList[0]
	thisList[0]=thisList[lngth-1]
	thisList[lngth-1]=temp1

	print(thisList)

Q83. Write a Python program to swap two elements in a list.

	thisList = ['1', '2', '4', 'sai']
	x=int(input("Enter first index"))
	y=int(input("Enter second index"))
	lngth=len(thisList)
	if(x|y<0 or x|y>lngth):
		print("Entered indexes are out of bound")
		exit()
	temp1=thisList[x]
	thisList[x]=thisList[y]
	thisList[y]=temp1

	print(thisList)

Q84. Write a Python program to find N largest element from a list.


	def findMax(list):
	 
		max = list[0]

		for x in list:
			if x > max:
				max = x
		return max

	input_string = int(input("Enter list elements seperated by comma: "))
	lstEx  = input_string.split(",")
	print("Largest element is:", findMax(lstEx))

Q85. Write a Python program to find cumulative sum of a list.

	list=[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]  
	cum_list=[]   
	sum = 0  
	for x in range(0,len(list)):  
		sum+=list[x]  
		cum_list.append(sum)   
	print(list)      
	print(cum_list) 

Q86. Write a Python program to check if a string is palindrome or not.

	str = input("Please enter a string: ")
	length=int(len(str))
	if(str[0:length-1:1]==str[length-1:0:-1]):
		print("Palindrome")
	else:
		print("Not a Palindrome")

Q87. Write a Python program to remove i'th element from a string.

	a = "Hello, World!"
	ip=int(input("Enter the index to remove it from string"))
	if(ip>len(a)):
		print("index out of bound")
	print(a.replace(a[ip], ""))

Q88. Write a Python program to check if a substring is present in a given string.

	MyString1 = "Hello there, this is python"
	ip=(input("Enter Substring: "))
	if ip in MyString1:
		print("Yes! it is present in the string")
	else:
		print("No! it is not present")

Q89. Write a Python program to find words which are greater than given length k.

Q90. Write a Python program to extract unquire dictionary values.

Q91. Write a Python program to merge two dictionary.

Q92. Write a Python program to convert a list of tuples into dictionary.
```
Input : [('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]
Output : {'Sachin': 10, 'MSD': 7, 'Kohli': 18, 'Rohit': 45}
```

Q93. Write a Python program to create a list of tuples from given list having number and its cube in each tuple.
```
Input: list = [9, 5, 6]
Output: [(9, 729), (5, 125), (6, 216)]
```

Q94. Write a Python program to get all combinations of 2 tuples.
```
Input : test_tuple1 = (7, 2), test_tuple2 = (7, 8)
Output : [(7, 7), (7, 8), (2, 7), (2, 8), (7, 7), (7, 2), (8, 7), (8, 2)]
```

Q95. Write a Python program to sort a list of tuples by second item.
```
Input : [('for', 24), ('Geeks', 8), ('Geeks', 30)] 
Output : [('Geeks', 8), ('for', 24), ('Geeks', 30)]
```

Q96. Write a python program to print below pattern.
```
* 
* * 
* * * 
* * * * 
* * * * * 
```
Q97. Write a python program to print below pattern.
```
    *
   **
  ***
 ****
*****
```

Q98. Write a python program to print below pattern.
```
    * 
   * * 
  * * * 
 * * * * 
* * * * * 
```

Q99. Write a python program to print below pattern.
```
1 
1 2 
1 2 3 
1 2 3 4 
1 2 3 4 5
```

Q100. Write a python program to print below pattern.
```
A 
B B 
C C C 
D D D D 
E E E E E 
```
