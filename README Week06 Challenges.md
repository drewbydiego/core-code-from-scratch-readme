<h1>Week #6 challenges</h1>
<h1>Week challenges (Tuesday) 💻</h1>
<h2>Variables 🤖</h2>
<b>"Declare a variable firstname and initialize it with the value 'Lata'."</b>
<h3>Solution</h3>


~~~

"use strict";

let firstname;
firstname = 'Lata';

~~~


<h2>What is x? X</h2>
<b>"Which value does x have after execution of the following code?
<br>let x = 'Geeta';"</b>
<h3>Solution</h3>


~~~

'Geeta'

~~~

<h2>Several variables 🥋🏻</h2>
<b>"Several variables are declared and initialized in 2 program lines:<br>
let city = 'Lubumbashi';<br>
let country = 'Congo';<br><br>
Declare a variable flower and assign it the value 'rose'. Declare a second variable tree and assign it the value 'maple'."</b>
<h3>Solution</h3>


~~~
"use strict";

let flower = "rose";
let tree = "maple";
~~~

<h2>Reassignment 🥋</h2>
<b>"Which value does x have after execution of the following code?
let x = 'Tic';<br>
x = 'Tac';<br>
x = 'Toe';"</b>
<h3>Solution</h3>


~~~
'Toe'
~~~

<h2>Assign variables 🥋</h2>
<b>"Which value does x have after execution of the following code?
let x = 'Laurel';<br>
let y = 'Hardy';<br>
let z = y;<br>
y = x;<br>
x = z;"</b>
<h3>Solution</h3>


~~~
'Hardy'
~~~


<h1>Week challenges (Wednesday) 💻</h1>
<h2>Functions 🏌🏻‍♂️</h2>
<b>"Define a function hello that returns 'Hello world!'."</b>
<h3>Solution</h3>

~~~
"use strict";

function hello() {

    return "Hello World!"
}

console.log(hello());
~~~

![image](https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/1b941ac2-f91d-486c-87b5-925ecdc6e3b9)


<h2>Multiple functions 🤹🏻</h2>
<b>"Define two functions. The first function a should return 'Hello a!' and the second function b should return 'Hello b!'."</b>
<h3>Solution</h3>

~~~
"use strict";

function a() {
    return 'Hello a!'
}

function b() {
    return 'Hello b!'
}

console.log(a());
console.log(b());
~~~

![image](https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/3f27423a-7b50-4a49-94e9-58d1c0b403cc)


<h2>Function calls📱</h2>
<b>"1. Define a function greet returning the value 'Haydo!'.<br>
2. Declare a variable salutation. Call the function greet and assign the result of the call to the variable salutation."</b>
<h3>Solution</h3>

~~~
"use strict";

let salutation;
salutation = greet();

console.log(salutation);

function greet(){

    return 'Haydo!';
}

~~~

<h2>What is x? (function version)</h2>
<b>"Which value does x have after execution of the following code?<br>
function reply(phrase) {
  return phrase;
}

let x = reply('How do you do?');"</b>
<h3>Solution</h3>

~~~
'How do you do?'

~~~

<h2>Parameters 📴</h2>
<b>"Write a function echo that also returns the passed parameter. echo('Greta') should return 'Greta' and echo('CO2') should return 'CO2'"</b>
<h3>Solution</h3>

~~~
function echo(p) {
    return p;
}

console.log(echo('Greta'));
console.log(echo('CO2'));


~~~


![image](https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/90d15c5a-03f1-4eb0-a5bd-aa32f655d647)
