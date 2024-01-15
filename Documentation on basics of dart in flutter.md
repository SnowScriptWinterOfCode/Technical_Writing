### **Flutter**
An open souce UI software development toolkit by Google.
Cross platform framework
A single code can be used to create application fo mobile, web and desktop
The language used in flutter is dart

### **Dart**
Developed by Google
features such as object oriented, class based and C syntax
strongly typed language with just in time and ahead of time complication

**Operators in dart**
Arithmetic: + - * / %
Relational: == != > < >= <=
Logical: && || !

**Comments**
Single line: //
Multiline: /* */

**Variables**
Hold data values
Numeric- int, double
Textual- string
Boolean- bool

**Final variables**- The variables whose value can be set only once and is determined at the runtime.

**Constant variables**- Variables who are constant and are set at the compile time. 

**Runtime**- When is compiled code is executed and the program performs task to produce final result or output during execution.

**Compile time**- When the source code is converted into machine or lower level code by a compiler and produces an executable file or code.

**Conditionals**
**(1) if else**
**(2) Ternary:** condition ? true statement: false statement
**(3) Switch:** used for multi branch decision and handles multiple possible values of variable

**Loops**
**(1) for loop:** used to iterate over a range and for fixed number of interations.
**(2) while loop:** executes a block of code as long as the condition is true.
**(3) do while loop:** generates atleast one execution of code. Rest working same as while loop.

**Continue keyword**- skips the rest of the loop code and proceeds to next iteration. useful for skipping specific iterations based on condition.

**Break keyword**- exits the loop or switch entirely. useful for terminating the loop based on specific conditions.

**Functions**
block of reusable code
encapsulate a set of instructions and gives modular code

Returntype functionname(parameters){
    //code
}

**Arrow functions**
short syntax, one line functions
for functions with single expression
No return statement
returns result of expression automatically

int add(int a, int b) => a+b; 

**Classes**
blueprint of creating objects
represents real world entities

class classname{
    //members
}

**Abstract classes**
cannot be instantiated 
provides blueprint of other classes

abstract class name{
    //code
}

**Constructors**
method for intialising objects
default constructor used if none is defined
has same name as class

**this keyword**
current instance of class
avoids naming conflict between instance varibles and parameters

**Getters**- methods that provide access to values of private instance variables
string get getname => name;

**Setters**- methods that allow modification of private instance variables
set setage(int newage)
=> age=newage;

**Static functions**- belong to class and are accessed using class name
**Static varibles**- shared among all instances of the class

**Private variables**
denoted by underscore (_) before variable name
restricts access to variable from outside class

class person {string -secret;}

**Class modifiers**
**(1) Abstract:** prevents instantiation of class
**(2) Final:** prevents class from being subclassed
**(3) Const:** requires all fields to be final

**Lists in dart**
ordered collection of elements
only same data type elements allowed

List <int> numbers =[1,2,3,4];

**Operations:** numbers[0] (Access)
numbers.add(6)
numbers.remove(3)
numbers.length

**Sets in dart**
unordered collection of unique elements
no duplicate elements

set <string> fruits={"apple", "banana"};

**Operations:** fruits.add("")
fruits.remove("")
fruits.contain("apple")
fruits.length

**Maps in dart**
collection of key value pairs
keys are mutable and the values are immutable

Map <string><int> scores= {"john":8,"jane":9};

**Operations:** scores["john]
scores ["jane"]=7
scores.remove("jane")
scores.length

**Asynchronous programming**
allows tasks to run concurrently without blocking main program flow
dart uses future and stream classes to handle asynchronous operations

**Exception handling in dart**
**(1) Try catch blocks:**
used to handle exceptions in synchronous code

try{
    //code that might give error
}
catch(e){
    //code to handl exception
}

**(2) Async-await:**
used in asynchronous code
readable exception handling
await keyword used only inside async function
async keyword used in function declaration
await used before future to pause execution until future completes

Future<void>
fetchdata() async{
    try{
        //asynchronous code that might throw exception
    }
    catch(e){
        //code to handle exception
    }
}
 
**Future (promises) in dart**
represents value or error available at some time in future
used for asynchronous operations

**Stream in dart**
represents sequence of asynchronous events over time
useful for handling continous data
ex: user input or data from server

