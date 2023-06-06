<h1>Week #9 challenges</h1>
<h1>Week challenges (Monday) 💻</h1>
<h2>"this" is a problem 🤖 - codewars</h2>
<b>"We want to create a constructor function 'NameMe', which takes first name and last name as parameters. The function combines the first and last names and saves the value in "name" property."</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/491d3f20-f15f-43dd-a801-e6af6d07e75b" alt="" width="600" height="300">

~~~javascript
function NameMe(first, last) {
  this.firstName = first;
  this.lastName = last;
  this.name = this.firstName + ' ' + this.lastName;
}
var n = new NameMe('John', 'Doe');
console.log(n.firstName); // Expected: John
console.log(n.lastName); // Expected: Doe
console.log(n.name); // Expected: John Doe
~~~


<h2>"Thinkful - List and Loop Drills: Lists of lists" 🤖 - codewars</h2>
<b>"You have a two-dimensional list in the following format:<br>
data = [[2, 5], [3, 4], [8, 7]]"</b>
<h3>Solution</h3>
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/41ba0e6b-3051-4719-a0c3-56508abcc661" alt="" width="600" height="300">

~~~javascript
function processData(data) {
  let result = 1;

  for (let i = 0; i < data.length; i++) {
    const subList = data[i];
    const processedValue = subList[0] - subList[1];
    result *= processedValue;
  }

  return result;
}
~~~

<h2>Stop gninnipS My sdroW! 🤖 - codewars</h2>
<b>"Write a function that takes in a string of one or more words, and returns the same string, but with all five or more letter words reversed (Just like the name of this Kata). Strings passed in will consist of only letters and spaces. Spaces will be included only when more than one word is present."</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/8f88ba74-ceb8-4eb5-93c1-906d3d39cc7f" alt="" width="600" height="300">

~~~javascript

function spinWords(string) {
  const words = string.split(' ');

  for (let i = 0; i < words.length; i++) {
    if (words[i].length >= 5) {
      words[i] = words[i].split('').reverse().join('');
    }
  }

  return words.join(' ');
}
~~~

<h1>Week challenges (Tuesday) 💻</h1>
<h2>"this" is an other problem 🤖 - codewars</h2>
<b>"Having created a function NamedOne which takes first & last names as parameters and returns an object with firstName, lastName and fullName ( = firstName + a space + lastName ) properties which should be all accessibles, we discovered that "accessible" also means "mutable"."</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/07d40376-edd6-49be-9d93-c11e465dea75" alt="" width="600" height="300">

~~~javascript

function NamedOne(first, last) {
  let firstName = first;
  let lastName = last;
  let fullName = firstName + ' ' + lastName;

  Object.defineProperty(this, 'firstName', {
    get: function() {
      return firstName;
    },
    set: function(value) {
      firstName = value;
      fullName = firstName + ' ' + lastName;
    }
  });

  Object.defineProperty(this, 'lastName', {
    get: function() {
      return lastName;
    },
    set: function(value) {
      lastName = value;
      fullName = firstName + ' ' + lastName;
    }
  });

  Object.defineProperty(this, 'fullName', {
    get: function() {
      return fullName;
    },
    set: function(value) {
      const nameParts = value.split(' ');
      if (nameParts.length === 2) {
        firstName = nameParts[0];
        lastName = nameParts[1];
        fullName = value;
      }
    }
  });
}
~~~

<h2>Who likes it? 🤖 - codewars</h2>
<b>"You probably know the "like" system from Facebook and other pages. People can "like" blog posts, pictures or other items. We want to create the text that should be displayed next to such an item."</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/663945ac-3d99-4dbd-bb5b-d7123c0018fd" alt="" width="600" height="300">

~~~javascript
function likes(names) {
  const length = names.length;

  if (length === 0) {
    return 'no one likes this';
  } else if (length === 1) {
    return `${names[0]} likes this`;
  } else if (length === 2) {
    return `${names[0]} and ${names[1]} like this`;
  } else if (length === 3) {
    return `${names[0]}, ${names[1]} and ${names[2]} like this`;
  } else {
    const remainingCount = length - 2;
    return `${names[0]}, ${names[1]} and ${remainingCount} others like this`;
  }
}
~~~

