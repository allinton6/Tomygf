<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Be My Valentine?</title>
    <style>
        /* General styling for the page */
        body {
            background-color: #FAD1D1; /* Light pink background */
            font-family: 'Arial', sans-serif;
            margin: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
        }

        h1 {
            color: #ff4d6d;
            font-size: 2.5em;
            margin-bottom: 40px;
        }

        .heart-container {
            width: 120px;
            height: 120px;
            position: relative;
            margin: 0 auto;
            margin-bottom: 50px;
        }

        .heart-container::before,
        .heart-container::after {
            content: '';
            width: 80px;
            height: 80px;
            background-color: #ff4d6d;
            border-radius: 50%;
            position: absolute;
            top: 0;
        }

        .heart-container::before {
            left: 0;
        }

        .heart-container::after {
            right: 0;
        }

        .heart-container .heart {
            width: 120px;
            height: 120px;
            background-color: transparent;
            border: 5px solid #ff4d6d;
            border-radius: 50%;
            position: absolute;
            top: 0;
            left: 50%;
            transform: translateX(-50%) rotate(45deg);
        }

        button {
            padding: 15px 30px;
            font-size: 18px;
            border: none;
            background-color: #ff4d6d;
            color: white;
            border-radius: 10px;
            cursor: pointer;
            transition: all 0.3s ease;
            margin: 10px;
        }

        button:hover {
            background-color: #ff2a56;
            transform: translateY(-5px);
        }

        .hidden {
            display: none;
        }

        .centered {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
        }

        /* Styling for individual page styles */
        .final-message {
            color: #ff4d6d;
            font-size: 2em;
            font-weight: bold;
        }

    </style>
</head>
<body>
    <div class="centered">
        <div class="heart-container">
            <div class="heart"></div>
        </div>
        <h1>Do you want to be my Valentine?</h1>
        <button onclick="answer('yes')">YES OFC</button>
        <button onclick="answer('no')">NO, FUCK YOU</button>
    </div>

    <script>
        // Function to handle answer choice
        function answer(choice) {
            if (choice === 'yes') {
                // Redirect to the love page
                window.location.href = "love.html";
            } else if (choice === 'no') {
                // Redirect to the 'No choice' page
                window.location.href = "no-choice.html";
            }
        }
    </script>
</body>
</html>

<!-- love.html -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>I Love You</title>
    <style>
        body {
            background-color: #FAD1D1; /* Light pink background */
            font-family: 'Arial', sans-serif;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            margin: 0;
        }

        h1 {
            color: #ff4d6d;
            font-size: 3em;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="centered">
        <h1>I LOVE YOU</h1>
    </div>
</body>
</html>

<!-- no-choice.html -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>You Have No Choice</title>
    <style>
        body {
            background-color: #FAD1D1;
            font-family: 'Arial', sans-serif;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            margin: 0;
        }

        h1 {
            color: #ff4d6d;
            font-size: 2.5em;
            font-weight: bold;
        }

        button {
            padding: 15px 30px;
            font-size: 18px;
            border: none;
            background-color: #ff4d6d;
            color: white;
            border-radius: 10px;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-top: 20px;
        }

        button:hover {
            background-color: #ff2a56;
            transform: translateY(-5px);
        }
    </style>
</head>
<body>
    <div class="centered">
        <h1>YOU HAVE NO CHOICE</h1>
        <button onclick="final()">YES</button>
    </div>

    <script>
        function final() {
            window.location.href = "final.html";
        }
    </script>
</body>
</html>

<!-- final.html -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Final Page</title>
    <style>
        body {
            background-color: #FAD1D1;
            font-family: 'Arial', sans-serif;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            margin: 0;
        }

        .final-message {
            color: #ff4d6d;
            font-size: 2.5em;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="centered">
        <h1 class="final-message">IK U HATE ME BUT I STILL LOVE YOU, MUAKS</h1>
    </div>
</body>
</html>
