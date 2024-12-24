<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Welcome to My Little Website</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(to bottom right, #ffe4e1, #add8e6);
            color: #333;
            margin: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
        }
        h1 {
            font-size: 3em;
            color: #6a5acd;
            text-shadow: 2px 2px #fff;
        }
        p {
            font-size: 1.2em;
            margin: 15px 0;
        }
        button {
            padding: 10px 20px;
            font-size: 1em;
            color: white;
            background-color: #6a5acd;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        button:hover {
            background-color: #836fff;
        }
        .game-section {
            margin-top: 30px;
            text-align: center;
        }
        .output {
            margin-top: 20px;
            font-size: 1.5em;
            color: #ff4500;
        }
    </style>
</head>
<body>
    <h1>Welcome to My Little Website</h1>
    <p>Feel free to explore and have fun!</p>

    <div class="game-section">
        <h2>Interactive Game: Random Number Generator</h2>
        <p>Click the button to generate a random number between 1 and 100:</p>
        <button id="randomNumberButton">Generate Number</button>
        <div class="output" id="output"></div>
    </div>

    <script>
        const button = document.getElementById('randomNumberButton');
        const output = document.getElementById('output');

        button.addEventListener('click', () => {
            const randomNumber = Math.floor(Math.random() * 100) + 1;
            output.textContent = `Your random number is: ${randomNumber}`;
        });
    </script>
</body>
</html>
