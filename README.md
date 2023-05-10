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
<h1>Week #3 challenges</h1>
<h1>Week challenges (Monday) 💻</h1>
<h2>Simple calculator🖩</h2>
<b>"For this challenge you will be performing a simple calculator, this calculator can perform the following operations:</b><br><br>
1. Sum (+)<br>
2. Subtract (-)<br>
3. Multiplication (*)<br>
4. Division (/)<br><br>
The calculator must ask the user for two numbers, after asking for the two numbers, you must ask for the operation to be performed, keep in mind that you must show the user the options available (+, -, *, /). The first thing that must be done is to validate that the operation that the user entered is valid, if it is not a valid option, the user must be shown an error message, for example: ⚠️ La operación no es valida and terminate the program. If the operation is valid, show the message: Procesando: <OPERACIÓN A REALIZAR> For, example: if the user has entered the numbers 10 and 15 as well as the operation *, the message should read: Procesando: 10 * 15. After this message the result of the operation must be displayed, following the previous example, the result of operating 10 * 15 is 150, so the program should return: Resultado: 150. Remember to use conditionals to identify which operations you should execute."<br>

<h3>Solution</h3><br>
Proceso CalculadoraBasica
    Definir numero1, numero2, resultado Como Real
    Definir operacion Como Caracter
	
    Escribir "Ingrese el primer numero:"
    Leer numero1
    Escribir "Ingrese el segundo numero:"
    Leer numero2
	
    Escribir "Ingrese la operacion a realizar (+, -, *, /):"
    Leer operacion
	
	si operacion = "+" Entonces
		resultado = numero1 + numero2
		Escribir "Procesando: ", numero1, " + ", numero2
        Escribir "Resultado: ", resultado
	SiNo
		si operacion = "-" Entonces
			resultado = numero1 - numero2
			Escribir "Procesando: ", numero1, " - ", numero2
			Escribir "Resultado: ", resultado
			
		SiNo
			si operacion = "*" Entonces
				resultado = numero1 * numero2
				Escribir "Procesando: ", numero1, " * ", numero2
				Escribir "Resultado: ", resultado
				
			SiNo
				si operacion = "/" Entonces
					resultado = numero1 / numero2
					Escribir "Procesando: ", numero1, " / ", numero2
					Escribir "Resultado: ", resultado
				SiNo
					Escribir "¡La operación no es valida!"
				FinSi
			FinSi
		FinSi
	FinSi
FinProceso

<img src="https://user-images.githubusercontent.com/76753050/232917347-267d6511-ece6-4b3c-9ac2-eff762b4b126.gif" alt="Example GIF" width="450" height="250">
<h2>Special number 🧮</h2>
<b>"You must create the code that follows the following logic, if the given number is 100, take this number as special and show the following message: "This is a special number!", but if the number is less than 1000, multiple of 10 and different from 100, you must show the following message: "This number is almost special". if none of the given conditions are met show the following message: "Just a regular number". Another developer was trying to program the logic, but apparently couldn't, you need to fix the code to work properly"<br><br>This was the code from the developer<br></b>

Algoritmo specialNumber

	Leer n
	Si n == 100 Entonces
		Imprimir 'This is a special number'
	FinSi
	Si n < 1000 Entonces
		Imprimir ''
	SiNo
		Imprimir 'Just a regular number'
	FinSi
	Si n % 10 == 0 Entonces
		Imprimir 'This number is multiple of 10'
	FinSi
FinAlgoritmo

<h3>Solution</h3><br>
<img src="https://user-images.githubusercontent.com/76753050/232918960-f95ee606-0615-42ca-acf4-538681dde1e4.gif" alt="Example GIF" width="450" height="250">
<h1>Week challenges (Tuesday) 💻</h1>
<h2>Simple calculator with Switch🖩</h2>
<b>"For this challenge you will be performing a simple calculator using Switch (Segun), this calculator can perform the following operations:<br><br>

