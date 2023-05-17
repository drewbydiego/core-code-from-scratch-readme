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

<h1>Week challenges (Tuesday) 💻</h1>
<h2>Objects 🤖 - Codewars</h2>
<b>"Task Give you a function animal, accept 1 parameter:obj like this:<br><br>

{name:"dog",legs:4,color:"white"}<br>
and return a string like this:<br><br>

'This white dog has 4 legs.'"</b>
<h3>Solution</h3>
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/abf9632a-848b-414f-b04e-87b8294ad0e1" alt="" width="600" height="300">

<h2>Return to sanity 🤖 - Codewars</h2>
<b>"This function should return an object, but it's not doing what's intended. What's wrong?"<br><br></b>

~~~

function mystery(sanity) {
    var results =
      {sanity: 'Hello'};
    return
      results;
  }
  
~~~

<h3>Solution</h3>
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/4fd6f8a2-87a3-4522-8e93-ab09a41b9ebb" alt="" width="600" height="300">

<h2>Object syntax debug 🤖 - Codewars</h2>
<b>"While making a zork-type game, you create an object of rooms. Unfortunately, the game is not working. Find all of the errors in the rooms object to get your game working again."</b>


~~~

var rooms = {
  first: {
    description: 'This is the first room'
    items: {
      chair: 'The old chair looks comfortable',
      lamp: 'This lamp looks ancient'
  },
  second: {
    description: 'This is the second room'
    items: {
      couch: 'This couch looks like it would hurt your back,
      table: 'On the table there is an unopened bottle of water'
    }
  }
}
  
~~~

<h3>Solution</h3>
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/f20aa97f-65b3-41b7-afeb-f68fba7de9fc" alt="" width="600" height="300">

<h1>Week challenges (Wednesday) 💻</h1>
<h2>Count strings in objects 🤖 - Codewars</h2>
<b>"Create a function strCount (takes an object as argument) that will count all string values inside an object. For example:"</b>


~~~

strCount({
  first: "1",
  second: "2",
  third: false,
  fourth: ["anytime",2,3,4],
  fifth:  null
  })
  //returns 3
  
~~~

<h3>Solution</h3>
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/4dc28988-ba45-4401-807f-629652b8efb2" alt="" width="600" height="300">

<h2>Extending JavaScript Objects: Get First & Last Array Element 🤖 - Codewars</h2>
<b>"Your task is to extend JavaScript Array object, with methods .first() and .last(), so you can get respectively first or last element of the array.<br><br>

~~~
    
var a = [2, 5, 7, 3 ,4];

a.first();  // 2
a.last();   // 4
    
~~~
    
Note: in case of empty array, methods should return undefined."</b>


<h3>Solution</h3>
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/4bffcb02-2d05-4afb-b2e2-d3d8f014f586" alt="" width="600" height="300">

<h2>Object Oriented Piracy 🤖 - Codewars</h2>
<b>"You have access to the ship "draft" and "crew". "Draft" is the total ship weight and "crew" is the number of humans on the ship.<br><br>

Each crew member adds 1.5 units to the ship draft. If after removing the weight of the crew, the draft is still more than 20, then the ship is worth looting. Any ship weighing that much must have a lot of booty!"</b>


~~~

function Ship(draft,crew) {
 this.draft = draft;
 this.crew = crew;
}
  
~~~

<h3>Solution</h3>
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/1b309844-8d64-4d2a-a298-7ba366405fc9" alt="" width="600" height="300">

