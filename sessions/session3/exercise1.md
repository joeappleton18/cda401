#Pre Exercise 

Ensure that you've completed the in note exercises before you start the main exercises for the week:

- [Conditions](https://sirus21.gitbooks.io/cda401/content/sessions/session3/conditional_statements.html)
- [Functions](https://sirus21.gitbooks.io/cda401/content/sessions/session3/functions.html)	




#Exercise 1 - Time Function
1) Create an `.html` document called `exercise1.html`

2) Include and external javaScript file called `exercise1.js` to use for this exercise. Add a `onload= main()` to the `<body>` tag of your html file. 


2) Within `exercise1.js` Define a function called `isMorningAfternoon` that takes in one parameter `hours` 

If `hours` is bigger than or equal to 12  the function should return **PM**    
If `hours` is smaller than 12 the function should return **AM**


```javascript


function isMorningAfternoon(hours) {
	//your code goes here
}

function main(){
	console.log(isMorningAfternoon(12));  //will return PM
	console.log(isMorningAfternoon(13)); // will return PM
	console.log(isMorningAfternoon(9)); // will return AM 
}
```

3) Copy and past the isMorningAfternoon function into last weeks clock exercise and use display it to append AM or PM to the end of the time.
**Note**, if you have not completed last weeks exercise, [please find the solution here](https://github.com/sirus21/Internet_technology/tree/master/session13_solution)
 


4) Create a function `convertTime`, this function should covert the time to a 12 hour clock and should be called before you append AM or PM.


#Exercise 2  - A Guessing Game



#Set Up 

1) Within a new folder create the following files:

	- js/main.js 
	- index.html
2) Within `main.js` create a function called `main`, for now it will just have one line of code in it `alert('working')`

3) Within `index.html`s body tag, add a inline load even that calls the function `main`.   `<body onload="main">`

#Task 

The aim of the task this week is to create a number guessing game. Your program will generate a number between a user defined range. The user will then make guesses with the aim of finding that number. Feedback will be given on if the guess is:

- Smaller than the number
- Larger than the number 
- An exact match! 

1) Add the following elements to `index.html` and give them `id`'s where appropriate:


- An input and label for the guess 
- A `<button>Click Me </button>` that will be pressed after the guess 
- A paragraph to hold the result 


2) At the top of your javascript file create vars to hold the following values: 
	
	- random_number 
	- number_of_guesses
	
3) `Math.round(Math.random() * (20 - 10) + 10);`  generates a random number between 20 and 10. The formula looks like this `Math.round(Math.random() * (max - min) + min);`.  Create a function `getRandomArbitrary(min, max)` which returns a random number between any given range.  


4) Set `random_number` equal to a random number by using the above function. This should be done in `main()` which is called when the page has loaded
 
5) Using **external javescript** add a click event to the button that runs a guess function. 

6) Write the guess function, it should grab the the [user input](notes.md#accessing-the-dom) and run some [comparisons](notes.md/#conditional-statements) and adjust the `inner_html` value of your paragraph to display the information based on the guess. 

7) **Advanced** set up a variable called `var number_of_guesses = 10`, decrement this variable on each guess. If the user runs out of guesses it's game over. The inputs should then be hidden. 



