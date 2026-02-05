# calc-
<!DOCTYPE html>
<html lang="kk">
<head>
    <meta charset="UTF-8">
    <title>Калькулятор</title>

    <script>
        function calc(op) {
            var a = Number(document.getElementById("n1").value);
            var b = Number(document.getElementById("n2").value);
            var r = document.getElementById("res");

            if(op == "+") r.value = a + b;
            if(op == "-") r.value = a - b;
            if(op == "*") r.value = a * b;
            if(op == "/") r.value = a / b;
        }

        function clearAll() {
            document.getElementById("n1").value = "";
            document.getElementById("n2").value = "";
            document.getElementById("res").value = "";
        }
    </script>
</head>

<body>

<h2>Калькулятор</h2>

Сан 1: <input type="number" id="n1"><br><br>
Сан 2: <input type="number" id="n2"><br><br>

<button onclick="calc('+')">+</button>
<button onclick="calc('-')">-</button>
<button onclick="calc('*')">*</button>
<button onclick="calc('/')">/</button>
<button onclick="clearAll()">C</button>

<br><br>

Нәтиже: <input type="text" id="res" readonly>

</body>
</html>
