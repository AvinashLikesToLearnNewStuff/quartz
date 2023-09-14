# JavaScript basics

From MDN docs
## [What is JavaScript?](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics#what_is_javascript)

- Its just a DOM manipulator with some cool effects

## [Language basics crash course](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics#language_basics_crash_course)
### [Variables](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics#variables)
variables - containers that store values

we declare them by using var or let\
like 
`var myVariable;
`
we use semicolons to end our statements. 
These are handy rules as to [[when to use semicolons]] 

Data Types in JS
String 
Number
Boolean
Array
Object
### [Operators](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics#operators)
| name                 | symbol  |
| -------------------- | ------- |
| addition             | +       |
| subtraction          | -       |
| multiplication       | *       |
| division             | /       |
| -------------------  | ------- |
| assignment           | =       |
| not , does not equal | !,!==   |


### [Conditionals](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics#conditionals)
if, else statements
```js

let timePass = "anime";
if (timePass === "anime") {
  alert("Yay, I love anime!");
} else {
  alert("Awwww, but anime is my favorite…");
}

```

### [Functions](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics#functions)

functions are building reusable pieces of code 
some functions are inbuilt and some we build ourselves

functions look like variable names followed by parantheses
they also take arguments, arguments are the things we put inside those parenthesis
like for example if we want to use the alert function we ask the question what do we need to tell the user , we supply what we want to tell the user using the argument taken by the alert function

`alert(the_thing_that_we_want_to_tell_the_user)`

we can define out own function
for that there are many ways but commonly we use the function keyword
example
```js
function loveAnime(anime1){
	alert("I love `${anime1}`");
	return "done";								 
}
```
The return statement takes some value from the function - i.e returns it, and give it to someone else for further processing 

### [Events](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics#events)
Events are the things that happen in a browser like clicking, screen change, element disappear etc

we want to do something when an event fires etc so for that we use event handlers
```js
document.querySelector("html").addEventListener("click", function () {
  alert("Ouch! Stop poking me!");
});
```

the most common way to handle the events is to use `addEventListener()` function
In the code snippet above, we are listening for the click event, 
as soon as we hear  a click event we fire our function


