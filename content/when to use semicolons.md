reference - https://www.codecademy.com/resources/blog/your-guide-to-semicolons-in-javascript/
#### Required: When two statements are on the same line
example var l = 0 ; i ++ <-- semicolon obligatory 
example var l = 0  <-- semicolon optional
i ++ <-- semicolon optional

#### Optional: After statements

The semicolon in JavaScript is used to separate statements, but it can be omitted if the statement is followed by a line break (or there’s only _one_ statement in a `{`block`}`).
A statement means 1 like which tells the computer to do something 
examples 
```js
var 2;
i = 6;
i = 2 + 2;
var x = 1;
var fun = function(){...};
alert("yu");
```
In all these statements semicolon is optional.

#### Avoid!
**1. After a closing curly bracket**
We shouldn’t put a semicolon after a closing curly bracket `}`. The only exceptions are _assignment statements_, such as `var obj = {};`, see above.

```
// NO semicolons after }:
if  (...) {...} else {...}
for (...) {...}
while (...) {...}

// BUT:
do {...} while (...);

// function statement: 
function (arg) { /*do this*/ } // NO semicolon after }
```

**2. After the round bracket of an if, for, while or switch statement**
never put semicolon after the round bracket of a for statement etc
example 
`for (i=4;i<3;i++;);`

the example from codeacademy site

```
if (0 === 1); { alert("hi") } // equivalent to: if (0 === 1) /*do nothing*/ ; alert ("hi");
```
but we can put ; in the inside of a () in a for loop after - just not after the first statement
we can write 
example 
`for (i=4;i<3;i++)`
but not
example 
`for (i=4;i<3;i++;)`

To fix unnessacary semicolons they recommended using jslint

[[A Quick Review]]