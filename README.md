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

## Notes on NGRX
 NgRx is a framework for building Reactive applications in angular. It also helps in maintaining the state throughout the application. <b>Reactive Programming</b> is way of programming way to handle asynchronous data stream and responding to the changes immediately. For example while watching cricket when batsman hits 6 we should not wait until the announcer announces it, as we are watching the cricketer on Tv.
 
<b>Store</b>
 - The central piece of ngrx is the store, which holds the state of the entire application in a single, immutable object.
 - The state is read-only and any changes are made through actions.
   
<b>Actions</b>
- It is plain javascript object that represent intention to change the state.
- It must have type property that describes type of Action being performed, can also carry Additional data as payload.
- Include the event (changes triggered) dispatched from Components.
  
<b>Reducers</b>
   - It is pure function used to handle the state change in response to the action.
   - Take current state and action as a parameter and return a new state.

<b>Selector</b>
  - Selector retrives the pieces of state from store.
  - They helps in encapsulating the logic for extracting data from store.

<b>Component</b>
-  Selector are used in component to get the data.

### Typescript
Typescript is strongly typed superset of Javascript that add optional types, classes, interface and many more features and compiles to plain JS(because browser can only understand JS) 
<p>Variable must be declared with its type. <b>If you try to assign value of one type with variable of another type, Typescript will generate a compilation error</b></p>

### Directives
Directives are the angular classes that can add new behaviour to the element in the template or modify the existing behaviour.
<p>Directive in angular can be categorized into following types</p>
<ul>
  <li>Component Directive: Components are directive that contains a template which is rendered in the place of a Component (Component = Directive + Template)</li>
  <li>Structural Directive: It is used to make the changes in the structure of a DOM. Element can be added or removed. hence, changing structure of a DOM. for eg: *ngFor , *ngIf etc</li>
  <li>Attribute Directive: It is used to make the changes in the behaviour or apperance of a DOM. For eg: ngStyle and ngClass</li>
</ul>
<p>note: Custom Directive is made using @Directive decorator</p>
<p>Component used to create UI widget. Directive is used to add behaviour to the exisiting DOM element.</p>
<p>Only one Component is present per one DOM. Many Directive can be used per DOM</p>
<p>Component contains Template. Directive doesn't contain Template</p>

### Decorators
<p>Decorator are special type of declaration that can be attached to class, method, properties or parameter allowing to configure or enhance their behaviour</p>
<p>Angular Decorator stores metadata about class, method and properties</p>
<ul>
  <li>Class decorator such as <b>@Component</b> and <b>@NgModule</b>  </li>
  <li>Property decorators for properties inside classes, such as <b>@Input</b> and <b>@Output</b>  </li>
  <li>Method decorators for methods inside classes, such as <b>@HostListener</b>  </li>
  <li>Parameter decorators for parameters inside class constructors, such as <b>@Inject</b> </li>
</ul>

### angular.json
It is a configuration file used by Angular CLI to manage various settings for Angular Project. It is a JSON file that defines structure and configuration of angular application.

### Angular CLI
It is a command line tool for creating, managing and building Angular applications. helps in following best practices while developing an angular application. It is built on top of Node js and npm(Node Package Manager)

### NPM 
It is default package manager for Node js. npm is used for managing and distributing JS packages.
<p>It is used for </p>
<ul>
  <li>Package installation</li>
  <li>Dependency Management</li>
  <li>Scripting</li>
</ul>

#### Package.json and Package-lock.json
<p>Package json contains information of Project such as name, version, scripts dependency etc.</p>
<p> Package-lock.json contain exact version of dependency installed including sub-dependencies. It is automatically created during npm install</p>
<p>note: 
In the context of Node.js and npm (Node Package Manager), dependencies refer to external packages or libraries that a Node.js project relies on to function correctly. These external packages are typically hosted on the npm registry, and npm is used to manage and install them. Dependencies are declared in the package.json file of a Node.js project.</p>

### Template 
Template is html view where data can be displayed by binding with Angular's Component. 
<p>Template can be declared inline inside component's template property or either link of seprate html file can be provided inside Component decorator's templateUrl</p>

