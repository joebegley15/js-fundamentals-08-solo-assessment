![General Assembly Logo](http://i.imgur.com/ke8USTq.png)

# Assessment for JavaScript Fundamentals

You have 20 minutes

## Instructions

Fork, clone, and npm install.

Follow the prompts below and complete each question.  You may use any resource, other than someone else in the classroom, to help you complete this assessment.

You should save your answers in this README.md file.

# Question 1

```js
var a = 2;
var b = 3;
a = b;
```

After this code executes, what are the values of a and b? Please explain your answer.

After this code executes a will be equal to b, so a = 3 and b = 3.

## Question 2

```js
var c = 5;
var d = 2;
c = c + d;
```

After this code executes, what is the value of c?  Please explain what the last line of this program `c = c + d;` means.

After the code executes d = 2 and c = 7. The line 'c = c + d' means that c's new value is itself plus the value of d.

## Question 3

```js
var x = 4;
var y = 3;
x = y;
y = 10;
```

After this code executes, what are the values of x and y?  Please explain your answer.

After the code executes x = 3 and y = 10. This is true because originally y = 10 and x takes on this value when the command x = y takes place. Then y = 10 overrules everything and y = 10.

## Question 4

```js
var weather;
weather = "sunny";
weather === "sunny";
```

What are the values of these expressions?  Explain your answers.

In line 1 we create the variable weather, which is still undefined. Weather now has a value of undefined.
In line 2 we give the variable a value of "sunny". The variable weather is now now sunny.
In line three we are asking if the weather is in fact sunny, and based on the the previous two lines this is true. Therefore, the value returned is true.

## Question 5

```js
var howMuchILikeSushi = 2;

if (howMuchILikeSushi >= 3) {
  console.log("sushi is delicious");
}

if (x > 0) {
  console.log("sushi is tasty");
}
```

Imagine that you take the code from this question, save it to a file called `food.js`, and run `node food.js` in your Terminal.

What would be the output? Explain your answer.

We'll get an error. The reason for that error is quite simple. In order to get a log of "sushi is delicious" how much I like sushi needs a value of at least 3, but its a 2, so its skips it. At this point we should have another option for when howMuchILikeSushi is less than 3, but we don't because we've used an undefined variable called x instead of howMuchILikeSushi. This would be a better replacement for that pience of code:

if (howMuchILikeSushi > 0) {
  console.log("sushi is tasty");
}


## Question 6

```js
var howMuchILikeSushi = 2;

if (howMuchILikeSushi > 0) {
  console.log("sushi is tasty");
} else if (x >= 3) {
  console.log("sushi is delicious");
} else {
  console.log("I don't like sushi");
}
```

Imagine that you take the code from this question, save it to a file called `sushi.js`, and run `node sushi.js` in your Terminal.

What would be the output? Explain your answer.

The output would be "sushi is tasty" because we would satisfy the conditions to the first if statement. I would rewrite this code because a person who likes sushi at a value of 5 would only get "sushi is tasty", not "sushi is delicious".

```js
//We'll learn about require later in the course
var ask = require('./ask.js');

var answer = 'not empty';

while (answer !== '' && answer !== 'SeCrEt') {
  answer = ask("Guess my secret? ");
}
```

Imagine that you take the code from this question, save it to a file called `name.js`, and run `node name.js` in your Terminal.

What would you have to type to exit the while loop?  Explain your answer.

You could type in SeCrEt or not type in anything at all and you would get out of the loop. The key here is the ! value because that is a negative, anything but those two values would keep you in the loop.

---

Commit and push your changes.

Submit a pull request.
