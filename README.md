# Ex.08 Design of a Standard Calculator
## Date:25:04:2024

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Calculator</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="calculator">
    <div><center>M.SUREN(212223230222)</center></div>
    <input type="text" id="display" readonly>
    <div class="keys">
      <button onclick="appendToDisplay('7')">7</button>
      <button onclick="appendToDisplay('8')">8</button>
      <button onclick="appendToDisplay('9')">9</button>
      <button onclick="appendToDisplay('/')">/</button>
      <button onclick="appendToDisplay('4')">4</button>
      <button onclick="appendToDisplay('5')">5</button>
      <button onclick="appendToDisplay('6')">6</button>
      <button onclick="appendToDisplay('*')">*</button>
      <button onclick="appendToDisplay('1')">1</button>
      <button onclick="appendToDisplay('2')">2</button>
      <button onclick="appendToDisplay('3')">3</button>
      <button onclick="appendToDisplay('-')">-</button>
      <button onclick="appendToDisplay('0')">0</button>
      <button onclick="appendToDisplay('.')">.</button>
      <button onclick="clearDisplay()">C</button>
      <button onclick="calculate()">=</button>
      <button onclick="appendToDisplay('+')">+</button>
    </div>
  </div>
  <script src="index.js"></script>
</body>
</html>


function appendToDisplay(value) {
    document.getElementById('display').value += value;
  }
  
  function clearDisplay() {
    document.getElementById('display').value = '';
  }
  
  function calculate() {
    try {
      var result = eval(document.getElementById('display').value);
      document.getElementById('display').value = result;
    } catch (error) {
      document.getElementById('display').value = 'Error';
    }
  }
  


  .calculator {
    width: 250px;
    margin: 50px auto;
    border: 1px solid #6ddd3d;
    border-radius: 5px;
    padding: 5px;
    background-color: #d879dd;
  }
  
  #display {
    width: 90%;
    padding: 10px;
    margin-bottom: 10px;
  }
  
  .keys {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 5px;
  }
  
  button {
    padding: 15px;
    font-size: 18px;
    border: none;
    background-color: #ddd;
    cursor: pointer;
  }
  
  button:hover {
    background-color: #ccc;
  }
  
```

## OUTPUT:

![alt text](<Screenshot 2024-04-25 142028.png>)

## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
