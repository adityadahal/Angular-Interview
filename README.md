# JS Practice Notes
### 1. Data Types 
  1. Primitive Data Type
     - String: Represent series of Character(ch). It can be represented using single or double quotes.
     - Number: Represent number, Can be written with or without decimal.
     - Big Int : This data type is used to store numbers which are above the limitation of the Number data type. It can store large integers.
     - Boolean : Logical Entity. It has two values <b>true</b> or <b>false</b>.
     - Undefined: When variable is declared but not assigned any values. It has value of undefined and also it's type is undefined.
     - Null: Represents invalid or non-existent value.
       note: Type of Primitive data type can be checked by using "type of" method. <br/>
       ![image](https://github.com/adityadahal/Practice-Notes/assets/107999400/972bbbad-8264-403c-86f2-76a55725b0ce) <br/>

  2. Non-Primitive Data Type
     Primitive data type can only <b>store single value</b>. To store multiple and complex value Non-primitive data type are used.
     - Object : used to store collection of data. It <b>stores data in KEY VALUE pair</b>.
     - Array: It is collection of Data in ordered List. <br/>
       ![image](https://github.com/adityadahal/Practice-Notes/assets/107999400/af85f62c-6226-4981-af02-1b6e30e16803) <br/>
       
### 2. Hoisting in Javascript
This means that irrespective of where the variables and functions are declared, they are moved on top of the scope. The scope can be both local and global. <br/>
Note - Variable initializations are not hoisted, only variable declarations are hoisted: <br/>
![image](https://github.com/adityadahal/Practice-Notes/assets/107999400/a99de92c-e37d-412d-8dc7-358e57e14da0) <br/>

### 3. Difference between “ == “ and “ === “ operators.
Both are <b>comparison operators</b>. The difference between both the operators is that <b>“==” is used to compare values</b> whereas, <b>“ === “ is used to compare both values and types</b>.

### 4. Const Var and let
- const : Block Scoped. It is final keyword. Cannot redeclare after declaring it once.
- let:  Block Scoped. let are only visible in the block declared  (inside curly braces {} note: Includes if else statement, loop and other block statements).
- var: Function Scoped. Only visible in function they are declared. var is not recommended to use these days.
  note: Hoisting is possible in all 3 but let and const are hoisted but not initialized so accessing those returns Reference Error. While as accessing var returns undefined

###  5. Implicit Type Coercion
It is automatic conversion of value from one data type to another. for eg: <br/>
![image](https://github.com/adityadahal/JS-Practise-Notes/assets/107999400/5423c93c-9505-4387-890b-7e4544c226cb) <br/>

### 6. NaN property in JavaScript
NaN property represents the “Not-a-Number” value. It indicates a value that is not a legal number. To check if a value is NaN, we use the isNaN() function, <br/>
![image](https://github.com/adityadahal/JS-Practise-Notes/assets/107999400/367cb086-f010-42ad-9657-41b418454215) <br/>

### 7. Explain passed by value and passed by reference
In JavaScript, primitive data types are passed by value and non-primitive data types are passed by reference. for eg: <br/>
<b>Primitive Data Type </b> <br/>
   ![image](https://github.com/adityadahal/JS-Practise-Notes/assets/107999400/05e31157-be4b-4213-bb7d-12b5d8db12d4) <br/>
From the above example, we can see that primitive data types when passed to another variable, are passed by value. Instead of just assigning the same address to another variable, the value is passed and new space of memory is created. <br/>
<b>Non-Primitive Data Type</b> <br/>
![image](https://github.com/adityadahal/JS-Practise-Notes/assets/107999400/18b7a094-aef2-495c-80d6-f0d8c3b52512) <br/>
### 8. Higher Order Functions 
Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions. <br/>

### 9. this keyword
The this keyword refers to the current object in a method or constructor. The most common use of the this keyword is to eliminate the confusion between class attributes and parameters with the same name

### 10. Closures in Javascript
Closures are an ability of a function to remember the variables and functions that are declared in its outer scope. It is just like getter in Java. <br/>
![image](https://github.com/adityadahal/JS-Practise-Notes/assets/107999400/43460a4e-a157-46d6-bb4b-48d4f89f3274) <br/>

### 11. Callbacks 
A callback is a function that will be executed after another function gets executed(completion of another function). Any function that is passed as an argument to another function so that it can be executed in that other function is called as a callback function.



   





