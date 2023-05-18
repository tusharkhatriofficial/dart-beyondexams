## _**WHAT IS A DART?**_


- Dart is a language that focused on **frontened** (mobile,web apps) **User Interface(UI)**
- Dart is developed by **Google** in 2011 and is a mixture of JavaScript,Java,C#
- Dart is an **Object Oriented & Strongly Typed**


___
### _**BENEFITS OF DART**_

 - Easy to learn
 - Comes with good documentation
 - Dart syntax is clean
 - Can compile to self-contained snapshots
 - It is portable
 - It is the only language that is well suited to being compiled both **AOT** (ahead-of-time) and **JIT** (just-in-time)
 - Extremely fast development cycles & fast execution & startup times


___


#### _**FIRST DART PROGRAM**_

```dart

void main() {

    print('Welcome to Dart!'); //used to show the output

    stdout.write('Enter your name:'); //used to show the output

    var name = stdin.readLineSync(); //can also use stdout 

    print("Welcome, $name");

}
```
___


### _**DART CLASS**_

- Class is the blueprint of objects and class is the collection of data member and data function means which include this fields, getter and setter and constructor and functions.


Syntax:  
```dart
class class_name {

    //Body of class
}
```
where- 
- Class is the keyword use to initialize the class.
- class_name is the name of the class.
- Body of class consists of fields, constructors, getter and setter methods, etc.

Example:
```dart
class fruit {

   fruit();

}
```

### _**DART OBJECT**_

- Objects are the instance of the class and they are declared by using new keyword followed by the class name.

Syntax:  
```dart
var object_name = new class_name([ arguments ]);
```

- new is the keyword use to declare the instance of the class
- object_name is the name of the object and its naming is similar to the variable name in dart.
- class_name is the name of the class whose instance variable is been created.
- arguments are the input which are needed to be pass if we are willing to call a constructor.


After the object is created, there will be the need to access the fields which we will create. We use the dot(.) operator for that purpose.

Syntax:  
```dart
 // For accessing the property
object_name.property_name;

// For accessing the method
object_name.method_name();
```

___

### _**DART VARIABLES**_

- A variable name is the name assign to the memory location where the user stores the data and that data can be fetched when required with the help of the variable by calling its variable name.

**TYPES OF VARIABLES**
1. Integer
2. Double
3. String
4. Booleans
5. Lists
6. Maps

**Declaration of Variables**
```dart
type variableName;
```
_Example_
```dart
int a; //declaration of variable
a=5; //initialization
print(a);

num or double percentage = 99.5; //syntax of num & double data type

bool isLogin = false; //syntax of boolean data type





```
**Inline Variable**

```dart
String name = Sneha;
name = SnehaKumari;
```

___

### _**DART VAR vs DYNAMIC-DIFFERENCE**_

- **Var**: 
   - can’t change TYPE of the variable, but can change the VALUE of the variable later in code.
   - Use var if you expect a variable assignment to change during its lifetime:

```dart
var msg = "Hello world.";
msg = "Hello world again.";
```

- **Dynamic**: 
   - can change TYPE of the variable, & can change VALUE of the variable later in code.


- Both in dynamic and var, the variable can hold data of any data type, i.e., int, float, string, if a variable is declared as a dynamic and if even initialized, its type can change over time.

```dart

void main() {
  dynamic x = 'abc';
  x = 12345;
  print(x);
}
```

- If you declare a variable as a var, once assigned type can not change.

```dart

void main() {
  var x = 'abc';
  x = 12345;
  print(x);
}
```

- The above code will result in the error stating that A value of type ‘int‘ can’t be assigned to a variable of type ‘String‘ – line 3

- BUT, if you state a var without initializing, it becomes a dynamic:

```dart

void main() {
  var x ;
  x = 'abc';
  x=12345;
  print(x);
}
```

___

### _**WHAT ARE FUNCTIONS?**_

- Function is a set of statements that take inputs, do some specific computation and produces output.
-  Functions are created when certain statements are repeatedly occurring in the program and a function is created to replace them. 
- Functions make it easy to divide the complex program into smaller sub-groups and increase the code reusability of the program.

```dart

return_type function_name ( parameters ) {
   // Body of function
   return value;
}
```
- In the above syntax: 

  - function_name defines the name of the function.
  -  return_type defines the datatype in which output     is going to come.
  -  return value defines the value to be returned from the function.

- The function is called as: 
```dart
function_name (argument_list);
```

- In the above syntax: 

     - function_name defines the name of the function.
     - argument list is the list of the parameter that the function requires.

**Example:**

```dart

int add(int a, int b)
{
	// Creating function
	int result = a + b;
	// returning value result
	return result;
}

void main()
{
	// Calling the function
	var output = add(10, 20);

	// Printing output
	print(output);
}
```

___