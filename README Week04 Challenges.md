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
