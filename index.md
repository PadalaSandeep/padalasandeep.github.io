<html>
<head>
    <title>Love Symbol</title>
    <style>
        #loveSymbol {
            font-size: 50px;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div id="loveSymbol" onclick="createLoveSymbol()">Kushi</div>

    <script>
        function createLoveSymbol() {
            const loveSymbol = document.createElement('div');
            loveSymbol.innerHTML = '&#10084; Kushi'; // HTML entity for heart symbol

            loveSymbol.style.position = 'absolute';
            loveSymbol.style.top = Math.random() * (window.innerHeight - 100) + 'px';
            loveSymbol.style.left = Math.random() * (window.innerWidth - 100) + 'px';
            loveSymbol.style.color = getRandomColor();

            document.body.appendChild(loveSymbol);
        }

        function getRandomColor() {
            const letters = '0123456789ABCDEF';
            let color = '#';
            for (let i = 0; i < 6; i++) {
                color += letters[Math.floor(Math.random() * 16)];
            }
            return color;
        }
    </script>
</body>
</html>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
