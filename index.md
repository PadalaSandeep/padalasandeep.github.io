<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kushi SPA</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f0f0f0;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            overflow: hidden;
        }
        
        #kushi-name {
            font-size: 36px;
            cursor: pointer;
            transition: color 0.3s;
            z-index: 1;
        }

        #kushi-name:hover {
            color: red;
        }

        #hearts-and-messages {
            position: relative;
            display: flex;
            flex-direction: row;
            justify-content: center;
            align-items: center;
            pointer-events: none;
        }

        .heart {
            font-size: 48px;
            margin: 20px;
            animation: beat 1s infinite;
            pointer-events: none;
            transition: color 1s ease-in-out;
        }

        .message {
            font-size: 24px;
            color: green;
            margin: 20px;
            pointer-events: none;
            transition: color 1s ease-in-out;
        }

        @keyframes beat {
            0%, 100% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.2);
            }
        }
    </style>
</head>
<body>
    <div id="kushi-name" onclick="showHeart()">Kushi</div>
    <div id="hearts-and-messages"></div>

    <script>
        const messages = [
            "Take care My SweetHeart",
            "You have a Million Dollar Smile, Smile Da eeeeeee",
            "One in a Billion Soul",
            "Sending all the love for speedy recovery"
        ];

        function getRandomElement(arr) {
            return arr[Math.floor(Math.random() * arr.length)];
        }

        function getRandomColor() {
            const letters = '0123456789ABCDEF';
            let color = '#';
            for (let i = 0; i < 6; i++) {
                color += letters[Math.floor(Math.random() * 16)];
            }
            return color;
        }

        function showHeart() {
            const heartsAndMessages = document.getElementById("hearts-and-messages");
            
            const randomMessage = getRandomElement(messages);
            const randomHeartColor = getRandomColor();
            const randomMessageColor = getRandomColor();

            const message = document.createElement("div");
            message.className = "message";
            message.textContent = randomMessage;
            message.style.color = randomMessageColor;

            const heart = document.createElement("div");
            heart.className = "heart";
            heart.textContent = "❤️";
            heart.style.color = randomHeartColor;

            heartsAndMessages.innerHTML = ""; // Clear previous hearts and messages

            heartsAndMessages.appendChild(message);
            heartsAndMessages.appendChild(heart);
        }
    </script>
</body>
</html>
