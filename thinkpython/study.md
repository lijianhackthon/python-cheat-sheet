## ch1 The way of the program
- The way of thinking like a computer scientist combines some of the best features of mathematics, engineering, and natural science.
  - Like mathematics, computer scientist use formal languages to denote ideas (specifically computations).
  - Like engineers, they design things, assembling components into systems and evaluating tradeoffs among alternatives
  - Like scientists, they observe the behavior of complex systems, form hypotheses, and test predictions

- The single most important skill for a computer scientist is problem solving.
  - Problem solving means the ability to formulate problems, think creatively about solutions, and express a solution clearly and accurately.

- Programming languages are formal languages that have been designed to express computations

- When you read a sentence in English or a statement in a formal language, you have to figure out what the structure of the sentence is (although in a natural language you do this subconsciously). This process is called **parsing**

- The structure of a program is important. So it is usually not a good idea to read from top to bottom, left to right. Instead, learn to parse the program in your head, identifying the tokens and interpreting the structure.


## ch2 Variables, expressions and statements
- type('Hello World!') # will output <type 'str'>
- state diagram shows what state each of the variables is in
- python 2 has 31 keywords:
    - and  as  assert  break  class  continue  def  del  elif  else  except  exec  finally  for  from  global  if  import  in  is  lambda  not  or  pass  print  raise  return  try  while  with  yield
- An expression is a combination of values, variables, and operators. A value all by itself is considered an expression, and so is a variable.
- A statement is a unit of code that the Python interpreter can excute.
- Technically an expression is also a statement, but it is probably simpler to think of them as different things. The important difference is that an expression has a value; a statement does not.
- When operands of '+' are strings, it applies concatenation; When operands of '\*' are strings, it performs repetition. If one of the operands is a string, the other has to be an integer
- Variables names are case sensitive

## ch3 Functions
- The expression in parentheses is called the argument of the function
- A module is a file that contains a collection of related variables and functions
- Composition: one of the most useful features of Programming languages is their ability to take small building blocks and compose them. Almost anywhere you can put a value, you can put an arbitrary expression, with one exception: the left side of an assignment statement has to be a variable name.
- Inside the function, the arguments are assigned to variables called parameters, eg. def print_twice(bruce): print bruce    # bruce is a paramenter
- Variables and paramenters of functions are local
- To keep track of which variables can be used where, it is sometimes useful to draw a stack diagram. Like state diagrams, stack diagram show the value of each variable, but they also show the function each variable belongs to. Each function is represented by a **frame**. A frame is a box with the name of a function beside it and the parameters and variables of the function inside it.
- The frames are arranged in a stack that indicates which function called which. **__main__** is a special name for the topmost frame. When you create a variable outside of any function, it belongs to **__main__**
- traceback: A list of the functions that are executing, printed when an exception occurs.
- The order of the functions in the traceback is the same as the order of the frames in the stack diagram.
- Two ways to import:
  - import module_name
  - from module_name import *   # The disadvantage is that there might be conflicts between names defined in different modules, or between a name from a module and one of your variables.
