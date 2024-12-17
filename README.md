<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>tahmid mahdi search engine</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f4f4f4;
        }
        .search-container {
            text-align: center;
        }
        input[type="text"] {
            width: 300px;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        input[type="submit"] {
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            background-color: #4CAF50;
            color: white;
            cursor: pointer;
        }
        input[type="submit"]:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <div class="search-container">
        <h1>tahmid mahdi search engine</h1>
        <form action="https://www.bing.com/search" method="get">
            <input type="text" name="q" placeholder="Search...">
            <input type="submit" value="Search">
        </form>
    </div>
</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LOL</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        .container {
            text-align: center;
        }
        .animated-box {
            width: 100px;
            height: 100px;
            background-color: #4CAF50;
            margin: 20px auto;
            animation: bounce 2s infinite;
        }
        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% {
                transform: translateY(0);
            }
            40% {
                transform: translateY(-150px);
            }
            60% {
                transform: translateY(-75px);
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Welcome to Tahmid Mahdi Search Engine!</h1>
        <div class="animated-box"></div>
        <p>Copilot Made This Site      Powered By Bing</p>
    </div>
</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fun Things Is Here!</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f4f4f4;
        }
        canvas {
            border: 1px solid #000;
        }
        .controls {
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Fun Things Is Here!</h1>
        <canvas id="paintCanvas" width="500" height="500"></canvas>
        <div class="controls">
            <button onclick="clearCanvas()">Clear</button>
        </div>
    </div>
    <script>
        const canvas = document.getElementById('paintCanvas');
        const ctx = canvas.getContext('2d');
        let painting = false;

        function startPosition(e) {
            painting = true;
            draw(e);
        }

        function endPosition() {
            painting = false;
            ctx.beginPath();
        }

        function draw(e) {
            if (!painting) return;
            ctx.lineWidth = 5;
            ctx.lineCap = 'round';
            ctx.strokeStyle = 'black';

            ctx.lineTo(e.clientX - canvas.offsetLeft, e.clientY - canvas.offsetTop);
            ctx.stroke();
            ctx.beginPath();
            ctx.moveTo(e.clientX - canvas.offsetLeft, e.clientY - canvas.offsetTop);
        }

        function clearCanvas() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);
        }

        canvas.addEventListener('mousedown', startPosition);
        canvas.addEventListener('mouseup', endPosition);
        canvas.addEventListener('mousemove', draw);
    </script>
</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Button Example</title>


