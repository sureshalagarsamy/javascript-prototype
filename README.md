### Prototype in JavaScript

> 
> What is Prototype in JavaScript?
>
> How to create prototype in JavaScript?

</br>
All the JavaScript objects have an object and its property called <b><em>prototype</em></b> and its used to add the custom functions and property.

The example looks like,


 ```javascript
 var employee = function () {
    //This is a constructor  function.
}

//Crate the instance of above constructor  function and assign in a variable
var empInstance = new employee();
empInstance.department = "IT";

console.log(empInstance.department);//The output of above is IT.

//The example with prototype as given below.
var employee = function () 
{ 
	//This is a constructor  function.
}

employee.prototype.department = "IT";//Now, for every instance employee will have a department.

//Crate the instance of above constructor function and assign in a variable
var empInstance = new employee();
empInstance.department = "HR";

console.log(empInstance.department);//The output of above is HR not IT.
 ```
