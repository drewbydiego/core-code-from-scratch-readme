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
