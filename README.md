<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Be My Valentine?</title>
    <style>
        body {
            background-color: pink;
            text-align: center;
            font-family: 'Arial', sans-serif;
            color: white;
        }
        h1 {
            margin-top: 50px;
            font-size: 2.5em;
        }
        .heart {
            color: red;
            font-size: 50px;
            animation: heartbeat 1s infinite;
        }
        @keyframes heartbeat {
            0% { transform: scale(1); }
            50% { transform: scale(1.2); }
            100% { transform: scale(1); }
        }
        .buttons {
            margin-top: 30px;
        }
        button {
            font-size: 20px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
        }
        .yes-btn {
            background-color: red;
            color: white;
        }
        .yes-btn:hover {
            background-color: darkred;
        }
        .hidden {
            display: none;
            margin-top: 20px;
            font-size: 1.5em;
        }
    </style>
</head>
<body>
    <h1>Will You Be My Valentine? <span class="heart">❤️</span></h1>
    <div class="buttons">
        <button class="yes-btn" onclick="showMessage()">Yes!</button>
    </div>
    <div id="message" class="hidden">
        Yay! You just made me the happiest person ever! 💖🥰
    </div>
    <script>
        function showMessage() {
            document.getElementById('message').style.display = 'block';
        }
    </script>
</body>
</html>
