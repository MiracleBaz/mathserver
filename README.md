# Ex.05 Design a Website for Server Side Processing
# Date:
# AIM:
To design a website to calculate the power of a lamp filament in an incandescent bulb in the server side.

# FORMULA:
P = I2R
P --> Power (in watts)
 I --> Intensity
 R --> Resistance

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Create python programs for views and urls to perform server side processing.

## Step 5:
Create a HTML file to implement form based input and output.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lamp Filament Power Calculator</title>
    <link rel="stylesheet" href="server.css">

    <script>
        function power()
        {
            var i = Number(document.getElementById('t1').value);
            var r = Number(document.getElementById('t2').value);
            var p = i*i*r;
            document.getElementById('power').innerText="Power of Lamp = "+p;
            
        }
    </script>
</head>
<body>
    <header>
        <h1>Lamp Filament Power Calculator</h1>
        <p>Calculate the power of your lamp filament quickly and easily.</p>
    </header>
        <div class="Calculate">
            <br><br>
            <p>POWER OF LAMP FILAMENT </p><p>CALCULATOR<p>
            <form>
                <input type="number" placeholder="Enter Intensity" id="t1"><br><br>
                <input type="number" placeholder="Enter Resistance" id="t2"><br><br>
                <input type="button" value="Calculate Power" onclick="power()"><br><br>
                <label id="power"></label>
            </form>
        </div>
</body>
</html>

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    text-align: center;
    font-size: 30px;
}

header {
    background-color:#333;
    color: white;
    padding: 20px;
}

main {
    padding: 20px;
}

form {
    margin: 20px auto;
    max-width: 300px;
}

label, input {
    display: block;
    margin: 10px 0;
}

input {
    padding: 5px;
    width: 100%;
}

button {
    background-color:#333;
    color: white;
    padding: 10px;
    border: none;
    cursor: pointer;
}

button:hover {
    background-color:#333;
}

#result {
    margin-top: 20px;
    font-size: 1.2em;
}
```
# SERVER SIDE PROCESSING:

![alt text](<Screenshot 2024-12-22 185718.png>)

# HOMEPAGE:

![alt text](<Screenshot 2024-12-23 083212.png>)

![alt text](<Screenshot 2024-12-22 182828.png>)

# RESULT:
The program for performing server side processing is completed successfully.
