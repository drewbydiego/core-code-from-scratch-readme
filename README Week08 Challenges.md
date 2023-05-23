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
