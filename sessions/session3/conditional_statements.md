#Conditional Statements 

In order to code decisions into our javaScript programs it's necessary to use conditional statements know as `if` statements. 

An `if` statement is a
conditional statement which checks to see if a statement is `true`
or `false` and then executes some additional statements depending
on the result.

In javaScript a basic IF statement looks as follows:

```javascript
if (condition) { 
	//code to be executed if condition is true 
}
```
**A real example**

```javascript

//check if the statement 5 > 3 is true and if so
//then print a suitable message
	if (5 > 3){
		console.log("It is bigger!"); 
   }

```

We can also specify an alternative by using an `else` as follows:

```javascript
if (5 > 3){
		console.log("It is bigger!"); 
}else {
		console.log("It is smaller");

}
```
The bigger than symbol `>` is know as a comparison operator.  You may want to make use of the following operators:

|Operator | Description |
|---------|  -----------|
|==|equal to|
|!=|not equal|
|>|greater than|
|<| 	less than|
|>=|greater than or equal to|
|<=|less than or equal to||


We can only have 1 else with every if. If we want to specify more than one alternative then we have to use `else if`. 

Consider the following example:

```javascript 

if (role == "Teacher"){
	console.log("You are a teacher!");
}
else if (role == "Student"){
	console.log("You are a student!");
}
else if (role == "Admin"){
	console.log("Your are an admin");
}
else{
	 console.log("I don’t know what you are!");
}
```

In the above example you will notice that an `else if` statement is used
to specify alternative paths and that you can have more than 1 `else if`
statement. In fact, you can have as many `else if` statements as you
like.