<h2>Convert string to camel case 🤖 - codewars</h2>
<b>"Complete the method/function so that it converts dash/underscore delimited words into camel casing. The first word within the output should be capitalized only if the original word was capitalized (known as Upper Camel Case, also often referred to as Pascal case). The next words should be always capitalized."</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/3666c53b-8288-4362-b372-2599d2f45e32" alt="" width="600" height="300">


~~~javascript
function toCamelCase(str) {
  var words = str.split(/[-_]/); 
  
  var camelCase = words.map(function(word, index) {
    if (index === 0) {
      return word; 
    } else {
      return word.charAt(0).toUpperCase() + word.slice(1); 
    }
  });
  
  return camelCase.join(''); 
}
~~~

<h1>Week challenges (Wednesday) 💻</h1>
<h2>Easy mathematical callback 🤖 - codewars</h2>
<b>"Write the processArray function, which takes an array and a callback function as parameters. The callback function can be, for example, a mathematical function that will be applied on each element of this array. Optionally, also write tests similar to the examples below."</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/457af742-bf23-4be4-825f-2e5e5698d811" alt="" width="600" height="300">

~~~javascript
function processArray(arr, callback) {
  return arr.map(callback);
}

~~~

<h2>Moving Zeros To The End 🤖 - codewars</h2>
<b>"Write an algorithm that takes an array and moves all of the zeros to the end, preserving the order of the other elements."</b>
<h3>Solution</h3>
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/9c0ba659-af25-49c5-ac3b-81d9d3ec4f6c" alt="" width="600" height="300">

~~~javascript
function moveZeros(arr) {
  var result = [];
  var count = 0;

  for (var i = 0; i < arr.length; i++) {
    if (arr[i] !== 0) {
      result.push(arr[i]);
    } else {
      count++;
    }
  }

  for (var j = 0; j < count; j++) {
    result.push(0);
  }

  return result;
}

~~~

<h2>Valid parentheses 🤖 - codewars</h2>
<b>"Write a function that takes a string of parentheses, and determines if the order of the parentheses is valid. The function should return true if the string is valid, and false if it's invalid."</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/4de77c63-ef3d-4e32-8e27-01c9586fff41" alt="" width="600" height="300">

~~~javascript
function validParentheses(parens) {
  var stack = [];
  for (var i = 0; i < parens.length; i++) {
    var char = parens[i];
    if (char === '(') {
      stack.push(char); 
    } else if (char === ')') {
      if (stack.length === 0) {
        return false; 
      }
      stack.pop(); 
  }
  return stack.length === 0; 
}
~~~

<h1>Week challenges (Thursday) 💻</h1>
<h2>The Hashtag Generator 🤖 - codewars</h2>
<b>"The marketing team is spending way too much time typing in hashtags.
Let's help them with our own Hashtag Generator!"</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/93cda4a7-3be2-4cbf-8b70-487fff64ba65" alt="" width="600" height="300">

~~~javascript
function generateHashtag(str) {
  var trimmedStr = str.trim();

  if (trimmedStr === '') {
    return false;
  }
  var words = trimmedStr.split(' ');
  var capitalizedWords = words.map(function(word) {
    return word.charAt(0).toUpperCase() + word.slice(1);
  });
  var hashtag = '#' + capitalizedWords.join('');
  if (hashtag.length > 140) {
    return false;
  }
  return hashtag;
}
~~~

<h2>String incrementer 🤖 - codewars</h2>
<b>"Your job is to write a function which increments a string, to create a new string.<br><br>

If the string already ends with a number, the number should be incremented by 1.<br>
If the string does not end with a number. the number 1 should be appended to the new string."</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/979e5849-6b04-4d1b-ba32-b41281ff196c" alt="" width="600" height="300">

~~~javascript
function incrementString(strng) {
  var numericPart = strng.match(/\d+$/); 

  if (numericPart === null) {
    return strng + '1';
  }

  var numericString = numericPart[0];
  var numericPartLength = numericString.length;

  var incrementedNumber = (parseInt(numericString, 10) + 1).toString(); // Increment the numeric part

  while (incrementedNumber.length < numericPartLength) {
    incrementedNumber = '0' + incrementedNumber;
  }

  var nonNumericPart = strng.substring(0, strng.length - numericPartLength);

  return nonNumericPart + incrementedNumber;
}
~~~

