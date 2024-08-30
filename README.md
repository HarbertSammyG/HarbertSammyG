<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple PHP App</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        .container {
            margin-top: 50px;
        }
        h1 {
            color: #333;
        }
        p {
            color: #666;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Welcome to My PHP App</h1>
        <p>This is a simple PHP application with HTML, CSS, and JavaScript.</p>
        <button onclick="displayMessage()">Click Me</button>
        <p id="message"></p>
    </div>
    
    <script>
        function displayMessage() {
            document.getElementById('message').innerHTML = "Hello, this is JavaScript in action!";
        }
    </script>
    
    <?php
        echo "<p>This is a message from the server-side PHP script.</p>";
    ?>
</body>
</html>