1. Sum (+)
2. Subtract (-)
3. Multiplication (*)
4. Division (/)</b><br><br>
The calculator must ask the user for two numbers, after asking for the two numbers, you must ask for the operation to be performed, keep in mind that you must show the user the options available (+, -, *, /). The first thing that must be done is to validate that the operation that the user entered is valid, if it is not a valid option, the user must be shown an error message, for example: ⚠️ La operación no es valida and terminate the program. If the operation is valid, show the message: Procesando: <OPERACIÓN A REALIZAR> For, example: if the user has entered the numbers 10 and 15 as well as the operation *, the message should read: Procesando: 10 * 15. After this message the result of the operation must be displayed, following the previous example, the result of operating 10 * 15 is 150, so the program should return: Resultado: 150. Remember to use Switch (Segun) to identify which operations you should execute."
<h3>Solution</h3><br>
Algoritmo CalculadoraSwitch

	Definir num1, num2, resultado como real
	Definir operador como caracter
	Escribir("Ingrese el primer número: ")
	Leer num1
	Escribir("Ingrese el segundo número: ")
	Leer num2
	Escribir("Ingrese el operador (+, -, *, /): ")
	Leer operador
	Si operador == '+' | operador == '-' | operador == '*' | operador == '/' Entonces
	Segun operador Hacer
		"+" :
			resultado <- num1 + num2
			Escribir"Procesando: ", num1, " , ", num2
			Escribir"Resultado: ", resultado
		"-" :
			resultado <- num1 - num2
			Escribir "Procesando: ", num1, " - ", num2
			Escribir"Resultado: ", resultado
		"*" :
			resultado <- num1 * num2
			Escribir "Procesando: ", num1, " * ", num2
			Escribir"Resultado: ", resultado
		"/" :
			Si num2 = 0 Entonces
				Escribir "¡No se puede dividir entre cero!"
			Sino
				resultado <- num1 / num2
				Escribir "Procesando: ", num1, " / ", num2
				Escribir"Resultado: ", resultado
			FinSi
	FinSegun 
	SiNo
	Escribir"¡La operación no es valida!"
	fin si	
FinAlgoritmo
<br><img src="https://user-images.githubusercontent.com/76753050/232941836-c491d407-ae91-4db7-a72e-cbb609575448.gif" alt="Example GIF" width="450" height="250">
<h2>Multi Option Program 🤳</h2>
<b>"For this challenge you will create a program with multiple options using Switch (Segun), the options available are the following:<br><br>
1. Sum two numbers
2. Print the day of the week given the day number
3. Print the length of a given text<br><br>
This program must have a start menu where the user must select one of the previously described options. When the user selects each of the options, the program will perform the following:<br><br>

1. Sum. The user enters two numbers and the result of the sum of both is printed<br>
2. Print day of the week. The user enters a day of the week using numbers and the name of the day must be printed. For example, if the number 1 is entered, the program prints the text Lunes.<br>
3. Calculate text length. The user enters a text and the length of the text should be printed. I was able to use the Pseint Longitud function to get the length.
"</b>
<h3>Solution</h3>
Proceso Menuopciones

    Escribir "Seleccione una opción:"
    Escribir "1. Sumar dos números"
    Escribir "2. Imprimir día de la semana"
    Escribir "3. Calcular longitud de un texto"
    Leer opcion
	
	Segun opcion Hacer
		1:
			Escribir "Ingrese el primer número:"
            Leer num1
            Escribir "Ingrese el segundo número:"
            Leer num2
            resultado = num1 + num2
            Escribir "El resultado de la suma es:", resultado
		2:
			Escribir "Ingrese el número del día de la semana (1-7):"
            Leer dia
            Segun dia Hacer
                1: Escribir "Lunes"
                2: Escribir "Martes"
                3: Escribir "Miércoles"
                4: Escribir "Jueves"
                5: Escribir "Viernes"
                6: Escribir "Sábado"
                7: Escribir "Domingo"
                De Otro Modo:
                    Escribir "Día no válido"
            FinSegun
		3:
			Escribir "Ingrese un texto:"
            Leer texto
            longitudTexto = Longitud(texto)
            Escribir "La longitud del texto es:", longitudTexto
		De Otro Modo:
			Escribir "Opción no válida"
	Fin Segun
FinProceso
<br><img src="https://user-images.githubusercontent.com/76753050/232944050-35df939d-1782-402e-8a16-be17ab6fb830.gif" alt="Example GIF" width="450" height="250">


<h1>Week challenges (Wednesday) 💻</h1>
<h2>Multiplication Tables ✖️</h2>
<b>"For this challenge you will create a program to calculate the multiplication tables for a given number using While (Mientras). The user must enter a number and then the multiplication table for the number must be printed."</b>
<h3>Solution</h3><br>
Algoritmo MultiplicationTable

	Escribir "--TABLA DE MULTIPLICAR--"
	Escribir "Ingresa un número, por favor."
	Leer num
	contador = 1
	Escribir "Tabla del ", num
	Mientras contador <=10 Hacer
		Escribir num, " X ", contador, " = ", num * contador
		
		contador = contador + 1
	Fin Mientras
