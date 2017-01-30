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

3) **Optional** copy and past the isMorningAfternoon function into last weeks clock exercise and use display it to append AM or PM to the end of the time. 


4) **Optional** Create a function `convertTime`, this function should covert the time to a 12 hour clock and should be called before you append AM or PM.