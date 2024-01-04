# JS Practice Notes
### Data Types 
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
       
### Hoisting in Javascript
This means that irrespective of where the variables and functions are declared, they are moved on top of the scope. The scope can be both local and global. <br/>
Note - Variable initializations are not hoisted, only variable declarations are hoisted: <br/>
![image](https://github.com/adityadahal/Practice-Notes/assets/107999400/a99de92c-e37d-412d-8dc7-358e57e14da0) <br/>

### Difference between “ == “ and “ === “ operators.
Both are <b>comparison operators</b>. The difference between both the operators is that <b>“==” is used to compare values</b> whereas, <b>“ === “ is used to compare both values and types</b>.

### Const Var and let
- const : Block Scoped. It is final keyword. Cannot redeclare after declaring it once.
- let:  Block Scoped. let are only visible in the block declared  (inside curly braces {} note: Includes if else statement, loop and other block statements).
- var: Function Scoped. Only visible in function they are declared. var is not recommended to use these days.
  note: Hoisting is possible in all 3 but let and const are hoisted but not initialized so accessing those returns Reference Error. While as accessing var returns undefined

###  Implicit Type Coercion
It is automatic conversion of value from one data type to another. for eg: <br/>
![image](https://github.com/adityadahal/JS-Practise-Notes/assets/107999400/5423c93c-9505-4387-890b-7e4544c226cb) <br/>

### NaN property in JavaScript
NaN property represents the “Not-a-Number” value. It indicates a value that is not a legal number. To check if a value is NaN, we use the isNaN() function, <br/>
![image](https://github.com/adityadahal/JS-Practise-Notes/assets/107999400/367cb086-f010-42ad-9657-41b418454215) <br/>


