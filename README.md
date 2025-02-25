<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Page</title>
    <script>
        // Function to validate login credentials
        function validateLogin() {
            var username = document.getElementById('username').value;
            var password = document.getElementById('password').value;

            // Check if username and password are 'pavan'
            if (username === 'pavan' && password === 'pavan') {
                // If correct, redirect to Snapchat's website
                window.location.href = 'https://www.snapchat.com';
            } else {
                alert('Invalid username or password.');
            }
        }
    </script>
</head>
<body>

    <h2>Login Page</h2>

    <form onsubmit="event.preventDefault(); validateLogin();">
        <label for="username">Username:</label><br>
        <input type="text" id="username" name="username" required><br><br>

        <label for="password">Password:</label><br>
        <input type="password" id="password" name="password" required><br><br>

        <button type="submit">Login</button>
    </form>

</body>
</html>
