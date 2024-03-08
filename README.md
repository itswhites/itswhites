<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Emoji Calculator</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="calculator">
        <input type="text" id="display" disabled>
        <div class="buttons">
            <button onclick="addToDisplay('1')">1</button>
            <button onclick="addToDisplay('2')">2</button>
            <button onclick="addToDisplay('3')">3</button>
            <button onclick="addToDisplay('+')">+</button>
            <button onclick="addToDisplay('4')">4</button>
            <button onclick="addToDisplay('5')">5</button>
            <button onclick="addToDisplay('6')">6</button>
            <button onclick="addToDisplay('-')">-</button>
            <button onclick="addToDisplay('7')">7</button>
            <button onclick="addToDisplay('8')">8</button>
            <button onclick="addToDisplay('9')">9</button>
            <button onclick="addToDisplay('*')">*</button>
            <button onclick="addToDisplay('0')">0</button>
            <button onclick="addToDisplay('/')">/</button>
            <button onclick="calculate()">=</button>
            <button onclick="clearDisplay()">C</button>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Emoji Calculator</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="calculator">
        <input type="text" id="display" disabled>
        <div class="buttons">
            <button onclick="addToDisplay('1')">1</button>
            <button onclick="addToDisplay('2')">2</button>
            <button onclick="addToDisplay('3')">3</button>
            <button onclick="addToDisplay('+')">+</button>
            <button onclick="addToDisplay('4')">4</button>
            <button onclick="addToDisplay('5')">5</button>
            <button onclick="addToDisplay('6')">6</button>
            <button onclick="addToDisplay('-')">-</button>
            <button onclick="addToDisplay('7')">7</button>
            <button onclick="addToDisplay('8')">8</button>
            <button onclick="addToDisplay('9')">9</button>
            <button onclick="addToDisplay('*')">*</button>
            <button onclick="addToDisplay('0')">0</button>
            <button onclick="addToDisplay('/')">/</button>
            <button onclick="calculate()">=</button>
            <button onclick="clearDisplay()">C</button>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
.calculator {
    width: 300px;
    margin: 50px auto;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

#display {
    width: calc(100% - 10px);
    padding: 10px;
    margin-bottom: 10px;
}

.buttons {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 5px;
}

button {
    padding: 10px;
    font-size: 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    background-color: #f0f0f0;
}

button:hover {
    background-color: #ddd;
}
function addToDisplay(value) {
    document.getElementById('display').value += value;
}

function calculate() {
    var expression = document.getElementById('display').value;
    try {
        var result = eval(expression);
        document.getElementById('display').value = result;
    } catch (error) {
        document.getElementById('display').value = 'Error';
    }
}

function clearDisplay() {
    document.getElementById('display').value = '';
}
