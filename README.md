<h1># core-code-from-scratch-readme Algorithms - Week 1</h1>
<h1>Week #1challenges</h1>
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

