#Basic javaScript Form Validation

Using javascript to validate web form entries **before** that information is sent to the server is an effective way to maintain data integrity. 

In order to perform basic form validation we need to introduce a few new concepts.    


##Listening For A Form Submission Event 
Hopefully, you remember that a powerful feature of [javaScript is the ability to react to events](https://sirus21.gitbooks.io/internet_technology_block_2/content/session13/event_listener.html). A very useful event for form validation is to listen to a submission event. We do this by implement the `submit` event listener. 

```javascript 
	 //add event listener to a form with a id of ourForm 
    var myForm = document.getElementById("ourForm");
    //the validateForm function will be called when the form submits 
    myForm.addEventListener("submit", validateForm);
```

Above, we call the function validateForm when the form with an id of `ourForm` is submitted. 


##Accessing Form Text Fields 
In-order to validate a form we need to actually access its values. Consider the following simple form:

```html
<!doctype html>
<html>
    <head>

    </head>
    <body>
        <form id="demoForm" action="results.html" method="get">
            <input type="text" name="userName" placeholder="enter name">
            <input type="button" value="go">  
        </form>
    </body>
</html>    
```
Here's how we'd access the userName field, using javaScript:

```java
//get a reference to the form and save it in the var form 
var form = document.getElementById("demoForm");
//grab the value of userNameTextBox
form.userName.value;  // will equal the value entered into the text field usrName
```

**Note**, we reference the text fields `name` attribute (userName) in oder to get the value of the form field. 

##Checking if there is a value in  a text field 

**Above** we showed you how to accesses the value of a text field. Checking that the value is not empty is easy:

```java
	if(form.userName.value == ""){
  		//form field is blank take action 
	}
```
	

##Hiding and Displaying Error Messages

Hopefully, it's fairly obvious that having the ability to hide and display error messages would be useful for form validation. Below is an example on how to display and then hide a paragraph element.  

**html**

```html
<p id="errorName"> Required </p>  
```

**java script**

```javascript
//hide p element 
document.getElementById("errorName").style.display = "none";
//display p element  
document.getElementById("errorName").style.display = "block";
```


##Preventing a Form Submitting 

A form is submitted to the server when the submit button is pressed. However, if there are errors in the form we want to prevent this from happening.  

In order to do this, we can access the submit button event and instruct it to prevent the default behaviour of submitting.  The instruction is placed in the `onSubmit` callback function. 

Assuming `validateForm` is  our callback function, below is how we'd prevent the form from submitting:

```javascript
function validateForm(event){
	  event.preventDefault();
}
```
Observe how we add the parameter `event` in the callback function. We can then prevent its default submission behaviour. 







  

 