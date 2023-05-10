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


<h2>Weather average ☁️</h2>
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