FinAlgoritmo
<br><img src="https://user-images.githubusercontent.com/76753050/233231592-70ff3f56-247c-4451-837d-e33ab34bb2b2.gif" alt="Example GIF" width="450" height="250">
<h2>Simple Calculator with Do While ❌</h2>
<b>"For this challenge we are going to use the simple calculator that we made in the challenge 02 but now adding the functionality to perform a calculation again without finishing the program. The program should ask us if we want to use another operation and if the user answers yes then we can perform a new operation. To solve this challenge remember to use Do while (Repetir Hasta Que)."</b>
<h3>Solution</h3><br>

Algoritmo CalculadoraDoWhile

	Definir num1, num2, resultado como real
	Definir operador como caracter
	Escribir "--CALCULADORA--"
	Repetir
	Escribir("Ingrese el primer número: ")
	Leer num1
	Escribir("Ingrese el segundo número: ")
	Leer num2
	Escribir("Ingrese el operador (+, -, *, /): ")
	Leer operador
	Si operador == '+' | operador == '-' | operador == '*' | operador == '/' Entonces
		Segun operador Hacer
			"+" :
				resultado <- num1 + num2
				Escribir"Procesando: ", num1, " , ", num2
				Escribir"Resultado: ", resultado
			"-" :
				resultado <- num1 - num2
				Escribir "Procesando: ", num1, " - ", num2
				Escribir"Resultado: ", resultado
			"*" :
				resultado <- num1 * num2
				Escribir "Procesando: ", num1, " * ", num2
				Escribir"Resultado: ", resultado
			"/" :
				Si num2 = 0 Entonces
					Escribir "¡No se puede dividir entre cero!"
				Sino
					resultado <- num1 / num2
					Escribir "Procesando: ", num1, " / ", num2
					Escribir"Resultado: ", resultado
				FinSi
		FinSegun 
	SiNo
		Escribir"¡La operación no es valida!"
	fin si	
	Escribir "¿Desea hacer otra operación?"
	Leer respuesta
	Hasta Que respuesta == 'No' | respuesta == 'no'

FinAlgoritmo

<br><img src="https://user-images.githubusercontent.com/76753050/233233247-6e51817d-e341-4d18-bf96-c40b57ecd5d5.gif" alt="Example GIF" width="450" height="250">

<h1>Week challenges (Thursday) 💻</h1>
<h2>Multiplication Tables with For ✖️</h2>
<b>"For this challenge you will create a program to calculate the multiplication tables for a given number using the For(Para) loop. The user must enter a number and then the multiplication table for the number must be printed."</b>
<h3>Solution</h3><br>
Algoritmo MultiplicationTableWithFor

	Escribir "--TABLA DE MULTIPLICAR (PARA)--"
	Escribir "Ingresa un número, por favor."
	Leer num
	Escribir "Tabla del ", num
	Para contador desde 1 hasta 10 Hacer
		Escribir num, " X ", contador, " = ", num * contador
	FinPara
FinAlgoritmo
<br><img src="https://user-images.githubusercontent.com/76753050/233508693-3d5e3610-7b1f-482f-aaf9-46f7da5bd413.gif" alt="Example GIF" width="450" height="250">

<h2>Ascending and Descending Numbers 🔢</h2>
<b>"For this challenge we are going to print numbers in ascending or descending order. The user must enter a number, then he must enter if he wants to print the numbers in ascending or descending order. If the user chooses ascending, the numbers will be printed from the number 0 to the number entered, otherwise the numbers will be printed descending from the number entered to the number 0.To solve this challenge remember to use the For(Para) loop."</b>
<h3>Solution</h3><br>
Algoritmo AscendingDescending

	Definir num, opcion como Entero
	
	Escribir "Ingrese un número:"
	Leer num
	
	Escribir "¿Desea imprimir en orden ascendente o descendente?"
	Escribir "(1 = Ascendente, 2 = Descendente)"
	Leer opcion
	
	Si opcion = 1 Entonces
		Escribir "Números en orden ascendente:"
		Para i desde 1 hasta num Hacer
			Escribir i
		FinPara
	SiNo
		Escribir "Números en orden descendente:"
		Para i desde num hasta 1 Hacer
			Escribir i
		FinPara
		
	FinSi
