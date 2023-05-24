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

### _**LISTS IN DART**_

- Dart list is similar to an array,which is the ordered collection of objects.
- The array is the most popular and commonly used collection in any other programming language.
- The syntax of declaraing the list is-
```dart

var list1 = [10,20,30,40,50]
```

- The Dart is defined by storing all elements inside the square bracket([]) and separated by commas(,).


![Flutter List](https://media.geeksforgeeks.org/wp-content/uploads/CommonArticleDesign1-min.png )


#### _**Creating a list**_

   - The following creates an empty list that will store integers:

```dart
int scores = [];
```

  - To create a list and initializes its elements, you place a comma-separated list of elements inside the square brackets ([]). In this example, Dart infers the list as List<int>.

- For example, the following creates a list of integers that have 4 numbers:



```dart
int scores = [1, 3, 4, 2];
```

- You can reassign the scores with an empty list:

```dart
scores = [];
```


- Dart understands that the scores is a list of integers.
-   If you attempt to assign a list of strings to it, you’ll get an error:
```dart
scores = ['one', 'three', 'four', 'two'];
```


- Error:

- A value of type 'List<String>' can't be assigned to a variable of type 'int'.

- Since the elements in the list are integers, you can use the var keyword to declare the list:

```dart
var scores = [1, 3, 4, 2];
```

- However, if you use the var keyword to declare a list and initialize its value to an empty list, Dart will infer the type of its elements as dynamic i.e., List<dynamic>. For example:

```dart
var scores = [];
```

#### _**Displaying a list**_

- To show the elements of a list, you can use the print() function. For example:

```dart

void main() {
  var scores = [1, 3, 4, 2];
  print(scores);
}
```

Output:

[1, 3, 4, 2]

#### **_Accessing elements_**
- Lists are zero-based indexing. It means that the first element has an index of 0, the second element has an index of 1, and so on.

- To access an element, you use subscript notation where the index goes within square brackets after the list name:

listName[index]

- For example, the following displays the 3rd element of the scores list:

```dart
void main() {
  var scores = [1, 3, 4, 2];
  print(scores[2]);
}
```

#### _**Assign values to elements**_
- To assign a value to an element, you also use the subscript notation. For example:

```dart
void main() {
  var scores = [1, 3, 4, 2];
  scores[2] = 5;

  print(scores);
}
```

Output:

[1, 3, 5, 2]

#### _**Adding elements to a list**_
- To add an element to a list, you use the add() method. The add() method appends an element at the end of a list. - For example:

```dart
void main() {
  var scores = [1, 3, 4, 2];
  scores.add(5);
  print(scores);
}
```

Output:

[1, 3, 4, 2, 5]


#### _**Removing elements from a list**_
- To remove an element from a list, you use the remove() method. 
- The following example uses the remove() method to remove number 1 from the scores list:

```dart
void main() {
  var scores = [1, 3, 4, 2];
  scores.remove(1);
  print(scores);
}
```


Output:

[3, 4, 2]


#### _**Immutable list**_
- To prevent a list from being reassigned to another list, you use the final keyword. For example:

```dart

final scores = [1, 3, 4, 2, 5];
```

- Since the scores list is final, you won’t be able to reassign it to another list. For example, the following will result in an error:

```dart
scores = [];
```

- Error:

   - The final variable 'scores' can only be set once.

  - However, you can operate on the list by adding an element or removing an existing element. For example:

```dart
void main() {
  final scores = [1, 3, 4, 2, 5];
  scores.add(6);
  print(scores);
}
```

Output:

[1, 3, 4, 2, 5, 6]

- To make a list truly immutable, you use the const instead of the final keyword:

```dart

void main() {
  const scores = [1, 3, 4, 2, 5];
  scores.add(6); // error
}
```


Output:

Unsupported operation: Cannot add to an unmodifiable list

### _**List properties**_

- To get the number of elements of a list, you use the length property. For example:

```dart
void main() {
  var scores = [1, 3, 4, 2, 5];
  print('Length: ${scores.length}');
}
```

- To access the first and last elements of a list, you use the first and last properties. For example:

```dart

void main() {
  var scores = [1, 3, 4, 2, 5];
  //
  print('First: ${scores.first}');
  print('Last: ${scores.last}');
}
```

Output:

First: 1
Last: 5


- To check if a list contains any elements, you can use the isEmpty or isNotEmpty property. For example:

```dart

void main() {
  var scores = [];
  print(scores.isEmpty); // true
  print(scores.isNotEmpty); // false
}
```

#### _**Iterating over list elements**_

- To iterate over list elements, you can use the for statement:

```dart

void main() {
  var scores = [1, 3, 4, 2, 5];
  for (var i = 0; i < scores.length; i++) {
    print(scores[i]);
  }
}
```


Output:

1
3
4
2
5

- In this example, we use a for loop that starts from the element 0 and ends at the element length-1. In each iteration, we access the element at an index and print it out.

- The for loop is quite verbose because you have to maintain a current index of the list elements. To make the code more concise, you can use the for in loop:

```dart

void main() {
  var scores = [1, 3, 4, 2, 5];
  for (var score in scores) {
    print(score);
  }
}
```
- In this example, the for-in loop assigns an element from the scores list to the score variable in each iteration.

- The List also has the forEach() method that executes a function for each element. For example:

```dart
void main() {
  var scores = [1, 3, 4, 2, 5];
  scores.forEach((score) => print(score));
}
```

- The function that you pass into the forEach() method takes the current element of the list as an argument. In this example, we pass an arrow function to the forEach() method, which prints out the score.

- Because the print() function is the same as the input forEach() method, you can make it shorter like this:

```dart

void main() {
  var scores = [1, 3, 4, 2, 5];
  scores.forEach(print);
}
```


#### _**Spreading list elements**_

- The spread operator (...) spreads list elements. For example, you can use the spread operator to combine multiple lists into one like this:

```dart

void main() {
  var lower = [1, 2, 3];
  var upper = [4, 5];
  var scores = [...lower, ...upper];
  print(scores);
}
```

-In this example, the ...lower returns all elements of the lower list and the ...upper returns all elements of the upper list. Therefore, the scores list contains all elements of both the lower and upper lists.

#### _**Collection if**_

- Dart provides you with a collection if for creating a list. The collection if to determine whether an element is included in a list based on a condition. For example:

```dart

void main() {
  var bye = true;
  var greetings = [
    if (bye) 'Good Bye',
    'Hi',
    'Hi there',
  ];

  print(greetings);
}
```

- In this example, if the bye variable is true, the collection if will include the 'Good Bye' element in the greetings list. Note that you can place an if collection anywhere in the list. It doesn’t have to be at the beginning of the list.

#### _**Collection for**_

- When creating a list, you can also use a collection for to generate elements from another list. For example:

```dart

void main() {
  var numbers = [1, 2, 3];
  var scores = [0, for (var number in numbers) number * 2];
  print(scores);
}
```

Output:

[0, 2, 4, 6]

- In this example, we use a for collection to iterate over the elements of the numbers list, double each of them, and assign the results as elements for the scores list.

### Summary

1.Use List<E> class to manage an indexable collection of elements. Lists are zero-based indexing.
2.Use the add() method to append an element to a list.
3.Use the remove() method to remove an element from a list.
4.Use for, for-in, and forEach() to iterate over list elements.
5.Use the final keyword to define a list that can be assigned once.
6.Use the const keyword to define an immutable list.

___


### _**MAPS & HASHMAPS IN DART**_

- In Dart programming, Mpas are dictionary-like data types that exist in key-value form (known as lock-key).
- There is no restriction on the type of data that goes in a map data type.
- Maps are very flexible and can mutate their size based on the requirements.
- It is important to note that all locks(keys) need to be unique inside a map data type.

- Syntax:
```dart
var map_name = {key1:value1, key2:value2,..., key n:value n}
```

**Defining Maps**
```dart
var map_name = {
  'Key1': 'Value1',
  'Key2': 2,
  'Key3': 3.0,
  'Key4': true,
  
};
```

Example:
```dart
var map_name = {
  'Name': 'Value1',
  'YearOfExperience': 2,
  'Avg.Rating': 3.0,
  'CanLocateToOffice': true,
  
};
```


**If we want to fetch some of it**:

```
print(map_name['Key2']);  //2

print(map_name['Key5']);  //null

print(map_name['key2']);  //null

print(map_name['Key4']);  //true
```

**How to add other value:**


```dart
var map_name = {
  'Name': 'Value1',
  'YearOfExperience': 2,
  'Avg.Rating': 3.0,
  'CanLocateToOffice': true,
  
};

map_name['key1'] = 'Sneha'; //{Key1: Value1, Key2: 2, Key3: 3.0, Key4: true, key1: Sneha}
  
print(map_name);
```

  **Another way of defining the Maps**

```dart
  var mapName = Map();

  mapName['Name'] = "Sneha";

  mapName['YearOfExperience'] = "Sneha";

  mapName['Name'] = "Sneha";
      
  print(mapName);
  ```

**How to remove**

```dart
print(mapName.isnotEmpty);  //true

print(mapName.isEmpty);  //false

print(mapName.length);  //4

print(mapName.Keys);  //(Name, YearOfExperience, Avg.Rating, CanLocateToOffice)

print(mapName.values);  //(Sneha, 2, 3.0, true)

print(mapName.containsKey('Name')); //true

print(mapName.containsValue(false));  //false

print(mapName.remove('CanLocateToOffice'));  //true

print(mapName);  //{Name: Sneha, YearOfExperience: 2, Avg.Rating: 3.0}

```
___

### _**Final vs Const Keywords - Difference and How to Use?**_

- Dart supports the assignment of constant value to a variable. These are done by the use of the following keyword:

1.const keyword
2.final keyword

- These keywords are used to keep the value of a variable static throughout the code base, meaning once the variable is defined its state cannot be altered. There are no limitations if these keywords have a defined data type or not.

**Final Keyword In Dart**

- The final keyword is used to hardcode the values of the variable and it cannot be altered in future, neither any kind of operations performed on these variables can alter its value (state).

```dart
// Without datatype
final variable_name;

// With datatype
final data_type  variable_name;
```

_Example_: Using the final keywords in a Dart program.

```dart
void main() {
   
  // Assigning value to geek1
  // variable without datatype
  final geek1 = "How are you?";
   
  // Printing variable geek1
  print(geek1);
    
  // Assigning value to geek2
  // variable with datatype
  final String geek2 = "Let's meet!!";
   
  // Printing variable geek2
  print(geek2);
}
```

  Output:
     How are you?
     Let's meet!!

**Const Keyword in Dart**

- The Const keyword in Dart behaves exactly like the final keyword. The only difference between final and const is that the const makes the variable constant from compile-time only. 
- Using const on an object, makes the object’s entire deep state strictly fixed at compile-time and that the object with this state will be considered frozen and completely immutable.

Example: Using const keywords in a Dart program.

```dart
void main() {
   
  // Assigning value to geek1
  // variable without datatype
  const geek1 = "How are you?";
   
  // Printing variable geek1
  print(geek1);
    
  // Assigning value to
  // geek2 variable with datatype
  const String geek2 = "Let's meet!!";
   
  // Printing variable geek2
  print(geek2);
}
 ```

Output:

 How are you?
 Let's meet!!
 
___


### _**CONDITIONS IN DART**_

- When you write a computer program, you need to be able to tell the computer what to do in different situations. 
- With conditions, you can control the flow of the dart program. Suppose you need to execute a specific code when a particular situation is true. 
- In that case, you can use conditions in Dart. 

**TYPES OF CONDITION**

1.If Condition
2.If-Else Condition
3.If-Else-If Condition
4.Switch case

### If Condition

- The easy and most common way of controlling the flow of a program is through the use of an if statement. 
- If statement allow us to execute a code block when the given condition is true. 
- Conditions evaluate boolean values.

- Syntax:
```dart

if(condition) {
    Statement 1;
    Statement 2;
       .
       .
    Statement n;
}
```

- Example Of If Condition
   

```dart
void main()
{
    var age = 20;
    
    if(age >= 18){
      print("You are voter.");
    }
}
```
Output:
  You are voter.

### If-Else Condition

- If the result of the condition is true, then the body of the if-condition is executed. 
- Otherwise, the body of the else-condition is executed.

- Syntax:
```dart

if(condition){
statements;
}else{
statements;
}
```
Example Of If-Else Condition:
- Dart program prints whether the person is a voter or not based on age.
```dart
  void main()
  {
        int age = 12;
        if(age >= 18){
            print("You are voter.");
        }else{
            print("You are not voter.");
        }
  }
  ```
Output:
   You are not voter.

  ### Condition Based On Boolean Value

- If the married status is false, it prints you are single; otherwise, it will print you are married.
```dart
  void main()
  {
        bool isMarried = false;
        if(isMarried){
            print("You are married.");
        }else{
            print("You are single.");
        }
  }
  ```
  Output:
    You are single.

### If-Else-If Condition

- When you have multiple if conditions, then you can use if-else-if. 
- You can learn more in the example below. 
- When you have more than two conditions, you can use if, else if, else in dart.

- Syntax:
```dart

if(condition1){
statements1;
}else if(condition2){
statements2;
}else if(condition3){
statements3;
}
.
.
.
else(conditionN){
statementsN;
}
```
 Example Of If-Else-If Condition:
 ```dart
 void main() {
  int noOfMonth = 5;

  // Check the no of month
  if (noOfMonth == 1) {
    print("The month is jan");
  } else if (noOfMonth == 2) {
    print("The month is feb");
  } else if (noOfMonth == 3) {
    print("The month is march");
  } else if (noOfMonth == 4) {
    print("The month is april");
  } else if (noOfMonth == 5) {
    print("The month is may");
  } else if (noOfMonth == 6) {
    print("The month is june");
  } else if (noOfMonth == 7) {
    print("The month is july");
  } else if (noOfMonth == 8) {
    print("The month is aug");
  } else if (noOfMonth == 9) {
    print("The month is sep");
  } else if (noOfMonth == 10) {
    print("The month is oct");
  } else if (noOfMonth == 11) {
    print("The month is nov");
  } else if (noOfMonth == 12) {
    print("The month is dec");
  } else {
    print("Invalid option given.");
  }
}
```
Output:
   The month is may

### Find Greatest Number Among 3 Numbers
- Dart program, which finds the greatest number among three numbers.
```dart
void main()
{
        int num1 = 1200;
        int num2 = 1000;
        int num3 = 150;

        if(num1 > num2  && num1 > num3){
            print("Num 1 is greater: i.e $num1");
        }
        if(num2 > num1 && num2 > num3){
           print("Num2 is greater: i.e $num2");
        }
        if(num3 > num1 && num3 > num2){
            print("Num3 is greater: i.e $num3");
        }
    }
```

 Output:
   Num 1 is greater: i.e 1200

  ### Switch Case 

  - In Dart, switch-case statements are a simplified version of the nested if-else statements. Its approach is the same as that in Java.

- Syntax:
```dart

switch ( expression ) { 
   case value1: { 
      // Body of value1
   } break; 
   case value2: { 
      //Body of value2 
   } break; 
   .
   .
   .
   default: { 
      //Body of default case  
   } break; 
} 
```

- The default case is the case whose body is executed if none of the above cases matches the condition.

- Rules to follow in switch case:


     1.There can be any number of cases. But values should not be repeated.
      2.The case statements can include only constants. It should not be a variable or an expression.
     3.There should be a flow control i.e break within cases. If it is omitted than it will show error.
   4.The default case is optional.
   5.Nested switch is also there thus you can have switch inside switch.


Example 1: Normal switch-case statement
```dart

void main()
{
    int gfg = 1;
    switch (gfg) {
    case 1: {
        print("Example number 1");
    } break;
    case 2: {
        print("Example number 2");
    } break;
    case 3: {
        print("Example number 3");
    } break;
    default: {
        print("This is default case");
    } break;
    }
}
```

Output:
   Example number 1

Example 2: Nested switch-case statement
```dart

void main()
{
    int gfg1 = 1;
    String gfg2 = "hello";
    switch (gfg1) {
    case 1: {
        switch (gfg2) {
        case 'hello': {
            print("Welcome to India");
        }
        }
    } break;
    case 2: {
        print("India number 2");
    } break;
    default: {
        print("This is default case");
    } break;
    }
}
```

Output:
    Welcome to India


___

### _**LOOPS IN DART**_

- In Programming, loops are used to repeat a block of code until certain conditions are not completed. 
- For, e.g., if you want to print your name 100 times, then rather than typing print(“your name”); 100 times, you can use a loop.

- There are different types of loop in Dart. They are:

 1. For Loop
2. For Each Loop
3. While Loop
4. Do While Loop

- Print Your Name 10 Times Without Using Loop
```dart

void main() {
    print("John Doe");
    print("John Doe");
    print("John Doe");
    print("John Doe");
    print("John Doe");
    print("John Doe");
    print("John Doe");
    print("John Doe");
    print("John Doe");
    print("John Doe");
}
```

 Output:
John Doe
John Doe
John Doe
John Doe
John Doe
John Doe
John Doe
John Doe
John Doe
John Doe

- Print Your Name 10 Times Using Loop

```dart
void main() {
  for (int i = 0; i < 10; i++) {
    print("John Doe");
  }
}
```
Output:
John Doe
John Doe
John Doe
John Doe
John Doe
John Doe
John Doe
John Doe
John Doe
John Doe

#### For Loop
- This is the most common type of loop. 
- You can use for loop to run a code block multiple times according to the condition. 
- The syntax of for loop is:
```dart

for(initialization; condition; increment/decrement){
            statements;
}
```

- Initialization is executed (one time) before the execution of the code block.
- Condition defines the condition for executing the code block.
- Increment/Decrement is executed (every time) after the code block has been executed.

- Example : Display Sum of n Natural Numbers Using For Loop
```dart
void main(){

  int total = 0;
  int n = 100; // change as per required
  
  for(int i=1; i<=n; i++){
    total = total + i;
  }
  
  print("Total is $total");
  
}
```
Output:
Total is 5050

#### For Each Loop

- The for each loop iterates over all list elements or variables. 
- It is useful when you want to loop through list/collection. 
- The syntax of for-each loop is:
```dart

collection.forEach(void f(value));
```
- Example: Print Each Item Of List Using Foreach
```dart

void main(){
  List<String> footballplayers=['Ronaldo','Messi','Neymar','Hazard'];
  footballplayers.forEach( (names)=>print(names));
}
```
Output:
Ronaldo
Messi
Neymar
Hazard

#### While Loop

- In while loop, the loop’s body will run until and unless the condition is true. 
- You must write conditions first before statements. 
- This loop checks conditions on every iteration. 
- If the condition is true, the code inside {} is executed, if the condition is false, then the loop stops.

- Syntax:
```dart
while(condition){  
       //statement(s);  
      // Increment (++) or Decrement (--) Operation;  
}  
```

-A while loop evaluates the condition inside the parenthesis ().
- If the condition is true, the code inside {} is executed.
- The condition is re-checked until the condition is false.
- When the condition is false, the loop stops.
- Example: To Print 1 To 10 Using While Loop
```dart

void main() {
  int i = 1;
  while (i <= 10) {
    print(i);
    i++;
  }
```
Output:
1
2
3
4
5
6
7
8
9
10

#### Do While Loop

- Do while loop is used to run a block of code multiple times. 
- The loop’s body will be executed first, and then the condition is tested. 
- The syntax of do while loop is:
```dart

do{
    statement1;
    statement2;
    .
    .
    .
    statementN;
}while(condition);
```

- First, it runs statements, and finally, the condition is checked.
- If the condition is true, the code inside {} is executed.
- The condition is re-checked until the condition is false.
- When the condition is false, the loop stops.
 
 - Example : To Print 1 To 10 Using Do While Loop

```dart
void main() {
  int i = 1;
  do {
    print(i);
    i++;
  } while (i <= 10);
}
```
Output:
1
2
3
4
5
6
7
8
9
10

___