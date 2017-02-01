# Conditional Statements

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

```
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
to specify alternative paths and that you can have more than 1 `else if`  statement. In fact, you can have as many `else if` statements as you like.


#Multiple conditions

 You can join together different conditions with "or” or “and” statements, to test whether either statement is true, or both are true, respectively.

In JavaScript “or” is written as `||` and “and” is written as `&&`.

Say you want to test if the value of x is between 10 and 20—you could do that with a condition stating:

```
if(x > 10 && x < 20) {
    ...
}
```

If you want to make sure that country is either “England” or “Germany” you use:

```
if(country === 'England' || country === 'Germany') {
    ...
}
```




##Section Exercise

##Exercise 1 `if` 


{% exercise %}
Fill up the value of `name` to validate the condition.
{% initial %}
var name =

if (name === "John") {

}
{% solution %}
var name = "John";

if (name === "John") {

}
{% validation %}
assert(name === "John");
{% endexercise %}

##Exercise 2 `else`

{% exercise %}
Fill up the value of `name` to validate the `else` condition.
{% initial %}
var name =

if (name === "John") {

} else if (name === "Aaron") {
    // Valid this condition
}
{% solution %}
var name = "Aaron";

if (name === "John") {

} else if (name === "Aaron") {
    // Valid this condition
}
{% validation %}
assert(name === "Aaron");
{% endexercise %}



##Exercise 3 `multiple conditions`


{% exercise %}
Fill up the 2 conditions so that `primaryCategory` equals `"E/J"` only if name equals `"John"` and country is `"England"`, and so that `secondaryCategory` equals `"E|J"` only if name equals `"John"` or country is `"England"`
{% initial %}
var name = "John";
var country = "England";
var primaryCategory, secondaryCategory;

if ( /* Fill here */ ) {
    primaryCategory = "E/J";
}
if ( /* Fill here */ ) {
    secondaryCategory = "E|J";
}
{% solution %}
var name = "John";
var country = "England";
var primaryCategory, secondaryCategory;

if (name === "John" && country === "England") {
    primaryCategory = "E/J";
}
if (name === "John" || country === "England") {
    secondaryCategory = "E|J";
}
{% validation %}
assert(primaryCategory === "E/J" && secondaryCategory === "E|J");
{% endexercise %}