FinAlgoritmo
<br><img src="https://user-images.githubusercontent.com/76753050/233509661-20d25816-3f49-4362-86a9-99220994a917.gif" alt="Example GIF" width="450" height="250">

<h2>Greetings 😀</h2>
<b>"For this challenge, you need to create a program that prints a greeting based on an hour entered. The program should do the following:<br>
<ul>
  <li>Print Buenos dias! if the hour is from 0 to 12</li>
  <li>Print Buenas tardes! if the hour is from 13 to 18</li>
  <li>Print Buenas noches! if the hour is from 19 to 23</li>
  <li>Ask the user if he wants to perform another greeting. If the answer is Si, the program must start again.</li>
  <li>At the end of the program, print out the number of times the program has greeted."</li></ul></b>
<h3>Solution</h3><br>


Algoritmo Greeting

	Definir hora como Entero
	Definir continuar Como Caracter
	contador = 0
	
	Repetir
		Escribir "Ingrese la hora (0 a 23):"
		Leer hora
		
		Si hora >= 0 & hora <= 12 Entonces
			Escribir "Buenos dias!"
		SiNo Si hora >= 13 & hora <= 18 Entonces
				Escribir "Buenas tardes!"
			SiNo Si hora >= 19 & hora <= 23 Entonces
					Escribir "Buenas noches!"
				SiNo
					Escribir "Hora inválida."
				FinSi
			FinSi
		FinSi
		
		Escribir "¿Desea realizar otro saludo? ¿Si/No?):"
		Leer continuar
		
		contador = contador + 1
		
	Hasta Que continuar = 'No' | continuar ='no' | continuar = 'NO'
	
	Escribir "El programa ha saludado ", contador, " veces."
FinAlgoritmo


<br><img src="https://user-images.githubusercontent.com/76753050/233512281-bc563f03-fd06-4581-8a70-f8d36b7e5452.gif" alt="Example GIF" width="450" height="250">

<h1>Week #4 challenges</h1>
<h1>Week challenges (Monday) 💻</h1>
<h2>Average sales and commission 📟</h2>
<b>"Make a program that asks how many sales the seller had, Once the number of sales is entered, ask for the value of each sale until all are entered, then return as a result the average value of sales, and the commission that the seller will take, If the seller had more than 5 sales, his commission will be 15% of the total value of the sales, if he sold 5 or less, his commission will be only 10%.</b>
<h3>Solution</h3><br>
Algoritmo SellerCommission
	
	Escribir "Enter the number of sales:"
	Leer numSales
	Cdata = ""

	totalSales <- 0
	Para i desde 1 hasta numSales hacer
		Escribir "Enter the value of sale ", i, ":"
		Leer saleValue
		totalSales <- totalSales + saleValue
	FinPara
	

	promedioVentas <- totalSales / numSales
	Si numSales > 5 Entonces
		comision <- 0.15 * totalSales
		Cdata = "15%"
	SiNo
		comision <- 0.10 * totalSales
		Cdata = "10%"
	FinSi
	
	Escribir "Average value of sales:", promedioVentas
	Escribir "Sellers commission:", comision
	Escribir "Comission value ", Cdata
	
FinAlgoritmo

<br><img src="https://user-images.githubusercontent.com/76753050/234150852-924f535f-2c70-45db-8f8d-e5eb67fff195.gif" alt="Example GIF" width="450" height="250">

<h2>Even or odd 📟</h2>
<b>"Request a number from 1 to 50, if the number is not between those values, report the error and request it again until you get a valid number, then it shows on the screen all the numbers from 1 to that number, if the number is even it only shows the even numbers, if it is odd it only shows the odd ones."</b>
<h3>Solution</h3>
Algoritmo EvenOddNumbers
	
	num <- 0
	Mientras num < 1 |  num > 50 hacer
		Escribir "Enter a number between 1 and 50:"
		Leer num
		Si num < 1 |  num > 50 Entonces
			Escribir "Error Enter a number between 1 and 50!!!!"
			Escribir "-----------------------------------------"
		FinSi
	FinMientras

	Para i desde 1 hasta num hacer
		Si num % 2 = 0 Entonces
			Si i % 2 = 0 Entonces
				Escribir i
			FinSi
		SiNo
			Si i % 2 <> 0 Entonces
				Escribir i
			FinSi
		FinSi
	FinPara
	
