## TCA - Common Issues

### Using empty elements to create space

It's often tempting to use empty HTML elements in order to create space within an HTML document.

Consider the following **incorrect** example:

```javascript
...
<body>
    <h1>  This is a heading </h1>
    <!-- incorrectly using empty <p> tags in order to create space -->
    <p></p>
    <p></p>
    <p> This is my paragraph </p>

</body>
...
```

In the above example we are using empty `<p>` elements in order to create space. This is very bad practice, as adding unnecessary elements makes HTML pages unwieldy and hard to maintain. Furthermore, we can no longer fully control the look and feel of our page using our external style sheet.

Rather than using empty elements we should instead use CSS to create space. Within our css file we could add the following:

```javascript
    h1 { 

        margin-bottom: 50 px;

    }
```

### Not changing the display style of the image on the front page

One of the tasks to be completed on `index.html` was to insert and image such that it lives on it's own line. Many of you wrapped the `<img>` element in a `<div>` or a `<p>` to achieve this. This is bad as we're adding unnecessary elements.

The correct solution was to display the layout of the image from block to inline using css:

**html**

```
<img class="my_image" src="img/image1">
```

**css**

```
.my_image{
    display:block
}
```


If we want text to flow around the image we can simply float it:

```
.my_image{
	float:left;
}



### Validation errors

There's really no excuse here. For our client side scripting assignment  you should all make sure that your HTML is 100% valid using the W3C validator.

### Invalid Links

Always make your links portable. Many of you constructed links that would only work on your local computer:

**Good**

```
<a href="session1/index.html"> Index Page </a>
```

* Use `/` for the path
* Link relative to the the location 
* No spaces in the folder or file name 

**Bad**

```
<a href="C:\mydocument\session1\index file.html"> Index Page </a>
```

* An absolute reference to the c drive on my computer 
* `\` used
* Space in the file name

### Failure to include a unique meta description

Each page should have a meta description within the `<head>`. It's a vital element for SEO:

```html
     <meta type = "description" content="This is a meta description ">
```

### Commenting

Be sure to use intuitive commenting for the next assessment.  
**As a minimum you should comment at:**

* The end of each div:  

```html
<div id="myDiv">
 ... 
</div> <!-- [END]#myDiv -->
```

* At the top of each page (optional), but helps me mark:

```html
<!-- 
    name: Joe Appleton 
    version: 1
    date: 11/01/2016
-->
```


### Unable to layout the form

Many of you struggled to lay out the form.  You'll need to do this for the next client side scripting assessment assignment. 

You can follow a simple process when it comes to laying out forms:

1) Create the form, using `<p>` tags to create separate lines:

```
<form action="post" id="myForm">

  <p><label for="name">Name<input type="text" name="name" id="" /></label></p>
  <p><label for="age">Age<input type="text" name="age" id="" /></label></p>
  <p><label for="">Location<input type="text" name="location" id="" /></label></p>
  
  <input type="submit" value="submit" name="" id="" />

</form>
```

2) Constrain the width of the form:

```
form{
  width:200px;
  border: 1px solid red;
  padding: 2%;
}

```

3) Float the text inputs to the right 

```  
<input type="submit" value="submit" name="" id="" />
```



### Failure to follow the specification

Many of you lost easy marks for simply not following the specification. Make sure you read assessment2 carefully, covering all the main points.




