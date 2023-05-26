<h1>Week #8 challenges</h1>
<h1>Week challenges (Monday) 💻</h1>
<h2>Training JS #7: if..else and ternary operator! 🤖 - codewars</h2>
<b>"Complete function saleHotdogs/SaleHotDogs/sale_hotdogs, function accepts 1 parameter:n, n is the number of hotdogs a customer will buy, different numbers have different prices (refer to the following table), return how much money will the customer spend to buy that number of hotdogs.
  "</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/ed927a47-06d0-4502-8554-a2db335294e0" alt="" width="600" height="300">

~~~

function saleHotdogs(n) {
  if (n < 5) {
    return n * 100;
  } else if (n >= 5 && n < 10) {
    return n * 95;
  } else {
    return n * 90;
  }
}

~~~


<h2>Training JS #8: Conditional statement--switch 🤖 - codewars</h2>
<b>"Complete the function howManydays. It accepts 1 parameter month, which means the month of the year. Different months have a different number of days as shown in the table below. Return the number of days that are in month. There is no need for input validation: month will always be greater than 0 and less than or equal to 12.
  "</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/ad0b2cfa-f740-4dbc-9ee2-74b0d8725bf0" alt="" width="600" height="300">

~~~

function howManydays(month) {
  var days;
  switch (month) {
    case 1:
    case 3:
    case 5:
    case 7:
    case 8:
    case 10:
    case 12:
      days = 31;
      break;
    case 4:
    case 6:
    case 9:
    case 11:
      days = 30;
      break;
    case 2:
      days = 28;
      break;
  }
  return days;
}


~~~



<h2>Basic calculator 🤖 - codewars</h2>
<b>"Write a function called calculate that takes 3 values. The first and third values are numbers. The second value is a character. If the character is "+" , "-", "*", or "/", the function will return the result of the corresponding mathematical function on the two numbers. If the string is not one of the specified characters, the function should return null (throw an ArgumentException in C#).
  "</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/c335462c-b432-494f-a277-31463789dc3c" alt="" width="600" height="300">

~~~

function calculate(num1, operation, num2) {
  switch (operation) {
    case "+":
      return num1 + num2;
    case "-":
      return num1 - num2;
    case "*":
      return num1 * num2;
    case "/":
      return num2 !== 0 ? num1 / num2 : null;
    default:
      return null;
  }
}


~~~

<h1>Week challenges (Tuesday) 💻</h1>
<h2>Even or odd 🤖 - codewars</h2>
<b>"In javascript Create a function that takes an integer as an argument and returns "Even" for even numbers or "Odd" for odd numbers. "</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/4b77229c-ffa1-45cf-b4fd-15e13d0739f3" alt="" width="600" height="300">

~~~javascript
function evenOrOdd(number) {
  if(number % 2 ===0){
    return "Even"
  }else{
    return "Odd"
  }
}
~~~

<h2>A wolf in sheep's clothing 🤖 - codewars</h2>
<b>"If the wolf is the closest animal to you, return "Pls go away and stop eating my sheep". Otherwise, return "Oi! Sheep number N! You are about to be eaten by a wolf!" where N is the sheep's position in the queue."</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/3610aad5-ac65-4db8-a081-409a22f2ae6a" alt="" width="600" height="300">

~~~javascript

function warnTheSheep(queue) {
  const wolfIndex = queue.findIndex(animal => animal === 'wolf');
  const sheepIndex = queue.length - wolfIndex - 1;

  if (sheepIndex === 0) {
    return "Pls go away and stop eating my sheep";
  } else {
    return "Oi! Sheep number " + sheepIndex + "! You are about to be eaten by a wolf!";
  }
}
~~~

<h2>Decode the morse code 🤖 - codewars</h2>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/16b36683-bbb8-4a91-a6d7-7d73f2607b16" alt="" width="600" height="300">


~~~javascript

decodeMorse = function(morseCode){
  function decodeMorseLetter(letter) {
    return MORSE_CODE[letter];
  }
  function decodeMorseWord(word) {
    return word.split(' ').map(decodeMorseLetter).join('');
  }
  return morseCode.trim().split('   ').map(decodeMorseWord).join(' ');
}
~~~

