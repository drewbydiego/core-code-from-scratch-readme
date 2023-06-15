<h1>Week #10 challenges</h1>
<h1>🧮 Work on the calculator project</h1>
<h1><a href="https://drewbydiego.github.io/BCalculator/">Calculadora</a></h1>
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/e629afc2-0226-42f1-accb-807d3daff657" alt="" width="600" height="300"><br><h1>CODE: </h1>

~~~javascript
let first = 0;
let second = 0;
let operation = "";
let error = false;
let op = false;
const calculator = document.querySelector(".calculator");
const display = calculator.querySelector(".display");
const buttons = calculator.querySelectorAll(".button");
const resul = document.getElementById("resul");
const btn_AC = document.getElementById("AC");
resul.addEventListener("click", () => {});

const del = document.getElementById("delete");
del.addEventListener("click", () => {
  display.innerHTML = eliminarUltimoDigito(display.innerHTML);
  first = 0;
});

function eliminarUltimoDigito(numero) {
  let absoluto = Math.abs(numero);
  let cadena = absoluto.toString();
  if (cadena.length > 1) {
    let subcadena = cadena.slice(0, -1);
    let nuevoNumero = parseFloat(subcadena);
    if (numero < 0) {
      nuevoNumero *= -1;
    }
    if (isNaN(nuevoNumero)) {
      return 0;
    } else {
      return nuevoNumero;
    }
  } else {
    return 0;
  }
}

btn_AC.addEventListener("click", () => {
  error = false;
  display.innerHTML = "0";
  first = 0;
  second = 0;
  resul.innerText = "0";
  btn_AC.classList.remove("toggle");
  op = false;
});

buttons.forEach((button) => {
  button.addEventListener("click", () => {
    if (error == true) {
      btn_AC.addEventListener("click", () => {
        error = false;
        op = false;
      });
    } else if (button.textContent == ".") {
      display.innerHTML = display.innerHTML + ".";
    } else {
      if (button.textContent == "+") {
        operation = "+";
        first = display.innerHTML;
        display.innerHTML = "+";
        op = false;
      } else if (
        button.textContent == "-" ||
        button.textContent.includes("-")
      ) {
        operation = "-";
        first = display.innerHTML;
        display.innerHTML = "-";
        op = false;
      } else if (button.textContent == "x") {
        operation = "x";
        first = display.innerHTML;
        display.innerHTML = "x";
        op = false;
      } else if (button.innerHTML == "/") {
        operation = "/";
        first = display.innerHTML;
        display.innerHTML = "/";
        op = false;
      } else if (button.innerHTML == "%") {
        operation = "%";
        first = display.innerHTML;
        display.innerHTML = "%";
        op = false;
      } else if (button.textContent == "±" && display.innerHTML != "0") {
        operation = "±";
        first = display.innerHTML;
        display.innerHTML = "±";
        op = false;
        display.innerHTML = calcularOperacion(parseFloat(first), 0, operation);
      } else if (button.textContent == "=") {
        second = display.innerHTML;
        if (isNaN(second)) {
        } else {
          if (op == false) {
            display.innerHTML = calcularOperacion(
              parseFloat(first),
              parseFloat(second),
              operation
            );

            if (isNaN(second)) {
              resul.innerText = first + " " + operation + " " + " =";
            } else {
              resul.innerText =
                first + " " + operation + " " + Math.abs(second) + " =";
            }
            //first = 0;
            op = true;
          }
        }
      } else {
        if (
          display.innerHTML == "+" ||
          display.innerHTML == "x" ||
          display.innerHTML == "/" ||
          display.innerHTML == "%" ||
          display.innerHTML == "±"
        ) {
          display.innerHTML = "";
        }
        if (display.innerHTML == "0") {
          display.innerHTML = parseInt(
            display.innerHTML + button.textContent.toString(),
            10
          );
        } else {
          display.innerHTML = display.innerHTML + button.textContent;
        }
      }
    }
  }); //Cierre click
});

function calcularOperacion(n1, n2, operation) {
  let resultado;
  switch (operation) {
    case "+":
      resultado = n1 + n2;
      break;
    case "-":
      resultado = n1 - Math.abs(n2);
      break;
    case "x":
      resultado = n1 * n2;
      break;
    case "/":
      if (n2 == 0) {
        resultado = "ERROR";
        error = true;
        btn_AC.classList.toggle("toggle");
      } else {
        resultado = n1 / n2;
      }
      break;
    case "±":
      resultado = -n1;
      break;
    case "%":
      resultado = (n1 / 100) * n2;
      break;
    default:
      console.log("Operación inválida");
      return;
  }
  //return resultado.toFixed(2);
  return resultado;
}
~~~
