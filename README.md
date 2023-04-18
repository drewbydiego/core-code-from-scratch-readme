<h1># core-code-from-scratch-readme Algorithms - Week 1</h1>
<h1>Week #1 challenges</h1>
<h1>Week challenges (Wednesday) 💻</h1>
<h2>Let's make pizza 🍕</h2>
<b>"Design an algorithm to prepare a pizza from scratch. Define the ingredients, what will be the flavor and the preparation."</b>
<h3>Solution</h3>
  <b>Flavor: cheese pizza.</b><br>
Ingredients:
<ul>
  <li>Pizza dough</li>
  <li>Tomato sauce</li>
  <li>Mozzarella cheese</li>
  <li>Salt</li>
  <li>Olive oil</li>
</ul><br>
  <b>Preparation:</b>
<ol>
  <li>Preheat the oven to a high temperature.</li>
  <li>Roll out the pizza dough to the desired thickness.</li>
  <li>Place the dough on a baking sheet or pizza stone.</li>
  <li>Spread tomato sauce over the dough, leaving some space around the edges.</li>
  <li>Sprinkle mozzarella cheese over the tomato sauce.</li>
  <li>Bake the pizza in the preheated oven until the crust is golden brown and the cheese is melted and bubbly.</li>
  <li>Remove the pizza from the oven and let it cool for a few minutes.</li>
  <li>Slice the pizza and serve.</li>
</ol><br>

<h2>Hot N Cold 🤒 🧊 🔥</h2>
<b>"Convert temperatures from Celsius to Fahrenheit and vice versa."</b>
<h3>Solution</h3><br>
<ol>
  <li>To convert from Celsius to Fahrenheit:</li>
    <ul>
       <li>Multiply the temperature in Celsius by 9/5.</li>
       <li>Add 32 to the result.</li>
       <li>The final number is the temperature in Fahrenheit.</li>
    </ul>
   <li>To convert from Fahrenheit to Celsius:</li>
    <ul>
       <li>Subtract 32 from the temperature in Fahrenheit.</li>
       <li>Multiply the result by 5/9.</li>
       <li>The final number is the temperature in Celsius.</li>
    </ul>
</ol><br>

<h2>Some geometry 📐</h2>
<b>"Design an algorithm to calculate the volume of a pyramid, a cube and a sphere."</b>
<h3>Solution</h3><br>
<ol>
  <li>To calculate the volume of a pyramid:
    <ul>
      <li>Determine the base area of the pyramid (length x width).</li>
      <li>Multiply the base area by the height of the pyramid.</li>
      <li>Divide the result by 3.</li>
      <li>The final number is the volume of the pyramid.</li>
    </ul>
  </li>
  <li>To calculate the volume of a cube:
    <ul>
      <li>Measure one side of the cube.</li>
      <li>Multiply the side length by itself twice (length x width x height).</li>
      <li>The final number is the volume of the cube.</li>
    </ul>
  </li>
  <li>To calculate the volume of a sphere:
    <ul>
      <li>Measure the radius of the sphere.</li>
      <li>Cube the radius (multiply it by itself three times).</li>
      <li>Multiply the result by 4/3 and by pi (3.14159).</li>
      <li>The final number is the volume of the sphere.</li>
    </ul>
  </li>
</ol>
<h1>Week challenges (Thursday) 💻</h1>
<h2>Numbers 📈</h2>
<b>"Design an algorithm to check if a number is even or odd. If it is even, write that it is even, otherwise write that it is odd. Represent the algorithm in a flowchart."</b>
<h3>Solution</h3><br>

