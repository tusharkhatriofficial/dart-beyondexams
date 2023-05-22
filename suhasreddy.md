# All about Dart

Dart is an open-source object-oriented programming language with c-style syntax which was developed by **Google in 2011**

It is Focused on **frontend**(mobile,web apps) **user interface**(UI) development. 

void main(){
    for(int i=0; i<5; i++){
        print('hellow ${i + 1}');
    }
}

# Benefits of Dart

* Use of async and awit for asynchronous programming.

* Dart is one of very few languages(and perhaps the only "mainstream" language) that is well suited to being complied both **AOT(ahead-of-time)** and **JIT(just-in-time)**. Supporting both kinds of compliation provides significant advantages to Dart and (especialy) Flutter (**Hot Reload Feature**)

* JIT compilation is used during development, using a complier that is especially fast

* Extremely fast development cycles, and fast execution and startup times

* Flutter doesnt split layout between your program and an additional templating or layout language like JSM or XML, nor does it require separate visual layout tools



# Creating First Program In dart

As we have discussed earlier, Dart is easy to learn if you know any of Java, C++, JavaScript, etc. The simplest "Hello World" program gives the idea of the basic syntax of the programming language. It is the way of testing the system and working environment. In this tutorial, we will give the basic idea of Dart's syntax. There are several ways to run the first program, which is given below:

**Using Command Line**
**Running on Browser**
**Using IDE**

Before running the first program, it must ensure that we have installed the Dart SDK properly

void main(){
    print('Welcome to Dart');

    stdout.write('Enter your Name:');

    var name = stdin.readLineSync();

    print("Welcome, $name");
}

this program first take input and give output

output: 
Welcome to Dart
Enter your Name: suhas 
Welcone, suhas


# Dart Class and Object

# Classes

* Dart classes are the blueprint of the object, or it can be called object constructors. A class can contain fields, functions, constructors, etc.

* We can assume a class as a sketch (prototype) or a car. It contains all the details about model name, year, features, price, etc.

* Dart provides class keyword followed by a class name is used to define a class; all fields and functions are enclosed by the pair of curly braces ({})

**Syntax**

class ClassName {  
   <fields>  
   <getters/setters>  
  <constructor>  
 <functions>  
}  

# Objects

* Dart is object-oriented programming, and everything is treated as an object in Dart. An object is a variable or instance of the class used to access the class's properties.Object have two features - state and behavior.

* Suppose a man is an object with a state (name, age, health) and behavior (walking, running, and sleeping).

* After creating the class, we can create an instance or object of that class which we want to access its fields and functions. The new keyword is used to declare class followed by the class name. 

# Syntax

var object_name = new class_nsme(<constructor_arguments>);


# Dart Data Types

# Number	
**Keyword**-int, double, num	
**Function**-Numbers in Dart are used to represent numeric literals

# Strings	
**Keyword**-String	
**Function**-Strings represent a sequence of characters

# Booleans	
**Keyword**-bool	
**Function**-It represents Boolean values true and false

# Lists	
**Keyword**-List	
**Function**-It is an ordered group of objects

# Maps	
**Keyword**-Map	
**Function**-It represents a set of values as key-value pairs

# Variables

* A variable name is the name assign to the memory location where the user stores the data and that data can be fetched when required with the help of the variable by calling its variable name.

__Syntax__- to declare variable

    type variable_name;

__Syntax__: to declare multiple variabels of same type:

    type variable1_name, variable2_name, variable3_name,......variableN_name;


# Difference between var and dynamic in Dart

* If you use var when you need to change your variable data Type with the passage of time, suppose first you store a string in a var data type then you have to store an int value in the same data type, You cannot achieve this thing with var.

* If a variable is declared as dynamic you can change its type anytime.

but if a variable is declared with var keyword and have an initial value its type cant be changed else if its not intialized you can change its DataType anytime too.
 
# Dart Functions

* Function is a set of statements that take inputs, do some specific computation and produces output. 

* Functions make it easy to divide the complex program into smaller sub-groups and increase the code reusability of the program.

__Syntax__: 

```dart
return_type function_name ( parameters ) {
   // Body of function
   return value;
}
```
* Basically, there are four types of functions in Dart. 

These are as follows:

* No arguments and no return type : Basically in this function, we do not give any argument and expect no return type.

* With arguments and no return type : Basically in this function, we do not give any argument but expect a return type. 

* No arguments and return type : Basically in this function, we are giving an argument and expect no return type. 

* With arguments and with return type : Basically in this function, we are giving an argument and expect return type.

# List in Dart

* Dart List is similar to an array, which is the ordered collection of the objects. 

* The array is the most popular and commonly used collection in any other programming language

* The syntax of declaring the list
      *var list1 = [10,20,30,40,50]*

* The Dart list is defined by storing all elements inside the square bracket ([]) and separated by commas (,).

void main() {   
   var list1 = new List(5);   
   list1[0] = 10;   
   list1[1] = 11;   
   list1[2] = 12;   
   list1[3] = 13;  
   list1[4] = 14;    
   print(list1);   
}

*Output*

[10,11,12,13,14]

# Maps and in dart

* In Dart programming, Maps are dictionary-like data types that exist in key-value form (known as lock-key).

* There is no restriction on the type of data that goes in a map data type.

* Maps are very flexible and can mutate their size based on the requirements.

* It is important to note that all locks(keys) need to be *unique* 

   var map_name = {key:1 value1, key2:value2,.....keyn:valuen}

main() {
    
    var map_name = {
        'Name':'Value1',
        'YearOfExperience': 2,
        'Avg.Rating': 3.0,
         'CanLocateToOffice': true,
    };

    map_name['Name'] = 'Raman';
    print(map_name);
}

# Difference between final and const

* The final keyword is used to hardcode the values of the variable and it cannot be altered in future, neither any kind of operations performed on these variables can alter its value (state).

// Without datatype
final variable_name;

// With datatype
final data_type  variable_name;

* The Const keyword in Dart behaves exactly like the final keyword. 
* The only difference between final and const is that the const makes the variable constant from compile-time only. 
* Using const on an object, makes the object’s entire deep state strictly fixed at compile-time and that the object with this state will be considered frozen and completely immutable.

# Conditional Programming in Dart

* Conditional in programming handles decision and performs specific actions, if the specified conditions are met.

* The following are the forms of conditional in Dart Programming:

     if statement: 
     if … else statement
     if … else if … statement
     switch statement
     nested statement

* An if can be followed by an optional else block. The else block will execute if the Boolean expression tested by the if block evaluates to false.     

main(){
    var a = 100;

    if(a>200){
      //Cond 1 is true
    } else if(a<50){
      //Cond 2 is true
    } else if(a>80){
      //Cond 3 is true
    } else {
      //all Cond are false
    }
}

# Loops in Dart

*For loops*
* You can iterate with the standard for loop. For example:

var message = StringBuffer('Dart is fun');
for (var i = 0; i < 5; i++) {
  message.write('!');
}
* Closures inside of Dart’s for loops capture the value of the index.

*While and do-while*
A while loop evaluates the condition before the loop:

while (!isDone()) {
  doSomething();
}
A do-while loop evaluates the condition after the loop:

do {
  printLine();
} while (!atEndOfPage());

*Break and continue*
Use break to stop looping:

while (true) {
  if (shutDownRequested()) break;
  processIncomingRequests();
}
Use continue to skip to the next loop iteration:

for (int i = 0; i < candidates.length; i++) {
  var candidate = candidates[i];
  if (candidate.yearsExperience < 5) {
    continue;
  }
  candidate.interview();
}