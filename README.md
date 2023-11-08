# operaciones
nuevo trabajo
<!DOCTYPE html>
<html>
<head>
    <title>Calculadora</title>
</head>
<body>
    <h1>Calculadora Simple</h1>
    
    <p>Introduce dos números:</p>
    <input type="text" id="num1" placeholder="Número 1">
    <input type="text" id="num2" placeholder="Número 2">
    
    <button onclick="multiplicar()">Multiplicar</button>
    <button onclick="dividir()">Dividir</button>
    
    <p>Resultado: <span id="resultado"></span></p>
    
    <script>
        function multiplicar() {
            var num1 = parseFloat(document.getElementById('num1').value);
            var num2 = parseFloat(document.getElementById('num2').value);
            var resultado = num1 * num2;
            document.getElementById('resultado').textContent = resultado;
        }

        function dividir() {
            var num1 = parseFloat(document.getElementById('num1').value);
            var num2 = parseFloat(document.getElementById('num2').value);
            if (num2 !== 0) {
                var resultado = num1 / num2;
                document.getElementById('resultado').textContent = resultado;
            } else {
                document.getElementById('resultado').textContent = "No se puede dividir por cero.";
            }
        }
    </script>
</body>
</html>
