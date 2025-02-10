TO KY
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
            flex-direction: column;
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

        /* Hidden content styling */
        .hidden {
            display: none;
        }

        .centered {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
        }

        .final-message {
            color: #ff4d6d;
            font-size: 1.8em;
            font-weight: bold;
            white-space: pre-wrap;
        }

        /* Styling for the heart outline */
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

    </style>
</head>
<body>

    <div id="first-question" class="centered">
        <div class="heart-container">
            <div class="heart"></div>
        </div>
        <h1>Do you want to be my Valentine?</h1>
        <button onclick="answer('yes')">YESSS OFC</button>
        <button onclick="answer('no')">NO FUCK YOU</button>
    </div>

    <div id="second-question" class="hidden centered">
        <h1>Do u hate me or smth?</h1>
        <button onclick="finalAnswer()">YES</button>
    </div>

    <div id="love-message" class="hidden centered">
        <h1>I LOVE YOU BBG</h1>
    </div>

    <div id="final-message" class="hidden centered">
        <h1 class="final-message">Ik u playing right? right right right right right right right right right right right right right right right right right right right right right right right right right right right right right</h1>
    </div>

    <script>
        function answer(choice) {
            if (choice === 'yes') {
                document.getElementById('first-question').classList.add('hidden');
                document.getElementById('love-message').classList.remove('hidden');
            } else if (choice === 'no') {
                document.getElementById('first-question').classList.add('hidden');
                document.getElementById('second-question').classList.remove('hidden');
            }
        }

        function finalAnswer() {
            document.getElementById('second-question').classList.add('hidden');
            document.getElementById('final-message').classList.remove('hidden');
        }
    </script>

</body>
</html>
