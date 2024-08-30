<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple PHP App</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <h1>Welcome to My PHP App</h1>

        <form method="post" action="index.php">
            <label for="name">Your Name:</label>
            <input type="text" id="name" name="name" required>

            <button type="submit">Submit</button>
        </form>

        <?php
            if ($_SERVER['REQUEST_METHOD'] === 'POST') {
                $name = $_POST['name'];
                echo "<p>Hello, $name!</p>";
            }
        ?>
    </div>

    <script src="script.js"></script>
</body>
</html>
