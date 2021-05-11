---
layout: post
title:      "Ternary Operators ( ? : )"
date:       2021-04-27 18:06:01 -0400
permalink:  ternary_operators
---

Upon completion my final portfolio project, My Plate, a React-Redux web application with a Rails-API backend, I really enjoy working with ternary operators again. I was introduced to them during the first module of our curriculum. Maybe this blog is to convince you to appreciate these simple little things as well! So..why ternary operators ```( ? : )```?


Let’s review what a ternary operator is.  My definition is it’s a simplified ` if/else` statement. But a more technical way to define it is that it is a comparison operator used in the context of if and else statements. 

A regular ` if/else` statement works like this:

```
If  conditional?
	action_if_true
else
	action_if_false
```

A ternary statement can bring this whole code onto one line with the following format:

`conditional ? action_if_true : action_if_false`

One of my first favorite things about ternary operator is that it is just easy on the eyes! Left to right, just like reading a sentence! A regarular` if/else` statement may require a warm up exercise for the poor eyes…left to right over and over in a downward motion and still digesting the logic! 

The ternary operorator is excellent for ` if/else` statements, however if you do have an ` else if ` in your code however, ternary will not be the best option for you. 

Lets look at an example from my project where I used the ternary operator
In my ` MealCard.js` Component, I have this line in my return value:

`<h2>{meal ? meal.location : null}</h2>`

What is ` meal`? If you ` console.log(meal)` in this file, you will see it is a meal object, below is an example:

`{id: 1, img_src: "https://order.superica.com/superica/images/superica/menuCategories/1400_1408_10.png?id=10", location: "Superica Buckhead", caption: "The best enchiladas!!🤤"}`

This line of code is saying, if `meal` is true? Render `meal.location` else `null`, which means the absence of value. 

The regular ` if/else` statement(pseudocode) can read:

```
If meal?
	Return meal.location
Else
	Null
```
		
There you have it..another example where 4 lines of code can be written in one. 
 I love the simplicity of the ternary operator and enjoyed incorporating it in my final project. 
 
 Cheers!
 
 https://github.com/Kiki1022/my-plate-backend.git
 https://github.com/Kiki1022/my-plate-frontend.git
 

