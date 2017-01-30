#Functions in javaScript 

We've already seen and used javaScript functions is this course. Let's take the opportunity at this stage to look into them in a little more depth.  

* Functions are named collections of statements
* javaScript has built-in functions, and you can write your own
* For example parseInt() parses a string and returns an integer

	```javascript 
	   //this is not a number it's a string , as it's in "" marks 
	   var firstNumber = "12"; 	  
	   //number1 will hold the numeric value 12
	   number1 = parseInt(firstNumber); 	   
	
	```
*  A function contains code that will be executed by an event or by a call to the function


##How To Define A Function 

```javascript
 function functionName(var1, var2, ...)
 { //some code;
 }

```

**Function's can also return values**

```javascript
function numberProduct(num1, num2) {
   var result = num1 * num2;
   return result;

}

var product = numberProduct(2,4);
console.log(product); // will output 8 to the console

```

* The parameters num1 and num2 are variables or values passed into the function. You can have as many parameters as you like.
* A function with no parameters must still include `( )` after the function name
* The word `function` must be written in lowercase letters in your code 
* You must call a function with the exact same capitals as in the function definition