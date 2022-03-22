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


Slicing Lists 


Nested Lists - 2D


Nested Lists - 3D 


Functions 



Arguments 



Return Statement 



List as Argument 


Scopes 


Arguments explained 



Tuples 


Dictionaries 


Python Internals 
