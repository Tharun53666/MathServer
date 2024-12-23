# Ex.05 Design a Website for Server Side Processing
## Date:22-12-2024

## AIM:
 To design a website to calculate the power of a lamp filament in an incandescent bulb in the server side. 


## FORMULA:
P = I<sup>2</sup>R
<br> P --> Power (in watts)
<br> I --> Intensity
<br> R --> Resistance

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
'''
math.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lamp Power Calculator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            color: #333;
            margin: 0;
            padding: 20px;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        h1 {
            color: #2c3e50;
        }

        label {
            font-weight: bold;
            display: block;
            margin-top: 10px;
        }

        input[type="number"] {
            width: 100%;
            padding: 8px;
            margin-top: 5px;
            margin-bottom: 15px;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 16px;
        }

        button {
            background-color: #3498db;
            color: #fff;
            border: none;
            padding: 10px 15px;
            border-radius: 5px;
            font-size: 16px;
            cursor: pointer;
        }

        button:hover {
            background-color: #2980b9;
        }

        #result {
            margin-top: 20px;
            font-size: 18px;
            color: #27ae60;
            font-weight: bold;
        }

        .container {
            background: #fff;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            max-width: 400px;
            width: 100%;
        }
    </style>
    <script>
        function calculatePower() {
            var I = parseFloat(document.getElementById("current").value);
            var R = parseFloat(document.getElementById("resistance").value);
            if (isNaN(I) || isNaN(R)) {
                document.getElementById("result").innerHTML = "Please enter valid numbers for current and resistance.";
                return;
            }
            var P = Math.pow(I, 2) * R;
            document.getElementById("result").innerHTML = "Power (P) = " + P.toFixed(4) + " Watts";
        }
    </script>
</head>
<body>
    <div class="container">
        <h1>Lamp Power Calculator</h1>
        <label for="current">Current (I) in Amps:</label>
        <input type="number" id="current" step="any">
        <label for="resistance">Resistance (R) in Ohms:</label>
        <input type="number" id="resistance" step="any">
        <button onclick="calculatePower()">Calculate Power</button>
        <div id="result"></div>
    </div>
</body>
</html>

'''


## SERVER SIDE PROCESSING:


## HOMEPAGE:

![alt text](<../WhatsApp Image 2024-12-23 at 11.27.08_ddd7e63b.jpg>)

## RESULT:
The program for performing server side processing is completed successfully.
