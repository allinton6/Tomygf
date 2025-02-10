# Tomygf
To kaiyi

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Be My Valentine?</title>
    <style>
        body {
            background-color: #FFC0CB; /* Light Pink Background */
            text-align: center;
            font-family: Arial, sans-serif;
            margin: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        h1 {
            color: #ff66b2;
            font-size: 3em;
        }

        .heart-outline {
            width: 100px;
            height: 100px;
            border: 5px solid #ff66b2;
            border-radius: 50%;
            position: absolute;
            top: 20%;
            left: 50%;
            transform: translateX(-50%);
            margin-top: 50px;
        }

        .heart-outline:before {
            content: "";
            position: absolute;
            width: 70px;
            height: 70px;
            background-color: #ff66b2;
            border-radius: 50%;
            top: -35px;
            left: 15px;
        }

        .heart-outline:after {
            content: "";
            position: absolute;
            width: 70px;
            height: 70px;
            background-color: #ff66b2;
            border-radius: 50%;
            top: -35px;
            right: 15px;
        }

        .btn {
            padding: 20px 40px;
            font-size: 20px;
            margin: 20px;
            cursor: pointer;
            background-color: #ff66b2;
            color: white;
            border: none;
            border-radius: 10px;
        }

        .btn:hover {
            background-color: #ff3399;
        }

        .centered {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
        }

        .hidden {
            display: none;
        }
    </style>
</head>
<body>
    <div class="heart-outline"></div>
    <div class="centered">
        <h1>Do you want to be my Valentine?</h1>
        <button class="btn" onclick="answer('yes')">YES OFC</button>
        <button class="btn" onclick="answer('no')">NO FUCK YOU</button>
    </div>

    <script>
        function answer(choice) {
            if (choice === 'yes') {
                // Redirect to the 'I love you' page
                window.location.href = "love.html";
            } else if (choice === 'no') {
                // Redirect to the 'You have no choice' page
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
            background-color: #FFC0CB; /* Light Pink Background */
            text-align: center;
            font-family: Arial, sans-serif;
            margin: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        h1 {
            color: #ff66b2;
            font-size: 3em;
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
            background-color: #FFC0CB; /* Light Pink Background */
            text-align: center;
            font-family: Arial, sans-serif;
            margin: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        h1 {
            color: #ff66b2;
            font-size: 2.5em;
        }

        .btn {
            padding: 20px 40px;
            font-size: 20px;
            margin: 20px;
            cursor: pointer;
            background-color: #ff66b2;
            color: white;
            border: none;
            border-radius: 10px;
        }

        .btn:hover {
            background-color: #ff3399;
        }
    </style>
</head>
<body>
    <div class="centered">
        <h1>YOU HAVE NO CHOICE</h1>
        <button class="btn" onclick="final()">YES</button>
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
            background-color: #FFC0CB; /* Light Pink Background */
            text-align: center;
            font-family: Arial, sans-serif;
            margin: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        h1 {
            color: #ff66b2;
            font-size: 2.5em;
        }
    </style>
</head>
<body>
    <div class="centered">
        <h1>IK U HATE ME BUT I STILL LOVE YOU, MUAKS</h1>
    </div>
</body>
</html>


      