FinAlgoritmo
<br><img src="https://user-images.githubusercontent.com/76753050/234151731-90f340dd-b35c-4b84-bac8-298e97f48634.gif" alt="Example GIF" width="450" height="250">

<h1>Week challenges (Tuesday) 💻</h1>
<h2>Full name 👾</h2>
<b>"Make a program that takes a first name and a last name, then returns a string with both values ​​with the first letter uppercase and the rest lowercase."</b>
<h3>Solution</h3><br>
Algoritmo FullName
	
    Escribir "Ingrese su nombre:"
    Leer nombre
    Escribir "Ingrese su apellido:"
    Leer apellido
    
	CapNombre = Mayusculas(Subcadena(nombre,0,0)) + Minusculas(Subcadena(nombre,1,Longitud(nombre)-1))
	CapApellido = Mayusculas(Subcadena(apellido,0,0)) + Minusculas(Subcadena(apellido,1,Longitud(apellido)-1))
    
    Escribir "Su nombre formateado es: ", CapNombre , " " , CapApellido
FinAlgoritmo
<br><img src="https://user-images.githubusercontent.com/76753050/234734460-a5c622a1-27db-4c88-b2bc-f1f01e85c0b9.gif" alt="Example GIF" width="450" height="250">

<h2>Throw dice👾</h2>
<b>"make a program that simulates the roll of 2 dice 10 times, and display for each roll the values ​​of the two dice separated by a space, in case the 2 dice throw the same value in addition to the result, add a string to the ending that says "the dice are the same"</b>
<h3>Solution</h3><br>
Algoritmo RollDice
	
    Definir MIN_DADO Como Entero
	MIN_DADO = 1
    Definir MAX_DADO Como Entero
	MAX_DADO = 6
    Definir dadosIguales Como logico
    
    Para i = 1 Hasta 10 Con Paso 1 Hacer
        dado1 = Aleatorio(MAX_DADO, MIN_DADO)
        dado2 = Aleatorio(MAX_DADO, MIN_DADO)
        
        Si dado1 = dado2 Entonces
            dadosIguales = Verdadero
        Sino
            dadosIguales = Falso
        FinSi
        
        Escribir dado1, " ", dado2
        Si dadosIguales Entonces
            Escribir " - los dice son iguales"
        FinSi
		
    FinPara
FinAlgoritmo
<br><img src="https://user-images.githubusercontent.com/76753050/234736131-25de97a0-7e89-4a49-a203-6b32ffcb8bc2.gif" alt="Example GIF" width="450" height="250">

<h1>Week challenges (Wednesday) 💻</h1>
<h2>Distance to zero "0"</h2>
<b>"Make a program that asks for 5 values ​​and also allows us to know which one is furthest from zero, once obtained it returns that number (the numbers can be negative), showing only the integer part of the number."</b>
<h3>Solution</h3><br>
Algoritmo NumeroFurthest
	
    Definir NUM_VALORES Como Entero 
	NUM_VALORES = 5
    Definir maxDistancia Como Real 
	maxDistancia = 0
    Definir numFurthest Como Real 
	numFurthest= 0
    
    Para i = 1 Hasta NUM_VALORES Con Paso 1 Hacer
        Escribir "Enter the value ", i, ": "
        Leer valor

        distancia = Abs(valor)
        
        Si distancia > maxDistancia Entonces
            maxDistancia = distancia
            numFurthest = valor
        FinSi
    FinPara

    Escribir "The furthest value from zero is: ", Redon(numFurthest)
FinAlgoritmo
<br><img src="https://user-images.githubusercontent.com/76753050/234737585-3e9b0f58-3e45-4ece-b423-c915fcbe85bb.gif" alt="Example GIF" width="450" height="250">

