#Exercise 2 - Form Validation

The idea of this exercise is to introduce how to perform basic form validation in an incremental fashion.  The process has been broken down intosteps,  you'll tutor will demo straight the solution to each step after the allotted time. If you're not in the lesson the entire solution will be available in next weeks notes. 


## 1 Set up folder structure and blank files (~3 mins)
Having an organised file structure is vitally important. Luckily, it's also very easy to achieve

With in a new folder create the following project structure:

![file_structure](img/file_structure.png)

## 2 Create a form  (~5 mins)

Within index.html create a new form with the following `<input type="text"` fields:


|field name| 
|----------|
|name      | 
|age       | 
|location  |

For the sake of this example let's assume all the fields are required. Beneath each input place a `<p>` element containing the error message to be displayed if the above input is not filled in. 

**Note** each `<p>` element should have a unique `id` attribute  e.g. 

```html
 <p id="errorName"> Required </p>  
```

At this stage your error messages will be on permanent display.


![form_error](img/html_sample.png)



## 3 Create the `<body>` `onLoad()` event (~3 mins)

1) Within the `<head>` of your  `index.html` page include your javaScript file. 

2) Add a `onload` attribute within your html file's `<body>` tag that calls the `main()` function within your javaScript file. 

3) Create a `main()`  function in your javaScript file and to test it's being called when you html file loads add `console.log("in main function")` in your `main()` function.

If all is good you should see "in main function" within the console tab in developer tools:

![console](img/console_window.png)


## 4 Add a `submit` event  to your form (~5 mins)
Add a submit event to your form that calls a function called `function validateForm(event)`. Within the function `validateForm` add the two lines:

```html
console.log("validating from");
event.preventDefault(event);
```
Press the submit button and check that validate form is printed to the console. 

## 5 Hide the error messages  (~10 mins)

1) Create a a new function called `hideErrors()`, this function will hide each error message. There are 3 error messages so your function will have 3 instructions. 

2) Call  `hideErrors()` in the `main()` function so the errors are not displayed when the html page loads. 


## 6 Validate the Form On Submit (~20 mins)
Ok, we're nearly there, we just need to actually validate the form when it is submitted. The logic to perform this will be placed in the `validate_form` function. Below is the pseudocode. Pseudocode is a  informal language that allows us to design functionality of our programs. 
   
		function validate_form 
			Hide all errors 
			Initialise form_valid to true
			if name empty
		        set form_valid to false 
		        display name error 
		   if location empty
		        set form_valid to false 
		        display location error 
		    if age empty
		        set form_valid to false 
		        display age error 
		     
		    if form_valid  == false 
		    		prevent form from submitting 
		    		
		  
Implement the above functionality using javaScript.         