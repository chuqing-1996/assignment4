<html>
<head>
    <meta charset="UTF-8">
    <title></title>
    <style>

        .container {
            width: 600px;
            height: 300px;
            margin: 0 auto;
            margin-top: 100px;
        }

        .num {
            border-radius: 7px;
            height: 35px;
            width: 120px;
        }


        .bb {
            width: 80px;
            height: 35px;
            border-radius: 7px;
            font-size: 20px;
            cursor: pointer;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>Welcome to HTML/CSS/JS play</h1>
       
        <input type="text" class="num" id="num1" value="" />       <input type="text" class="num" id="num2" value="" /> <br /><br />

        <input type="button" class="a bb" id="a" value="+" />
        <input type="button" class="b bb" id="b" value="-" />
        <input type="button" class="c bb" id="c" value="x" />
        <input type="button" class="d bb" id="d" value="÷" />
        <br />

        <p id="result">the result is 11</p>
    </div>


    <script>

        document.getElementById("a").addEventListener("click", function () {
            var num1 = document.getElementById("num1").value;
            var num2 = document.getElementById("num2").value;
            var result = Number(num1) + Number( num2);
            document.getElementById("result").innerHTML = "the result is " + result;
        });

        document.getElementById("b").addEventListener("click", function () {
            var num1 = document.getElementById("num1").value;
            var num2 = document.getElementById("num2").value;
            var result = Number(num1) - Number(num2);
            document.getElementById("result").innerHTML = "the result is " + result;
        });

        document.getElementById("c").addEventListener("click", function () {
            var num1 = document.getElementById("num1").value;
            var num2 = document.getElementById("num2").value;
            var result = Number(num1) * Number(num2);
            document.getElementById("result").innerHTML = "the result is " + result;
        });

        document.getElementById("d").addEventListener("click", function () {
            var num1 = document.getElementById("num1").value;
            var num2 = document.getElementById("num2").value;
            var result = Number(num1) / Number(num2);
            document.getElementById("result").innerHTML = "the result is " + result;
        });
    </script>
</body>
</html>