<h1>Week challenges (Wednesday) 💻</h1>
<h2>Who likes it? 🤖 - codewars</h2>
<b>"Implement the function which takes an array containing the names of people that like an item. It must return the display text as shown in the examples:"</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/05b0e673-603f-4ad5-87da-72c36f97e76e" alt="" width="600" height="300">

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


<h2>Bit counting 🤖 - codewars</h2>
<b>"Write a function that takes an integer as input, and returns the number of bits that are equal to one in the binary representation of that number. You can guarantee that input is non-negative."</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/29615c27-8e98-4d66-afb6-3f07976a6f5f" alt="" width="600" height="300">

~~~javascript
var countBits = function(n) {
  const binary = n.toString(2);

  let count = 0;
  for (let i = 0; i < binary.length; i++) {
    if (binary[i] === '1') {
      count++;
    }
  }

  return count;
};

~~~

<h2>Your order, please 🤖 - codewars</h2>
<b>"Your task is to sort a given string. Each word in the string will contain a single number. This number is the position the word should have in the result."</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/b431916c-9548-464e-b858-d00e3029642e" alt="" width="600" height="300">

~~~javascript
function order(words) {
  if (words.length === 0) {
    return "";
  }

  const wordArray = words.split(" ");
  const sortedArray = [];

  for (let i = 1; i <= 9; i++) {
    for (const word of wordArray) {
      if (word.includes(i.toString())) {
        sortedArray.push(word);
      }
    }
  }

  return sortedArray.join(" ");
}

~~~


<h1>Week challenges (Thursday) 💻</h1>
<h2>Counting duplicates 🤖 - codewars</h2>
<b>"Write a function that will return the count of distinct case-insensitive alphabetic characters and numeric digits that occur more than once in the input string. The input string can be assumed to contain only alphabets (both uppercase and lowercase) and numeric digits."</b>
<h3>Solution</h3>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/a08aa98c-f9e1-4630-b9da-1e40325ca3ec" alt="" width="600" height="300">

~~~javascript
function duplicateCount(text) {
  text = text.toLowerCase();
  
  var charCount = {};
  
  for (var i = 0; i < text.length; i++) {
    var char = text[i]; 
    if (!char.match(/[a-z0-9]/i)) {
      continue;
    }
    if (!charCount[char]) {
      charCount[char] = 0;
    }
    charCount[char]++;
  }
  
  var duplicateCount = 0;
  for (var key in charCount) {
    if (charCount[key] > 1) {
      duplicateCount++;
    }
  }
  
  return duplicateCount;
}
~~~

<h2>Encrypt this! 🤖 - codewars</h2>
<b>"You want to create secret messages which can be deciphered by the Decipher this! kata."</b>
<h3>Solution</h3>
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/b4fd033c-5bbd-451a-ab8d-ab3d1276af3e" alt="" width="600" height="300">

~~~javascript
function encryptThis(message) {
  return message.split(' ').map(function(word) {
    var firstChar = word.charCodeAt(0);
    if (word.length > 2) {
      var secondChar = word.charAt(1);
      var lastChar = word.charAt(word.length - 1);
      word = firstChar + lastChar + word.substring(2, word.length - 1) + secondChar;
    } else if (word.length === 2) {
      word = firstChar + word.charAt(1);
    } else {
      word = firstChar.toString();
    }
    return word;
  }).join(' ');
}

~~~


<h2>Valid parentheses 🤖 - codewars</h2>
<b>"Write a function that takes a string of parentheses, and determines if the order of the parentheses is valid. The function should return true if the string is valid, and false if it's invalid."</b>
<h3>Solution</h3>
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/50074ecf-25d4-4f13-8a73-fe44ef39b323" alt="" width="600" height="300">
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/485a23c9-2f4b-4284-80aa-f6cab1bba5d8" alt="" width="600">

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


<h2>Convert string to camel case 🤖 - codewars</h2>
<b>"Complete the method/function so that it converts dash/underscore delimited words into camel casing. The first word within the output should be capitalized only if the original word was capitalized (known as Upper Camel Case, also often referred to as Pascal case). The next words should be always capitalized."</b>
<h3>Solution</h3>
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/a9ab5c75-9fcd-406a-9503-577079a343a6" alt="" width="600" height="300">

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
