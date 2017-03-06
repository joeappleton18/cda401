#Simple form Validation Example
Let's tie together the form validation concepts with a very simple example.


>> html 

```html
<!doctype html>
<html>
    <head>
         <title> Our Form Validation Example </title>
         <script  type="text/javascript"  src="script/main.js"></script>
    </head>
    <body onload="main()">
        
        <form id="login">
            
            <p><input type="text"  name="userName" placeholder="name"></p>
            <p id="userNameRequiredError" style="display: none">  Required </p>
            <p><input type="password"  name="password" placeholder="password"></p>
            <p id="passwordRequiredError" style="display: none">  Required </p>    
            <input type="submit">       
        </form>
        
    </body>
</html> 

```

>> javascript 

```javascript

 //onload callback function
 function main() {
    
    console.log("in main function");
    var myForm  = document.getElementById("login");
    myForm.addEventListener("submit",validateForm);
  }
  
  //validate callback function 
  function validateForm(event) {
    var formValid = true;
    var myForm = document.getElementById("login"); 
    
    if (myForm.userName.value == "") {
        formValid = false;
        //display error message 
        document.getElementById("userNameRequiredError").style.display = "block";
        //stop form from submitting
        event.preventDefault();
    } else {
        
         document.getElementById("userNameRequiredError").style.display = "none";
    }
    
    if (myForm.password.value == "") {
        formValid = false;
        //display error message 
        document.getElementById("passwordRequiredError").style.display = "block";
        //stop form from submitting
        event.preventDefault();
    } else {
        
         document.getElementById("passwordRequiredError").style.display = "none";
    }
     
  }
```   