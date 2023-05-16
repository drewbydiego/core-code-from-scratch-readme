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

<h2>Fahrenheit 🤖</h2>
<b>"Write a function toFahrenheit that converts a temperature from Celsius to Fahrenheit.<br><br>

Example: toFahrenheit(0) should return 32."</b>
<h3>Solution</h3>


~~~

  function toFahrenheit(celsius) {
    const fahrenheit = (celsius * 9/5) + 32;
  
    return fahrenheit;
  }

  console.log(toFahrenheit(0));
  
~~~

![image](https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/0bc0e885-66f8-44fe-998e-686be5a72af2)

<h2>Boolean 🤖</h2>
<b>"Write a function nand that takes two Boolean values. If both values are true, the result should be false. In the other cases the return should be true.<br><br>

I.e.: The call nand(true, true) should return false. The calls nand(true, false), nand(false, true) and nand(false, false) should return true.
"</b>
<h3>Solution</h3>


~~~

  function nand(a, b) {
    if (a === true && b === true) {
      return false;
    }

    return true;
  }
  
  console.log(nand(true, true));
  console.log(nand(true, false)); 
  console.log(nand(false, true)); 
  console.log(nand(false, false)); 
  
~~~

![image](https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/1640e4a7-cdb0-460b-b40a-4b98d4c9801a)
