<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Không yêu em thì yêu ai</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffe4e1;
            margin: 0;
            padding: 0;
            overflow: hidden;
            position: relative;
        }
        h1 {
            color: #ff69b4;
        }
        p {
            font-size: 20px;
            margin: 10px 0;
        }
        .heart {
            color: #ff69b4;
            font-size: 50px;
        }
        .message {
            position: absolute;
            top: -50px;
            left: 50%;
            transform: translateX(-50%);
            display: none;
            color: #8b008b;
            font-size: 24px;
            animation: float 5s linear infinite;
            z-index: 2;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            background-color: #ff69b4;
            color: white;
            border: none;
            border-radius: 5px;
            margin: 10px;
            z-index: 2;
        }
        button:hover {
            background-color: #ff1493;
        }
        @keyframes float {
            0% {
                top: 100%;
                opacity: 0;
            }
            50% {
                opacity: 1;
            }
            100% {
                top: -50px;
                opacity: 0;
            }
        }
        #fireworks-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 1;
        }
        #question {
            margin-top: 20px;
        }
        #no-button {
            position: absolute;
        }
    </style>
    <script src="https://cdn.jsdelivr.net/npm/fireworks-js"></script>
</head>
<body>
    <h1>Ai Rít yêu Sông Tiền một chút xíuuuuu!<h1> 
    <p class="heart">❤️</p>
    <p>Thích nhìn embe cười👩‍❤️‍👨</p>
    
    <div class="message" id="message1">I love you *30000000000 🌻👩‍❤️‍👨</div>
    <div class="message" id="message2">Yêu ST một chút xíuuuu 🌞</div>
    <div class="message" id="message3">Mỗi ngày bên em là một món quà! 🎁</div>
    <div class="message" id="message4">Em chính là người tuyệt vời nhất! 🌟</div>
    <div class="message" id="message5">Yêu em nhiều hơn cả bầu trời! ✨</div>
    <div class="message" id="message6">Yêu cả bánh mì nữa </div>
    <div class="message" id="message7">KHÔNG YÊU EM THÌ YÊU AI </div>
    <div class="message" id="message1">I love you *30000000000 🌻👩‍❤️‍👨</div>
    <div class="message" id="message2">Yêu ST một chút xíuuuu 🌞</div>
    <div class="message" id="message3">🎁</div>
    <div class="message" id="message4">Em mười điểm 🌟</div>
    <div class="message" id="message5">Yêu em nhiều hơn cả bầu trời! ✨</div>
    <div class="message" id="message6">TLST người phụ nữ giàu có và bí ẩn quyền lực nhẩt thế giới</div>
    <div class="message" id="message7">Only youu </div>


    <div id="fireworks-container"></div>

    <div id="question">
        <p>Yêu em nhiều không?</p>
        <button id="yes-button">Có</button>
        <button id="no-button" onmouseover="moveNoButton()">Không</button>
    </div>

    <script>
        function showMessages() {
            var messages = document.getElementsByClassName('message');
            for (var i = 0; i < messages.length; i++) {
                messages[i].style.display = 'block';
                messages[i].style.left = (Math.random() * window.innerWidth) + 'px';
                messages[i].style.animationDelay = (Math.random() * 5) + 's';
            }
            startFireworks();
        }

        function startFireworks() {
            const container = document.getElementById('fireworks-container');
            const fireworks = new Fireworks(container, { 
                autoresize: true,
                opacity: 0.5,
                acceleration: 1.05,
                speed: 2,
                particles: 150
            });

            fireworks.start();
        }

        function moveNoButton() {
            var noButton = document.getElementById('no-button');
            noButton.style.left = Math.random() * (window.innerWidth - noButton.clientWidth) + 'px';
            noButton.style.top = Math.random() * (window.innerHeight - noButton.clientHeight) + 'px';
        }

        // Show messages and start fireworks on page load
        window.onload = showMessages;
    </script>
</body>
</html>
