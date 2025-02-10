TO KY
<!-- index.html (First Page) -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Be My Valentine?</title>
    <style>
        /* Styling for the first page */
        body {
            background-color: #FAD1D1; /* Light pink background */
            font-family: 'Arial', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            text-align: center;
        }

        h1 {
            color: #ff4d6d;
            font-size: 2.5em;
            margin-bottom: 40px;
        }

        button {
            padding: 15px 30px;
            font-size: 18px;
            margin: 20px;
            border: none;
            background-color: #ff4d6d;
            color: white;
            border-radius: 10px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        button:hover {
            background-color: #ff2a56;
        }
    </style>
</head>
<body>
    <div>
        <h1>Do you want to be my Valentine?</h1>
        <button onclick="answer('yes')">YESSS OFC</button>
        <button onclick="answer('no')">NO FUCK YOU</button>
    </div>

    <script>
        // Function to handle the user's answer
        function answer(choice) {
            if (choice === 'yes') {
                window.location.href = "love.html";  // Redirect to love page
            } else if (choice === 'no') {
                window.location.href = "hate.html";  // Redirect to hate page
            }
        }
    </script>
</body>
</html>

<!-- love.html (If 'YESSS OFC' is selected) -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>I Love You</title>
    <style>
        body {
            background-color: #FAD1D1;
            font-family: 'Arial', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            text-align: center;
        }

        h1 {
            color: #ff4d6d;
            font-size: 3em;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div>
        <h1>I LOVE YOU BBG</h1>
    </div>
</body>
</html>

<!-- hate.html (If 'NO FUCK YOU' is selected) -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Do You Hate Me?</title>
    <style>
        body {
            background-color: #FAD1D1;
            font-family: 'Arial', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            text-align: center;
        }

        h1 {
            color: #ff4d6d;
            font-size: 2.5em;
            margin-bottom: 30px;
        }

        button {
            padding: 15px 30px;
            font-size: 18px;
            margin: 20px;
            border: none;
            background-color: #ff4d6d;
            color: white;
            border-radius: 10px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        button:hover {
            background-color: #ff2a56;
        }
    </style>
</head>
<body>
    <div>
        <h1>Do u hate me or smth?</h1>
        <button onclick="finalAnswer()">YES</button>
    </div>

    <script>
        // Function for final answer redirection
        function finalAnswer() {
            window.location.href = "final.html";  // Redirect to final page
        }
    </script>
</body>
</html>

<!-- final.html (After the final answer is selected) -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Final Message</title>
    <style>
        body {
            background-color: #FAD1D1;
            font-family: 'Arial', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            text-align: center;
        }

        h1 {
            color: #ff4d6d;
            font-size: 1.8em;
            font-weight: bold;
            line-height: 1.5;
            white-space: pre-wrap;
        }
    </style>
</head>
<body>
    <div>
        <h1>Ik u playing right? right right right right right right right right right right right right right right right right right right right right right right right right right right right right right right</h1>
    </div>
</body>
</html>
