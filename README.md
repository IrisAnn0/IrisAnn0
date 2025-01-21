&lt;!DOCTYPE html&gt;
&lt;html lang=&quot;vi&quot;&gt;
&lt;head&gt;
    &lt;meta charset=&quot;UTF-8&quot;&gt;
    &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;
    &lt;title&gt;Không yêu em thì yêu ai&lt;/title&gt;
    &lt;style&gt;
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
    &lt;/style&gt;
    &lt;script src=&quot;https://cdn.jsdelivr.net/npm/fireworks-js&quot;&gt;&lt;/script&gt;
&lt;/head&gt;
&lt;body&gt;
    &lt;h1&gt;Ai Rít yêu Sông Tiền một chút xíuuuuu!&lt;/h1&gt; 
    &lt;p class=&quot;heart&quot;&gt;❤️&lt;/p&gt;
    &lt;p&gt;Thích nhìn embe cười👩‍❤️‍👨&lt;/p&gt;
    
    &lt;div class=&quot;message&quot; id=&quot;message1&quot;&gt;I love you *30000000000 🌻👩‍❤️‍👨&lt;/div&gt;
    &lt;div class=&quot;message&quot; id=&quot;message2&quot;&gt;Yêu ST một chút xíuuuu 🌞&lt;/div&gt;
    &lt;div class=&quot;message&quot; id=&quot;message3&quot;&gt;Mỗi ngày bên em là một món quà! 🎁&lt;/div&gt;
    &lt;div class=&quot;message&quot; id=&quot;message4&quot;&gt;Em chính là người tuyệt vời nhất! 🌟&lt;/div&gt;
    &lt;div class=&quot;message&quot; id=&quot;message5&quot;&gt;Yêu em nhiều hơn cả bầu trời! ✨&lt;/div&gt;
    &lt;div class=&quot;message&quot; id=&quot;message6&quot;&gt;Yêu cả bánh mì nữa &lt;/div&gt;
    &lt;div class=&quot;message&quot; id=&quot;message7&quot;&gt;KHÔNG YÊU EM THÌ YÊU AI &lt;/div&gt;
    &lt;div class=&quot;message&quot; id=&quot;message1&quot;&gt;I love you *30000000000 🌻👩‍❤️‍👨&lt;/div&gt;
    &lt;div class=&quot;message&quot; id=&quot;message2&quot;&gt;Yêu ST một chút xíuuuu 🌞&lt;/div&gt;
    &lt;div class=&quot;message&quot; id=&quot;message3&quot;&gt;🎁&lt;/div&gt;
    &lt;div class=&quot;message&quot; id=&quot;message4&quot;&gt;Em mười điểm 🌟&lt;/div&gt;
    &lt;div class=&quot;message&quot; id=&quot;message5&quot;&gt;Yêu em nhiều hơn cả bầu trời! ✨&lt;/div&gt;
    &lt;div class=&quot;message&quot; id=&quot;message6&quot;&gt;TLST người phụ nữ giàu có và bí ẩn quyền lực nhẩt thế giới&lt;/div&gt;
    &lt;div class=&quot;message&quot; id=&quot;message7&quot;&gt;Only youu &lt;/div&gt;


    &lt;div id=&quot;fireworks-container&quot;&gt;&lt;/div&gt;

    &lt;div id=&quot;question&quot;&gt;
        &lt;p&gt;Yêu em nhiều không?&lt;/p&gt;
        &lt;button id=&quot;yes-button&quot;&gt;Có&lt;/button&gt;
        &lt;button id=&quot;no-button&quot; onmouseover=&quot;moveNoButton()&quot;&gt;Không&lt;/button&gt;
    &lt;/div&gt;

    &lt;script&gt;
        function showMessages() {
            var messages = document.getElementsByClassName('message');
            for (var i = 0; i &lt; messages.length; i++) {
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
    &lt;/script&gt;
&lt;/body&gt;
&lt;/html&gt;