### Module
Module are the ones used to group related component, directives and services. Application is divided into seperate module to seperate the functionality of the application.
<p>Module is declared with <b>@ngModule</b> Declararor </p> 
<p>MetaData for NgModule Decorator are as follows</p>
<ul>
  <li>import: Import is used to import other dependent modules</li>
  <li>declaration: It is used to define the Component in the respective module</li>
  <li>bootstrap: Tells angular which component to bootstrap in application</li>
  <li>provider: used to configure injectable objects</li>
</ul>

### Life-cycle of Angular
Angular application does have lifecycle of a component from its creation or initialization to the component destruction.
<ul>
  <li>ngOnchange: It is called when the @Input property of parent is changed</li>
  <li>ngOnit: Called at initialization of the component</li>
  <li>ngDoCheck: Custom Change detection </li>
  <li>ngAfterViewInit:Called in response after Angular initializes the component's view and child view. </li>
  <li>ngAfterViewChecked: Called After Angular checks component and child view</li>
  <li>ngDestroy: Cleanup phase when Angular destroys the component.</li>
</ul>

### Data Binding
It helps in smooth communication between the Component and DOM (Html Template).
<p>There are three forms of data binding</p>
<p>1. <b>From Component to the DOM</b></p>
<p>* Interpolation: {{value}} Adds the value of property from component</p>
<p>** Property Binding:  [property]=”value”: The value is passed from the component to the specified property or simple HTML attribute</p>

<p>2. <b>From DOM to the component</b></p>
<p>Event Binding: (event)=”function”: When the specific DOM event happens. for eg: Click Event</p>

<p>3. <b>Two way Data binding</b></p>
<p> Two-way data binding allows to have the data flow both ways.  for eg: [(ngModel)]</p>

### Pipes
pipes are function which accept an input value and return transformed value.

### Chaining Pipes
The chaning pipes use multiple pipes on input. for eg: - {{result | date | uppercase}}

### Service
A service is a logical entity, a typescript class and a resuable code which can be used in multiple components which can be implemented with the help of Dependency injection.

### Dependency Injection
Dependency injection is a technique for creating and delivering some part of application to another part of application which requires them.


### Provider
provider is an object inside decorator which inform Angular that particular service is available for injecting inside the component

### Synchronous Programming
As Js is single threaded task are executed one after another, Each task must be completed before starting another task

### Asynchronous Programming
In Asycnhronous programming tasks can be started, program can continue to execute other task without waiting for the completion of other task.

### async and await 
async keyword is used to define asynchronous functions and await keyword is used inside the function to wait until the promise get resolved or rejected. <br/>
async will always return a promise.

### Reactive Programming
It is programming practice to handle asynchronous data and react to the changes immediately.

### Rxjs
<p>Rxjs is a js library that helps us to work with asynchronous data stream with the help of observable</p>
Rxjs is library for reactive programming using Observable. It provides powerful tool for handling asynchronous operation and manage flow of data overtime.
<p>Observable represents the stream of data</p>
<p>Stream represents collection of inifinite data</p>
<p>Observer subscribe to the Observable and react to emmited values</p>
<p>Operators is used to transform or manipulate the data stream</p>
<p></p>

### Observable
Observable is representation of data stream or values that can be emitted over time. event can be data or notifications.
<p>useful for handling asynchronous operations</p>
<p>Can be helpful to work with data that arrive over time such as response from the server</p>
<p>Observer subscribe to observable to receive notifications</p>
<p>It is Lazy, nothing will happen until someone subscribes to it</p>

### Subject
Subject can be special type of observable that can act both as producer and consumer of values. 
<p>It allows you to multicast, multiple subscriber can subscribe to it, when Subject emits a new value all subscribed observers will receive that value.</p>

### Observer
Observer is an object that listen to the values emitted by Observable. It is consumer of Observable. 
<p>Observer has three callback functions: </p>
<ul>
  <li>next: it is called when observable emits a new value</li>
   <li>error: it is called when error occurs during execution of observable</li>
   <li>complete: it is called when observable has completed emitting values</li>
</ul>

### Comparing Observable vs Promise
<ul>
  <li>Observable emits multiple value over time where as promise emit single value at a time</li>
  <li>Observable are not executed until we subscribe it where as promise are executed immediately after creation</li>
  <li>It is cancellable using unsubsribe method where as promise are not cancellable</li>
</ul>

### HttpClient
Http client is built-in-service available in angular class which performs Http request.












   





