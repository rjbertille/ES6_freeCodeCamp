# ES6_freeCodeCamp

Explore Differences Between the var and let Keywords

One of the biggest problems with declaring variables with the var keyword is that you can overwrite variable declarations without an error.

var camper = 'James';<br>
var camper = 'David';<br>
console.log(camper);<br>
// logs 'David'
As you can see in the code above, the camper variable is originally declared as James and then overridden to be David.<br>

In a small application, you might not run into this type of problem, but when your code becomes larger, you might accidentally overwrite a variable that you did not intend to overwrite.<br>

Because this behavior does not throw an error, searching and fixing bugs becomes more difficult.<br>

A new keyword called let was introduced in ES6 to solve this potential issue with the var keyword.<br>

If you were to replace var with let in the variable declarations of the code above, the result would be an error.<br>

let camper = 'James';<br>
let camper = 'David'; // throws an error <br>
This error can be seen in the console of your browser.<br>

So unlike var, when using let, a variable with the same name can only be declared once.<br>

Note the "use strict". This enables Strict Mode, which catches common coding mistakes and "unsafe" actions. For instance:<br>

"use strict";<br>
x = 3.14; // throws an error because x is not declared <br>

Update the code so it only uses the let keyword.<br>

- var does not exist in code.<br>

- catName should be Oliver<br>

- quote should be "Oliver says Meow!"<br>

<strong>let catName;</strong><br>
<strong>let quote;</strong><br>
<strong>function catTalk() {</strong><br>
<strong>"use strict";</strong><br>
<strong>catName = "Oliver";</strong><br>
<strong>quote = catName + " says Meow!";</strong><br>
<strong>}</strong><br>
<strong>catTalk();</strong><br>
//Run the test<br>