<h2>Toss coin 🪙</h2>
<b>"From the data we receive first a name and a value, then another name and another value, using the built-in function aleatorio() we simulate the flip of a coin, We must return the name of the winner in capital letters and the value I win, to avoid cheating, if a player puts a value of zero or negative, the opponent automatically wins, in case both cheat, "game canceled" is returned."</b>
<h3>Solution</h3><br> 
Algoritmo TossCoin

    Definir nombre1, nombre2 Como Cadena
    Definir valor1, valor2, resultado Como Real
    
    Escribir "Enter the players name 1"
    Leer nombre1
    Escribir "Write the value of ", nombre1, ": "
    Leer valor1

    Escribir "Enter the players name 2"
    Leer nombre2
    Escribir "Write the value of ", nombre2, ": "
    Leer valor2
    
    Si valor1 <= 0 Entonces
        resultado = valor2
        Escribir Mayusculas(nombre2), " has won by cheating with a value of ", resultado
    Sino Si valor2 <= 0 Entonces
			resultado = valor1
			Escribir Mayusculas(nombre1), " has won by cheating with a value of ", resultado
		Sino

			moneda = Aleatorio(0,1)
	
			Si valor1 > valor2 Entonces
				Si moneda = 0 Entonces
					resultado = valor1
					Escribir Mayusculas(nombre1), " has won with a value of ", resultado
				Sino
					resultado = valor2
					Escribir Mayusculas(nombre2), " has won with a value of ", resultado
				FinSi
			Sino Si valor2 > valor1 Entonces
					Si moneda = 0 Entonces
						resultado = valor2
						Escribir Mayusculas(nombre2), " has won with a value of ", resultado
					Sino
						resultado = valor1
						Escribir Mayusculas(nombre1), " has won with a value of ", resultado
					FinSi
				Sino
					Escribir "The game has been cancelled due to cheating by both players."
				FinSi
			FinSi
		FinSi
	FinSi
FinAlgoritmo

<br><img src="https://user-images.githubusercontent.com/76753050/234740873-e7081d87-2780-438e-a780-6583d8a2beb5.gif" alt="Example GIF" width="450" height="250">

<h1>Week challenges (Thursday) 💻</h1>
<h2>Total price 🪙</h2>
<b>"Create a function called TotalPrice that takes 2 parameters, price and VAT, and returns the price including VAT. if the price exceeds 3000 a 10 percent discount is made on the total price.</b>
<h3>Solution</h3><br>
Algoritmo ProgramTotalPrice
	
    Definir price, vat, pTotal Como Real
	
    price <- 5000
    vat <- 21
	
    pTotal <- TotalPrice(price, vat)
	
    Escribir "The total price with VAT is: ", pTotal
FinAlgoritmo


Funcion value <- TotalPrice(price, vat)
	Definir discount, priceWVat Como Real
	
	priceWVat <- price + (price * vat / 100)
	
	Si price > 3000 Entonces
		discount <- priceWVat * 0.1
		priceWVat <- priceWVat - discount
	FinSi
	
	value <- priceWVat
	
FinFuncion

<br><img src="https://user-images.githubusercontent.com/76753050/235031506-bfe6bf0e-7874-4610-96e3-a8ba298411e2.gif" alt="Example GIF" width="450" height="250">

<h2>Reverse direction and size 👨🏻‍💻</h2>
<b>"Create a function called ReverseDirectionAndSize that takes some text as a parameter and reverses it, eg: "Hello" -> "olleH" and also reverses the letters if they are uppercase to lowercase and if they are lowercase to uppercase, it should do something. like this:<br><br>

"HelLO" --> "olLEh"<br>

"Leonardo" --> "ODRANOEl"<br>

"Text" --> "TXEt""</b><br>
<h3>Solution</h3><br>
Algoritmo Directiontext

	Imprimir Reverse("Leonardo")
FinAlgoritmo

Funcion result <- Reverse (ctext)

	Definir result Como Caracter;
	result = "";
	Para nChar = Longitud(ctext) - 1 Hasta 0 Con Paso -1 Hacer
		xChar = Subcadena(ctext, nChar, nChar);
		SI xChar = Mayusculas(xChar) Entonces
			xChar = Minusculas(xChar)
		SiNo
			xChar = Mayusculas(xChar)
		FinSi
		result = Concatenar(result, xChar)
	FinPara
Fin Funcion

<br><img src="https://user-images.githubusercontent.com/76753050/235034381-e5243f59-84ea-4e00-8161-ee44e85c05fc.gif" alt="Example GIF" width="450" height="250">

<h1>Week #5 challenges</h1>
<h1>Week challenges (Monday) 💻</h1>
<h2>Time Converter 📟</h2>
<b>"Create a function called timeConverter that receives a positive number of seconds and returns a string based on the number. "Days: 1, Hours: 5, Minutes: 40 and seconds: 5"<br><br>

4000 --> "days: 0, hours: 1, minutes: 6, and seconds: 4"<br>

40000 --> "days: 0, hours: 11, minutes: 6, and seconds: 4"<br>