![Even or Odd -  Diagrama de flujo week1 (1)](https://user-images.githubusercontent.com/76753050/229239320-571b6dd8-4087-44c4-8d68-38a05ddc7595.png)

<h2>How old are you 👴</h2>
<b>"Write pseudocode for an algorithm that calculates the age of a person based on date of birth"</b>
<h3>Solution</h3><br>
<ol>
  <li><b>OUTPUT</b> a message to ask the date of birth -> "What is your date of bith?"<br></li>
  <li><b>INPUT</b> user's date of birth<br></li>
  <li><b>STORE</b> the date of birth -> 'date_of_birth'<br></li>
  <li><b>DEFINE</b> the current year in a variable -> 'right_now'<br></li>
  <li><b>DEFINE</b> a variable to calculate the age -> 'age'<br></li>
  <li><b>CALCULATE</b> the age by subtracting the current date/year 'right_now' and the 'date_of_birth'<br>
    age = right_now - date_of_birth<br></li>
  <li><b>OUTPUT</b> the result -> "Your age is " + age<br></li>
  <li><b>End</b><br></li>
</ol>

<h2>Find the treasure 👑</h2>
<b>"We are in a room with three chests. We know that at least one has a treasure in it. Each chest has a message, but all the messages are lies.<br><br>
Left chest: The middle chest has a treasure<br>
Middle chest: All these chests have treasures in them<br>
Right chest: Only one of these chests has treasures.<br><br>

Which chests have treasures?"<br></b>

<img width="354" alt="202836372-19159ef8-14d5-4ecf-b08c-819b05e79f81" src="https://user-images.githubusercontent.com/76753050/229242574-e984db61-8956-494b-bc28-692fd33bc5d9.png">

<h3>Solution</h3><br>
<b>The chest A and C contain a treasure</b><br><br>
The message on the left chest says that the middle chest has a treasure, but we know this can't be true because all the messages are lies. Therefore, the middle chest does not have a treasure.<br><br>
The message on the middle chest says that all three chests have treasures, but since we know at least one message is false, this one must be false too. This means that at least one chest does not have a treasure, and since we already know the middle chest does not have a treasure, we can conclude that either the left or right chest has a treasure.<br><br>
The message on the right chest says that only one chest has a treasure, but again, we know this is a lie. This means that either zero or two chests have a treasure.<br><br>
After checking the posibilities on each chest, We can know that the middle chest does not have treasure but the other ones have, since "at least" one chest can have it We can choose the "A" or "C".

<h1>Week #2 challenges</h1>
<h1>Week challenges (Monday) 💻</h1>
<h2>Logic problem 🎲</h2>
<b>"The teacher asks his 5 students if they studied mathematics yesterday.<br><br>

Alice: "Nobody studied math yesterday".<br>
Bob: "1 person studied math yesterday".<br>
Charlie: "2 people studied math yesterday".<br>
Dan: "3 people studied mathematics yesterday".<br>
Eva: "4 people studied mathematics yesterday".<br><br>

The teacher knows that only those who studied would be telling the truth and those who didn't would be lying. Who is telling the truth?"</b>
<h3>Solution</h3>
<p>Out of the five students, only those who studied math yesterday would tell the truth, and those who didn't would lie. Alice's statement contradicts the rest, so it's false. Bob said one person studied math yesterday, which means Alice's statement is false, and someone did study. Charlie, Dan, and Eva's statements agree that more than one person studied math yesterday. Since three people cannot have studied math yesterday, Eva's statement is false, and two people studied math yesterday. Therefore, the only student telling the truth is Charlie, who said that two people studied math yesterday.</p>

<h2>Cereal vrs Milk 🥛</h2>
<b>"Create an algorithm to prepare a bowl of cereal with milk. Represent the result in pseudocode and in a flowchart."</b>
<h3>Solution</h3>
<h3>Pseudocode</h3><br>
<ol>
  <li>Grab a clean bowl.</li>
  <li>Pour the desired amount of cereal into the bowl.</li>
  <li>Grab the milk container from the fridge.</li>
  <li>Pour the desired amount of milk into the bowl, over the cereal.</li>
  <li>Take a spoon and mix the cereal and milk until they are well combined.</li>
  <li>Enjoy your bowl of cereal and milk.</li>
</ol>
<h3>Flowchart</h3><br>
<img width="300" alt="202836372-19159ef8-14d5-4ecf-b08c-819b05e79f81" src="https://user-images.githubusercontent.com/76753050/231023593-acc3948f-5f1e-4c50-9296-cf4a1aac21ed.png">
<h1>Week challenges (Tuesday) 💻</h1>
<h2>Install PSeInt 🖥️</h2>
<b>For this week we are going to use a program called PSeInt, this tool will help us to understand key programming concepts using a pseudocode language. The description of this tool is the following:</b><br><br><p>"It is a tool to assist a student in their first steps in programming.
Through a simple and intuitive pseudo-language in Spanish (complemented by a flowchart editor),
it allows you to focus your attention on the fundamental concepts of computational algorithms,
minimizing the difficulties of a language and providing a work environment with numerous aids and teaching resources."</p>
<h3>Solution</h3><br>
<img width="500" alt="202836372-19159ef8-14d5-4ecf-b08c-819b05e79f81" src="https://user-images.githubusercontent.com/76753050/231320816-11559c44-0a93-4fbb-8b84-0d4c7fffc809.png">

<h2>Print my name 🖨️</h2>
<b>"This will be a guided challenge, the idea is for you to use PSeInt. For this challenge, we will print your name on the screen, a simple task that will help us to review the way PSeInt works."</b>
<h3>Solution</h3><br>
<img width="500"500 alt="202836372-19159ef8-14d5-4ecf-b08c-819b05e79f81" src="https://user-images.githubusercontent.com/76753050/231321329-cf22b358-52a2-4ba9-a5a7-fe2b5d49c1b5.png">

<h2>Print my name & age 🐱‍💻</h2>
<b>"This challenge is similar to the previous guided challenge, but now you will try alone. For this challenge, you will need to create an algorithm in Pseudocode using PSeInt that prints your name and your age in separate lines, remeber that your name should be a string and your age a number"</b>
<h3>Solution</h3><br>
<img width="500" alt="202836372-19159ef8-14d5-4ecf-b08c-819b05e79f81" src="https://user-images.githubusercontent.com/76753050/231322027-09ebcd04-e1c6-489d-8c75-584acb083964.png">
<h1>Week challenges (Wednesday) 💻</h1>
<h2>Algorithm game🐱‍</h2>
<b>"This will be a fun challenge, you will be playing a game base on simple commands, and the idea is for you to help the squirrel to take the pine cone. For this challenge try to pass the first 15 levels. We wish you all the luck and happy gaming."</b>
<h3>Solution</h3><br>
<img width="500" alt="202836372-19159ef8-14d5-4ecf-b08c-819b05e79f81" src="https://user-images.githubusercontent.com/76753050/231916321-6b951322-5dd1-473c-adb5-1a811fbd2589.png">

<h2>Mod 💻</h2>
<b>"The challenge for you now is to create a PSeInt program that will receive a number from the user and add the mod operator using the even/odd case ( X % 2 ) where X is the user input"</b>
<h3>Solution</h3><br>
<img width="500" alt="202836372-19159ef8-14d5-4ecf-b08c-819b05e79f81" src="https://user-images.githubusercontent.com/76753050/231917408-afb7d832-d0e1-4930-944b-3b498a43b3fa.png">

<h2>Register form 💻</h2>
<b>"You are given the task to create a registration form for new users, this form should ask the user for the following information:"
-First name<br>
-Last name<br>
-Age<br>
-Email<br>
-Address
</b>
<h3>Solution</h3><br>
<img width="500" alt="202836372-19159ef8-14d5-4ecf-b08c-819b05e79f81" src="https://user-images.githubusercontent.com/76753050/231919514-833b459a-a9ae-4b53-8344-a9bd4d42b0a1.png">
<h1>Week challenges (Thursday) 💻</h1>
<h2>Truth tables 🧑‍🏫</h2>
<b>"You are going to learn about three main logical operations used in programming, these operations are called AND, OR, and NOT. Each of the operations uses booleans as operands, and when applying the operations a result is generated, which is also a boolean, this is easier to check using the Truth Tables for each of the operations, now your task is for you to learn, and add the Truth Tables for each of the operations add them to your README and check if the following operations are correct by answering ✅ or ❌ at the end of each operation"</b>
<h3>Solution</h3><br>
<ol>
  <li>T & T = T ✅</li>
  <li>T & F = F ✅</li>
  <li>F & T = T ❌</li>
  <li>F & F = F ✅</li>
  <li>T | T = T ✅</li>
  <li>T | F = F ❌</li>
  <li>F | T = T ✅</li>
  <li>F | F = F ✅</li>
  <li>~T = T ❌</li>
  <li>~F = T ✅</li>
  <li>(T & F) | (~F) = T ✅</li>
  <li>(T | F ) & (F | F) = T ❌</li>
  <li>~((T | F ) & (F | F)) & F = F ✅</li>
  <li>~((T | F ) & (F | F)) & T = T ✅</li>
</ol>
<h2>Boolean results ✍🏻</h2>
<b>"You have been assigned to verify and explain a code created by one of your colleagues, the idea is that you can describe the value that each variable has within the code as well as what was done for each line. What is expected of you is that you add comments below each line showing the value that the variable would have and a short explanation of how that value is reached."</b><br>
This is the code:<br><br>

Algoritmo boolean<br>
	a <- 5 == 3<br>
	b <- 4 <> 3<br>
	c <- 7 > 7<br>
	d <- 4 < 4<br>
	e <- 100 <= 90<br>
	f <- 40 >= 40<br>
FinAlgoritmo

<h3>Solution</h3><br>
Algoritmo boolean

    a <- 5 == 3      // a = falso
    // The '==' operator checks if the left and right operands are equal. Since 5 is not equal to 3, the value of a is false.
    
    b <- 4 <> 3      // b = verdadeiro
    // The '<>' operator checks if the left and right operands are not equal. Since 4 is not equal to 3, the value of b is true.
    
    c <- 7 > 7       // c = falso
    // The '>' operator checks if the left operand is greater than the right operand. Since 7 is not greater than 7, the value of c is false.
    
    d <- 4 < 4       // d = falso
    // The '<' operator checks if the left operand is less than the right operand. Since 4 is not less than 4, the value of d is false.
    
    e <- 100 <= 90   // e = falso
    // The '<=' operator checks if the left operand is less than or equal to the right operand. Since 100 is not less than or equal to 90, the value of e is false.
    
    f <- 40 >= 40    // f = verdadeiro
    // The '>=' operator checks if the left operand is greater than or equal to the right operand. Since 40 is equal to 40, the value of f is true.
    
FinAlgoritmo
<h2>Identify odd and even numbers👨🏻‍💻</h2>
<b>"Remember the last challenge about the Mod operator? well, today your task will be to create a program that will be able to detect based on the user input if the number is odd or even. The process should be the following:"</b><br><br>

1. The user enters a number
2. Your algorithm detects if the number is odd or even (remember to use conditional statements Si...Entonces)
3. Print ‘Número: x es par’ if the number is even (x is the number the user enters)
4. Print ‘Número: x es impar’ if the number is odd (x is the number the user enters)
<h3>Solution</h3><br>

Algoritmo DetectarNumeroParImpar

    Escribir "Por favor ingrese un número: "
    Leer numero

    Si numero % 2 == 0 Entonces
        Escribir "Número: " , numero , " es par"
    SiNo
        Escribir "Número: " , numero , " es impar"
    FinSi

FinAlgoritmo
<br><img src="https://user-images.githubusercontent.com/76753050/232912068-28b1c9bf-76cb-4ccf-a5f9-5cc055fc5f0f.gif" alt="Example GIF" width="450" height="250">
