# pcep-preparation
This repository contains notes from PCEP Preparation

BASICS:  
Print function(built-in function, can be used without import)  
Function Execution:   
1. Check function name  
2. Check arguments passed  
3. Jump into the function   
4. Executes the function   
5. Returns to your code  
6. Resumes the execution   
    
\n - new line   
end="" (keyword argument)  
sep="" (keyword argument)  
     
Literals  
Numbers - Integers(123), Octal(0o123), Hexadecimal(0x123), Floating point(123.45)  
Strings - Double Quotes ("Hello!"), Single quotes ('Hello!'), Use quotes within strings ('Hi "hi"'), Escape quotes ('Hi \'hi\'')  
Boolean - False(False), True(True), Numeric False(0), Numeric True(1)   
      
Operators  
Arithmetic - +(Addition), -(Subtraction), *(Multiplication), /(Division), //(Floor Division), %(Modulo), **(Exponential)  
Binary Operator   
Unary Operator (-)  
Highest Priority - (+,-)unary, **, (*,/,//,% ), binary(+,-) Lowest Priority   
Same priority -> Left to right   
Sub-experession (To change default priority)   

Variables   
Variable name - upper/lower/digit/underscore, begin with letter/underscore, case sensitive, can't be reserved word(change casing to use reserved word)   
short cut operator (+=) cost += 2 instead of cost = cost + 2    
     
Comments   
created by # followed by text, multi-line comment should have # in every line  
     
Input   
input() - Always returns a string, deaf program(doesn't use input function)  
Type casting - int(), float()  
int(input())  
     
String Methods  
Arithmetic operators(+,*) can be used for strings, multiply by 0 or negative number returns empty string   
str can be used for casting integer/float   
  
MAKING DECISIONS:  
Comparison Operators  
==, !=, >, >=, <, <=  
     
Conditional Statements  
if condition:  
  print("The condition is met")  
elif:  
  print("only the second condition is true")  
else:  
  print("The condition is not met")  
    
Loops  
while condition:  
  print("condition")  
else:  
  print("condition")  
     
for i in range(10):   starts from 0   
for i in range(2,5):     
  if(i == 2):  
    break  
  print("i is: ",i)  
    
continue - skip current iteration   
    
Logic and Bit Operations  
Operators (and,or, not)  
True and True -> True   
True and False -> False   
False and True -> False   
False and False -> False   
      
True or True -> True   
True or False -> True   
False or True -> True   
False or False -> False   
     
not True -> False   
not False -> True   
      
Bitwise Operators   
&(Conjuction) |(Disjuction) ~(Negation) ^(Exclusive)   
& (1 and 1 Returns 1)  
| (At least one 1 Returns 1)  
^ (Exactly 1 Returns 1)  
~ (1 for every 0, 0 for every 1)  
Bit shifting - (>>, <<) Right or left   
right shift (integer division by 2)  
left shift (multiplication by 4)  
     
Lists   
collection of multiple elements, scaler and index  
access by using []  
len()  
del countries[1] => deletes the second item on the list     
countries[-1] => access last element in the list    
IndexError   
     
List Methods   
list.append() - add new item to end of list   
list.insert() - add new item in between value    
countries.insert(2,"Italy")  
swap items in list - using temp variable OR countries[0], countries[1] = countries[1], countries[0]  
list.sort() - default asc    
list.reverse() - first item will be last viz    
     
Iterating Lists   
ages = [56, 72, 24, 46]  
total = 0  
for age in ages:  
  total += age   
average = total / len(ages)  
print(average)  
     
Understanding Lists 
slice the list to avoid change of value in copied list 

Slicing Lists 
list[start:end]
print(letters[:]) - copy entire list with out modifying original list 
del letters[1:3] - modifies original list 

Finding in Lists 
element in list OR element not in list 

Nested Lists - 2D
list consist of other list 
classroom[2][1]
countries = [['Egypt', 'USA', 'India'],
       ['Dubai', 'America', 'Spain'], 
       ['London', 'England', 'France']]
countries2  = [country for sublist in countries for country in 
                       sublist if len(country) < 6]
print(countries2)

Nested Lists - 3D 
3D array or a queue 
school[1][2][1]


Functions 
def input_number():
  return int(input("Enter a number"))


Arguments 
def input_number(num):
  return int(input("Enter a number")) * num 
can use named parameters, default value for parameter   


Return Statement 
return - stop execution of function body 
def print_sum(num1, num2):
  sum = num1 + num2 
  if(sum == 0):
    return
  print("The sum is: ", str(sum))
python always returns none   
def is_even(num):
  if(num % 2 == 0):
    return True 
print(is_even(6)) => True 
print(is_even(7)) => None  
	

List as Argument 
def multiply_values(list):
   multiplied_values = []
   for item in list:
     multiplied_values.append(item * 2)
	 
   return multiplied_values  	 

print(multiply_values([1,2,3]))


Scopes 
variable inside function body is only within function 
if var not defined inside function body, uses global scope
use global to access variable outside function scope


Arguments explained 
vars vs list (replaces in original list)


Tuples 
List is mutable (can be modified) 
Tuple is immutable 
Uses paranthesis or set of values separated by commas 
elements in tuple can have different data types
to have 1 element in a tuple add comma in the end 
A Tuple is a collection of items that are ordered, unchangeable, and allow duplicate values.

Dictionaries 
consists of key/value, surrounded by curly brace, seperated by :
usernames = {
    "lydia": "lydiahallie",
	"sarah": "sarah123",
	"max": "max_",
	"joe": "joejoe",
}

print(usernames["sarah"])
Access methods: dictionary.key(), dictionary.values(), dictionary.items()
print(usernames.keys())
iterate using keys method 
for key in usernames.keys():
  print(key + " - " + usernames[key]) 

print(usernames.keys())
print(usernames.items()) - returns tuples consisting of key/value pair 
Modifying a dictionary - usernames["max"]="max123"
Add new value to dictionary - usernames.update({ "chloe": "chloe123" })
Delete - del usernames["max"]
remove all items in dict - usernames.clear()
remove last items in dict - usernames.popitem()
copy a dictionary - usernames_copy = usernames.copy()
  
  
Python Internals 
Interpreted language 
CPython, Cython, Jython, RPython(doesn't need interpreter to run)

Conclusion 
Buy voucher at outcert.com 
KODEKLOUD20 for 20% discount 


PCEP Mock Exam 1
1. …. is one of the literal types in Python.
Numeric, String, Boolean 
2. Which of the following statements assigns the value 50 to the variable x in Python:
x == 50, x >> 50, x : 50, x = 50 (correct)
3. What will be the output of the following Python code?
matrix = [[j for j in range(3)] for i in range(3)] 
print(matrix[1][2])
1, 4, 2(correct), 0 
4. What will be the output of below Python code?
list1 = [10, 11, 12, 13, 14]
print(list1[0])
11, 12, 10(correct), 14 
5. Write a Python program to create an empty tuple:
x = (0), x = (2,3), x = tuple(3), x = () (correct)
6. What would get printed:
min_score = 13
score = 13
print(score > min_score)
print(score <= min_score)
False False, False True(correct), True False, True True 
7. The …. function prints the specified message to the screen, or another standard output device.
input(), print()(correct), return(), vars()
8. What is the output of the following python code?
name = "Sally"# employee name
data = "#123" 
print (name+data)
Sally#123
9. What is the output of the following snippet:
a = (10, 20, 30, 40, 50)
a = a[::-1]
print(a)
(40,20), (10,30,50), (50,40,30,20,10)(correct), (10,20,30,40,50)
10. What will be the output of below Python code?
my_list = [0, 1, 2, 3, 4]
my_list.append("python")
print(my_list[2:])
[2,3,4,'python']
11. What does the following code produce as output?
i = 1
x = 3
sum = 0
while ( i <= x ):
 sum += i
 i += 1
print(sum)
6(correct),12,3,1
12. What will be the output of the following Python code?
matrix = [[[0, 1, 2], [0, 1, 2], [0, 1, 2]], [[0, 1, 2], [0, 1, 2], [0, 1, 2]], [[0, 1, 2], [0, 1, 2], [0, 1, 2]]]
matrix2 = []
for submatrix in matrix:
  for val in submatrix:
    matrix2.append(val)
print(matrix2[2][2])
1,2(correct),0,4
13. What is the output of the following snippet:
def get_even_func(numbers):
    even_numbers = [num for num in numbers if not num % 2]
    return even_numbers
get_even_func([1, 2, 3, 4, 5, 6])
[2,4,6]
14. for i in [9, 1, 5, 6]:, how many times a loop runs ?
2,1,4(correct),3
15. Given the nested if-else below, what will be the value x when the code executed successfully.
x = 0
a = 6
b = 6
if a > 0:
    if b < 0: 
        x = x + 6 
    elif a > 6:
        x = x + 5
    else:
        x = x + 4
else:
    x = x + 3

print(x)
4(correct),2,0,3
16. The function can have only one parameter. If any data (parameters) are passed, they are passed explicitly.
False(correct), True
17. The output of the following snippet of the code will be:
def my_function(x):
  return 10 - x
print(my_function(4))   
8,6(correct),9,5 
18. What will be the output of below Python code?
countries = ["USA", "Canada", "India"]
countries[0], countries[1] = countries[1], countries[0]
print(countries) 
['Canada','USA','India']
19. What will be the output of the below Python code?
list1=['UK','India','Canada']
list1.insert(1,8)
print(list1)	
['UK', 8, 'India', 'Canada']
20. What is the output of the following nested loop:
for num in range(5, 9):
   for i in range(2, num):
       if num%i == 1:
          print(num)
          break  
5678
21. What will be the output of below Python code?
list1 = [1, 2, 3, 4, 5]
for i in list1:
    if i==5:
        print(i)
5(correct),1,3,4
22. Which of the following method is used to delete a brand key and its value from the following dictionary:
testdict = {'brand': 'oppo', 'ram': '3', 'Os': 'Android', 'year': 2020}
del testdict['brand']
23. …. is a string method used to convert string into a lower case.
islower(),casefold()(correct),tolower(),lower()(correct)
23. What is the output of the following snippet:
x = 20
def my_function():
  x = 30
  print(x, end=' ')
my_function()
print(x, end=' ')
False, 20 20, Error, 30 20(correct) 
24. Which method should you use in order to convert the input into a string correctly:
year_of_birth = input("In what year were you born?")
print("You were born in" + ...(year_of_birth))
float, int, str(correct), bin 
25. A dictionary is a collection that is …, … and …
Ordered, changeable, does not allow dupicates 
26. The output of the following snippet of the code will be:
def fullname_func(fname, lname):
  print(fname + " " + lname)
fullname_func("John", "Mark")
John Mark 
27. What will be the output of the following Python code?
i = 5
while True:
    if i%0o11 == 0:
        break
    print(i)
    i += 1
5678
28. In Python, a variable must be declared before it is assigned a value:
True, False(correct) 
29. Fill out the missing operators:
20 ... 5 ... 4 = 16.0
/ and *