150000 --> "days: 1, hours: 17, minutes: 40, and seconds: 0""</b><br>
<h3>Solution</h3><br>
Algoritmo timeConverterProgram

	Escribir "Write the a positive number of seconds"
	Leer seconds
	timeConverter(seconds)
FinAlgoritmo
![time converter](https://user-images.githubusercontent.com/76753050/235818478-e6057ec2-358b-4058-a3c0-0327e9122400.gif)

Funcion timeConverter(seg)

    Definir dias, horas, minutos, segundos Como real
	dias = trunc(seg / 86400)
    horas <- trunc((seg % 86400) / 3600)
    minutos <- trunc((seg % 3600) / 60)

    segundos <- trunc(seg % 60)

    Escribir  "Days: " + ConvertirATexto(dias) + ", Hours: " + ConvertirATexto(horas) + ", Minutes: " + ConvertirATexto(minutos) + " and seconds: " + ConvertirATexto(segundos)
FinFuncion

<br><img src="https://user-images.githubusercontent.com/76753050/235818503-59d8bcc8-3a47-4a01-b0cc-1f0d82e1f91c.gif" alt="Example GIF" width="450" height="250">

<h2>Compare distances 😵‍💫</h2>
<b>"Create a function called compareDistances that asks for 5 numbers, these can be positive or negative, add the positives with positives and negatives with negatives, the function should return true if there is more distance to 0 with positives or false if the distance is greater with negatives.<br><br>

4, 12 , 100, 8, -60 --> true<br>

40, 120 , 10, -80, -91 --> false"</b><br>
<h3>Solution</h3><br>

Algoritmo timeConverterProgram

	compareDistances() 
FinAlgoritmo


Funcion compareDistances()

    Definir num, sumPos, sumNeg Como Real
	sumPos = 0
	sumNeg = 0
    Escribir "Enter five numbers:"
    
    Para i <- 1 Hasta 5 Con Paso 1 Hacer
        Leer num
        Si num >= 0 Entonces
            sumPos <- sumPos + num
        Sino
            sumNeg <- sumNeg + num
        FinSi
    FinPara
    
    Si Abs(sumPos) > Abs(sumNeg) Entonces
        Escribir  Verdadero
    Sino
        Escribir  Falso
    FinSi
FinFuncion

<br><img src="https://user-images.githubusercontent.com/76753050/235819296-1cd91e79-ab58-4fe0-a888-07891ead8e9a.gif" alt="Example GIF" width="450" height="250">

<h1>Week challenges (Tuesday) 💻</h1>
<h2>Sum of pairs ➕</h2>
<b>"write a function called sumOfPairs that asks for a number from 1 to 100 indefinitely, if a negative number or greater than 100 is entered, it stops asking for more numbers and returns the sum of all the even numbers entered.<br><br>

4, 12 , 100, 11, -60 --> 116<br>

40, 121 --> 40"</b><br>
<h3>Solution</h3><br>

Algoritmo pairs

	sumOfPairs()
FinAlgoritmo

Funcion sumOfPairs()

    Definir sum, num Como Entero
    sum = 0
    num = 0
    
    Repetir
        Escribir "Ingrese un número entre 1 y 100: "
        Leer num
        Si num > 0 & num <= 100 Entonces
            Si num % 2 = 0 Entonces
                sum = sum + num
            FinSi
        Sino
        FinSi
    Hasta Que num < 1 | num > 100
    
    Escribir  sum
FinFuncion
<br><img src="https://user-images.githubusercontent.com/76753050/235820501-e6f1d85f-6409-4e64-878e-8b1072e693ce.gif" alt="Example GIF" width="450" height="250">

<h2>Mid point 🐦‍⬛</h2>
<b>"write a function called midpoint that given 2 values ​​(can be negative) does not return the value of the midpoint between them<br><br>

-50,50 --> 0<br>

40, 80 --> 60"<br></b>
<h3>Solution</h3><br>

Algoritmo Mpoint

	Escribir "Write number 1"
	leer v1
	Escribir "Write number 2"
	leer v2
	midpoint(v1, v2)
FinAlgoritmo

Funcion midpoint(valor1, valor2)

    Definir punto_medio Como Real
    punto_medio = (valor1 + valor2) / 2
    
    Escribir  punto_medio
FinFuncion

<br><img src="https://user-images.githubusercontent.com/76753050/235820980-f6dd698e-8ad9-46da-8f07-a29f17c02c0f.gif" alt="Example GIF" width="450" height="250">

<h1>Week challenges (Wednesday) 💻</h1>
<h2>Cashier 👩‍💻</h2>
<h3>Solution</h3><br>

Proceso cashier

    Definir balance, Tbalance Como Entero
    balance <- 1000
    opcion <- ""
	
    Mientras opcion <> "c" Hacer
        Escribir "select an option: a. to deposit. b. withdraw. c. go out."
        Leer opcion
		
        Si opcion = "a" Entonces
            balance = deposit(balance)
			Sino Si opcion = "b" Entonces
			balance = withdraw(balance)
        FinSi
	finsi
    FinMientras
	Escribir "Your balance is: ", balance

FinProceso

Funcion Tbalance <- deposit (balance)

		Definir amount Como Entero
		Escribir "how much do you want to deposit:"
		Leer amount
		balance <- balance + amount
		Tbalance <- balance
		Escribir  Tbalance

FinFuncion

Funcion Tbalance <- withdraw(balance)

		Definir amount Como Entero
		Escribir "how much do you want to withdraw:"
		Leer amount
		Tbalance <- balance - amount
		Escribir Tbalance
FinFuncion


<br><img src="https://user-images.githubusercontent.com/76753050/236361551-abc62f0e-2f4b-4fb5-bde2-b7b9d4371495.gif" alt="Example GIF" width="450" height="250">


<h2>Weather average ☁️"</h2>
<b>"write an algorithm that loops indefinitely until 'x' is entered which will calculate an average of the weather, note that for each value entered it should ask if it is fahrenheit or celsius, then ask for the value. add everything up and divide by the number of values ​​entered. The result must be returned in celsius, have a function that, in case fahrenheit is entered, transforms it to celsius in order to add them."</b>
<h3>Solution</h3><br>

Algoritmo Weather

	Definir count Como Entero 
	count = 0
	Definir total Como Real 
	total = 0
	Definir option Como Caracter
	option = ""
	Mientras option <> "x" Hacer
		Escribir "a. Enter degrees Celsius."
		Escribir "b. Enter degrees Fahrenheit."
		Escribir "x. Exit."
		Leer option
		
		Segun option Hacer
			"a", "b": 
				Imprimir "Enter temperature:"
				Leer degree
				count = count + 1
				Segun option Hacer
					"a": total = total + degree
					"b": total = total + fahrenheitToCelsius(degree)
				FinSegun
			"x": 
			De Otro Modo: Imprimir "Try a different option"
		FinSegun
	FinMientras
	
	Imprimir "The average temperature is ", total / count, " degrees Celsius."
FinAlgoritmo

Funcion celsius <- fahrenheitToCelsius(fahrenheit)

	Definir celsius Como Real
	celsius = (fahrenheit - 32) * 9/5
Fin Funcion

<br><img src="https://user-images.githubusercontent.com/76753050/236366180-bbd3fa15-b880-4fa9-ad1b-98e5f3f9450d.gif" alt="Example GIF" width="450" height="250">

<h1>Week challenges (Thursday) 💻</h1>
<h2>'IF' statement in JavaScript 🤓</h2>
<b>"Create an if statement with the JavaScript syntax"</b>
<h3>Solution</h3>

```

"use strict";

let number1, number2;

number1 = 30;
number2 = 20;

if (number1 > number2) {
    console.log("The number " + number1 + " is greater than " + number2)
}else{
    console.log("The number " + number1 + " is not greater than " + number2)
}

```

<h2>'WHILE' loop in JavaScript 🤓</h2>
<b>"Create a while loop statement with the JavaScript syntax"</b>
<h3>Solution</h3>


~~~

"use strict";

let i = 0;

while (i <= 10) {
    console.log(i);
    i++;
}


~~~




<br><img src="https://user-images.githubusercontent.com/76753050/236970553-bfe28a16-1a81-41a9-a5ed-80bc7235842a.png" alt="Example GIF" width="450" height="250">

<h2>''FOR' loop in JavaScript 🤓</h2>
<b>"Create a while loop statement with the JavaScript syntax"</b>
<h3>Solution</h3>


~~~

"use strict";

let number = 6;
for (let i = 1; i <=10; i++) {
    console.log(number + " X " + i + " = " + number*i);
}


~~~




<br><img src="https://user-images.githubusercontent.com/76753050/236971355-022486a9-ae18-40e8-848e-7cf303b1c825.png" alt="" width="450" height="250">

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
