<h1>Week #7 challenges</h1>
<h1>Week challenges (Monday) 💻</h1>
<h2>String: substr() 🤖</h2>
<b>"Write a function firstWord, taking a string and returning the first word in that string. The first word are all characters up to the first space.<br><br>

Example: firstWord('see and stop') should return 'see'."</b>
<h3>Solution</h3>


~~~

"use strict";

function firstWord(str) {

    const firstSpaceIndex = str.indexOf(' ');

    const firstWord = str.substring(0, firstSpaceIndex);
  
    return firstWord;
  }


  console.log(firstWord('see and stop')); 
~~~

![image](https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/ae2b963d-398d-4ef6-bd79-e90b042e916b)

<h2>String: replace() 🤖</h2>
<b>"Write a function normalize, that replaces '-' with '/' in a date string.<br><br>

Example: normalize('20-05-2017') should return '20/05/2017'."</b>
<h3>Solution</h3>

~~~

  function normalize(string) {

    return normaldata = string.replace(/-/g, '/');
  }

  console.log(normalize('20-05-2017')); 
  
  
~~~

![image](https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/5a40e469-dce2-42cf-9520-6d0efb603bea)

<h2>Increment 🤖</h2>
<b>"Which value does x have after execution of the following code?<br>
let x = 3;<br>
x++;<br>
x = x * 2;<br>
x--;"</b>
<h3>Solution</h3>


~~~

x = 7
~~~

<h2>String: substr() 🤖</h2>
<b>"Write a function firstWord, taking a string and returning the first word in that string. The first word are all characters up to the first space.<br><br>

Example: firstWord('see and stop') should return 'see'."</b>
<h3>Solution</h3>


~~~


~~~
