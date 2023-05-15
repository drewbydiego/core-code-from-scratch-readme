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


<h1>Week challenges (Thursday) 💻</h1>
<h2>Strings 🧵</h2>
<b>"Write a function greet having one parameter and returning 'Hello <parameter>!'.<br><br>

Example: greet('Ada') should return 'Hello Ada!' and greet('Grace') should return 'Hello Grace!'."</b>
<h3>Solution</h3>

    
~~~

    
"use strict";

function greeting(x) {
    return 'Hello ' + x;
  }

  console.log(greeting("Diego"));


~~~
    
![image](https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/b1cea5f5-4a4f-4b0d-884d-288b3f128248)

 <h2>String: length 🧵</h2>
<b>"Write a function length that takes a string and returns the number of characters of the string.<br><br>

Example: length('sun') should return 3."</b>
<h3>Solution</h3>

    
~~~

    
"use strict";

function getLength(x){
    return x.length;
}

console.log(getLength("Diego Flores"));


~~~
    
![image](https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/88469e46-47f2-4c7a-9a6b-4753e535464f)

 <h2>String: toUpperCase() 🧵</h2>
<b>"Write a function toCase that takes a string and returns that string in lowercase and uppercase with - as delimiter.<br><br>

Example: toCase('Mthatha') should return 'mthatha-MTHATHA'."</b>
<h3>Solution</h3>    

~~~

    
"use strict";

function toCase(x) {
    return x.toLowerCase() + ' ' + x.toUpperCase();
  }

  console.log(toCase("diego"));


~~~
    
 ![image](https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/007b5a70-4a76-48c5-8479-92ca393e44f7)

    
<h2>String: charAt() 🧵</h2>
<b>"Write a function shortcut that takes two strings and returns the initial letters of theses strings.<br><br>

Example: shortcut('Amnesty', 'International') should return 'AI'."</b>
<h3>Solution</h3>    
    
~~~

    
"use strict";

  function scut(text1, text2) {
    return text1.charAt(0) + text2.charAt(0);
  }

  console.log(scut("Diego", "Flores"));

~~~
    
 ![image](https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/38a63168-8e7d-4930-9261-bae9c7254804)
   
<h2>String: indexOf() 🧵</h2>
<b>"Write a function indexOfIgnoreCase taking two strings and determining the first occurrence of the second string in the first string. The function should be case insensitive.
<br><br>
Example: indexOfIgnoreCase('bit','it') and indexOfIgnoreCase('bit','IT') should return 1."</b>
<h3>Solution</h3>     
    
~~~

    
"use strict";

  function indexOfIgnoreCase(str1, str2) {
    const lowercaseStr1 = str1.toLowerCase();
    const lowercaseStr2 = str2.toLowerCase();
    return lowercaseStr1.indexOf(lowercaseStr2);
  }
  
  console.log(indexOfIgnoreCase('bit', 'it')); 

~~~
    
 ![image](https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/64e269f3-fcf9-47b0-a619-5a35781a6789)
   
