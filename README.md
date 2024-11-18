<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Defective Application</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        h1, h2 {
            color: #333;
        }
        form {
            max-width: 600px;
            margin: auto;
        }
        label {
            display: block;
            margin: 10px 0 5px;
        }
        input, select {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        button {
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <h1>Defective Application</h1>
    <form id="defectiveForm">
        <label for="username">Username</label>
        <input type="text" id="username" name="username">

        <label for="password">Password</label>
        <input type="password" id="password" name="password">

        <label for="email">Email</label>
        <input type="text" id="email" name="email">

        <label for="age">Age</label>
        <input type="number" id="age" name="age" min="1" max="100">

        <label for="gender">Gender</label>
        <select id="gender" name="gender">
            <option value="">Select</option>
            <option value="male">Male</option>
            <option value="female">Female</option>
            <option value="other">Other</option>
        </select>

        <label for="country">Country</label>
        <input type="text" id="country" name="country">

        <button type="submit">Submit</button>
    </form>

    <script>
        document.getElementById('defectiveForm').addEventListener('submit', function(event) {
            event.preventDefault();
            alert('Form submitted successfully!');
        });
    </script>
</body>
</html>
