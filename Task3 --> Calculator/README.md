<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="wclassth=device-wclassth, initial-scale=1.0">
    <title>Calculator</title>
    <style>
        body {
            background-color: rgb(199, 192, 192);
        }

        .structure {
            position: absolute;
        }

        .calcul {
            position: relative;
            height: 560px;
            width: 350px;
            background-color: #434343;
            border-radius: 30px;
            border: 5px solid #434343;
            box-shadow: 10px 2px 35px #434343;
            padding: 20px;
        }

        .screen {
            position: relative;
            top: 10px;
            left: 7px;
            height: 90px;
            width: 320px;
            border-radius: 4px;
            background-color: #a9b27d;
            margin-bottom: 20px;
            font-size: 36px;
            text-align: right;
            padding: 10px;
            overflow-x: auto;
        }

        .clean {
            position: relative;
            top: 8px;
            left: 8px;
            height: 60px;
            width: 55px;
            background-color: #393838;
            color: whitesmoke;
            font-weight: bolder;
            justify-content: space-evenly;
            margin: 13.5px;
            font-size: 18px;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            box-shadow: -1px 8px 15px #1d1c1c;
        }

        .clean:active {
            background-color: #474545;
            box-shadow: 0px 3px 0px rgb(85, 73, 73);
        }
    </style>
</head>

<body>
    <div class="structure">
        <div class="calcul">
            <div class="screen" id="screen"></div>
            <button class="clean">C</button>
            <button class="clean">⟵</button>
            <button class="clean">%</button>
            <button class="clean" style="background-color: orange;">/</button>

            <button class="clean">7</button>
            <button class="clean">8</button>
            <button class="clean">9</button>
            <button class="clean" style="background-color: orange;">*</button>

            <button class="clean">4</button>
            <button class="clean">5</button>
            <button class="clean">6</button>
            <button class="clean" style="background-color: orange;">-</button>

            <button class="clean">1</button>
            <button class="clean">2</button>
            <button class="clean">3</button>
            <button class="clean" style="background-color: orange;">+</button>

            <button class="clean" style="width: 138px;">0</button>
            <button class="clean">.</button>
            <button class="clean" style="background-color: orange;">=</button>
        </div>
    </div>

    <script>
        let screen = document.getElementById("screen");
        let buttons = document.querySelectorAll(".clean");
        let screenValue = "";

        buttons.forEach(button => {
            button.addEventListener("click", (e) => {
                let buttonText = e.target.innerText;

                if (buttonText === "C") {
                    screenValue = "";
                    screen.innerText = "";
                }
                else if (buttonText === "⟵") {
                    screenValue = screenValue.slice(0, -1);
                    screen.innerText = screenValue;
                }
                else if (buttonText === "=") {
                    try {
                        screenValue = eval(screenValue);
                        screen.innerText = screenValue;
                    } catch {
                        screen.innerText = "Error";
                        screenValue = "";
                    }
                }
                else {
                    screenValue += buttonText;
                    screen.innerText = screenValue;
                }
            });
        });
    </script>
</body>

</html>
