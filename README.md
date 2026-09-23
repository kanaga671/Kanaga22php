# Kanaga22php
<?php

$correctUsername = "student";
$correctPassword = "12345";

if ($_SERVER["REQUEST_METHOD"] == "POST") {

    $username = $_POST["username"];
    $password = $_POST["password"];

    if ($username == $correctUsername && $password == $correctPassword) {
        echo "<h2>Login Successful!</h2>";
        echo "Welcome, " . $username;
    } 
    else {
        echo "<h2>Invalid Username or Password</h2>";
    }
}

?>

<!DOCTYPE html>
<html>
<head>
    <title>College Student Login</title>
</head>

<body>

<h2>College Student Login</h2>

<form method="post">

    <label>Username:</label>
    <input type="text" name="username" required>
    <br><br>

    <label>Password:</label>
    <input type="password" name="password" required>
    <br><br>

    <input type="submit" value="Login">

</form>

</body>
</html>
Username: student
Password: 12345
