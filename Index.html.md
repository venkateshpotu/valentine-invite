<!DOCTYPE html>  
<html lang="en">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Valentine's Day Invitation 💝</title>  
    <style>  
        * {  
            margin: 0;  
            padding: 0;  
            box-sizing: border-box;  
        }  
  
        body {  
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;  
            min-height: 100vh;  
            display: flex;  
            justify-content: center;  
            align-items: center;  
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);  
            overflow: hidden;  
            position: relative;  
        }  
  
        .heart-bg {  
            position: absolute;  
            width: 100%;  
            height: 100%;  
            overflow: hidden;  
            z-index: 0;  
        }  
  
        .floating-heart {  
            position: absolute;  
            font-size: 20px;  
            animation: float-up 15s infinite ease-in;  
            opacity: 0;  
        }  
  
        @keyframes float-up {  
            0% {  
                transform: translateY(100vh) rotate(0deg);  
                opacity: 0;  
            }  
            10% {  
                opacity: 0.6;  
            }  
            90% {  
                opacity: 0.6;  
            }  
            100% {  
                transform: translateY(-100vh) rotate(360deg);  
                opacity: 0;  
            }  
        }  
  
        .container {  
            background: rgba(255, 255, 255, 0.95);  
            padding: 60px 50px;  
            border-radius: 30px;  
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);  
            text-align: center;  
            max-width: 500px;  
            width: 90%;  
            position: relative;  
            z-index: 1;  
            animation: slideIn 0.8s ease-out;  
        }  
  
        @keyframes slideIn {  
            from {  
                transform: translateY(-50px);  
                opacity: 0;  
            }  
            to {  
                transform: translateY(0);  
                opacity: 1;  
            }  
        }  
  
        .heart-icon {  
            font-size: 80px;  
            margin-bottom: 20px;  
            animation: heartbeat 1.5s infinite;  
        }  
  
        @keyframes heartbeat {  
            0%, 100% {  
                transform: scale(1);  
            }  
            10%, 30% {  
                transform: scale(1.1);  
            }  
            20%, 40% {  
                transform: scale(1);  
            }  
        }  
  
        h1 {  
            color: #e91e63;  
            font-size: 36px;  
            margin-bottom: 20px;  
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);  
        }  
  
        .message {  
            color: #555;  
            font-size: 20px;  
            margin-bottom: 40px;  
            line-height: 1.6;  
        }  
  
        .buttons {  
            display: flex;  
            gap: 20px;  
            justify-content: center;  
            position: relative;  
            height: 120px;  
            align-items: center;  
        }  
  
        button {  
            padding: 18px 45px;  
            font-size: 20px;  
            font-weight: bold;  
            border: none;  
            border-radius: 50px;  
            cursor: pointer;  
            transition: all 0.3s ease;  
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);  
        }  
  
        .yes-btn {  
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);  
            color: white;  
        }  
  
        .yes-btn:hover {  
            transform: scale(1.1);  
            box-shadow: 0 6px 20px rgba(245, 87, 108, 0.4);  
        }  
  
        .no-btn {  
            background: linear-gradient(135deg, #a8edea 0%, #fed6e3 100%);  
            color: #666;  
            position: absolute;  
        }  
  
        .celebration {  
            position: fixed;  
            top: 0;  
            left: 0;  
            width: 100%;  
            height: 100%;  
            background: rgba(0, 0, 0, 0.8);  
            display: none;  
            justify-content: center;  
            align-items: center;  
            z-index: 1000;  
            animation: fadeIn 0.5s ease-out;  
        }  
  
        @keyframes fadeIn {  
            from { opacity: 0; }  
            to { opacity: 1; }  
        }  
  
        .celebration-content {  
            background: white;  
            padding: 60px 40px;  
            border-radius: 30px;  
            text-align: center;  
            max-width: 600px;  
            width: 90%;  
            position: relative;  
            animation: popIn 0.6s cubic-bezier(0.68, -0.55, 0.265, 1.55);  
        }  
  
        @keyframes popIn {  
            0% {  
                transform: scale(0);  
                opacity: 0;  
            }  
            100% {  
                transform: scale(1);  
                opacity: 1;  
            }  
        }  
  
        .celebration-content h2 {  
            color: #e91e63;  
            font-size: 42px;  
            margin-bottom: 20px;  
            animation: rainbow 3s infinite;  
        }  
  
        @keyframes rainbow {  
            0%, 100% { color: #e91e63; }  
            25% { color: #9c27b0; }  
            50% { color: #f44336; }  
            75% { color: #ff5722; }  
        }  
  
        .celebration-content p {  
            font-size: 24px;  
            color: #555;  
            margin-bottom: 30px;  
        }  
  
        .confetti {  
            position: absolute;  
            width: 10px;  
            height: 10px;  
            background: #f0f;  
            position: fixed;  
            animation: confetti-fall 3s linear infinite;  
        }  
  
        @keyframes confetti-fall {  
            to {  
                transform: translateY(100vh) rotate(360deg);  
                opacity: 0;  
            }  
        }  
  
        .emoji-explosion {  
            font-size: 60px;  
            margin: 20px 0;  
            animation: spin 2s linear infinite;  
        }  
  
        @keyframes spin {  
            from { transform: rotate(0deg); }  
            to { transform: rotate(360deg); }  
        }  
  
        .date-info {  
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);  
            color: white;  
            padding: 15px 30px;  
            border-radius: 25px;  
            font-size: 20px;  
            font-weight: bold;  
            margin-top: 20px;  
            display: inline-block;  
            box-shadow: 0 4px 15px rgba(245, 87, 108, 0.4);  
        }  
  
        .sparkle {  
            position: fixed;  
            pointer-events: none;  
            animation: sparkle-animation 1s ease-out forwards;  
        }  
  
        @keyframes sparkle-animation {  
            0% {  
                transform: scale(0) rotate(0deg);  
                opacity: 1;  
            }  
            100% {  
                transform: scale(1) rotate(180deg);  
                opacity: 0;  
            }  
        }  
    </style>  
</head>  
<body>  
    <div class="heart-bg" id="heartBg"></div>  
  
    <div class="container">  
        <div class="heart-icon">💖</div>  
        <h1>Valentine's Day Invitation</h1>  
        <p class="message">  
            Will you be my Valentine tomorrow?<br>  
            <strong>Let's make February 14th special together! 💕</strong>  
        </p>  
        <div class="buttons">  
            <button class="yes-btn" onclick="celebrateYes()">Yes! 💝</button>  
            <button class="no-btn" id="noBtn" onmouseover="runAway(event)" onclick="runAway(event)">No 😢</button>  
        </div>  
    </div>  
  
    <div class="celebration" id="celebration">  
        <div class="celebration-content">  
            <div class="emoji-explosion">🎉💖✨</div>  
            <h2>Yay! 🎊</h2>  
            <p>Thank you Spoorthy for choosing Venkatesh as your Valentine!</p>  
            <div class="date-info">📅 Valentine's Date: February 14, 2026</div>  
            <p style="margin-top: 30px; font-size: 20px;">Get ready for the most amazing Valentine's Day! 💕</p>  
        </div>  
    </div>  
  
    <script>  
        function createFloatingHearts() {  
            const heartBg = document.getElementById('heartBg');  
            const hearts = ['❤️', '💕', '💖', '💗', '💝', '💘'];  
              
            for (let i = 0; i < 15; i++) {  
                const heart = document.createElement('div');  
                heart.className = 'floating-heart';  
                heart.textContent = hearts[Math.floor(Math.random() * hearts.length)];  
                heart.style.left = Math.random() * 100 + '%';  
                heart.style.animationDelay = Math.random() * 15 + 's';  
                heart.style.fontSize = (Math.random() * 20 + 15) + 'px';  
                heartBg.appendChild(heart);  
            }  
        }  
  
        createFloatingHearts();  
  
        function runAway(event) {  
            event.preventDefault();  
            const noBtn = document.getElementById('noBtn');  
            const container = document.querySelector('.container');  
            const containerRect = container.getBoundingClientRect();  
              
            const maxX = containerRect.width - noBtn.offsetWidth - 100;  
            const maxY = 200;  
              
            const randomX = Math.random() * maxX;  
            const randomY = Math.random() * maxY - 100;  
              
            noBtn.style.left = randomX + 'px';  
            noBtn.style.top = randomY + 'px';  
              
            noBtn.style.transform = 'scale(0.9)';  
            setTimeout(() => {  
                noBtn.style.transform = 'scale(1)';  
            }, 100);  
        }  
  
        function celebrateYes() {  
            const celebration = document.getElementById('celebration');  
            celebration.style.display = 'flex';  
              
            createConfetti();  
            createSparkles();  
              
            document.body.style.animation = 'none';  
        }  
  
        function createConfetti() {  
            const colors = ['#f44336', '#e91e63', '#9c27b0', '#673ab7', '#3f51b5', '#2196f3', '#00bcd4', '#009688', '#4caf50', '#ffeb3b', '#ff9800', '#ff5722'];  
              
            for (let i = 0; i < 150; i++) {  
                const confetti = document.createElement('div');  
                confetti.className = 'confetti';  
                confetti.style.left = Math.random() * 100 + '%';  
                confetti.style.top = -10 + 'px';  
                confetti.style.background = colors[Math.floor(Math.random() * colors.length)];  
                confetti.style.animationDelay = Math.random() * 3 + 's';  
                confetti.style.animationDuration = (Math.random() * 3 + 2) + 's';  
                document.body.appendChild(confetti);  
                  
                setTimeout(() => {  
                    confetti.remove();  
                }, 5000);  
            }  
        }  
  
        function createSparkles() {  
            const sparkleInterval = setInterval(() => {  
                const sparkle = document.createElement('div');  
                sparkle.className = 'sparkle';  
                sparkle.textContent = '✨';  
                sparkle.style.left = Math.random() * window.innerWidth + 'px';  
                sparkle.style.top = Math.random() * window.innerHeight + 'px';  
                sparkle.style.fontSize = (Math.random() * 30 + 20) + 'px';  
                document.body.appendChild(sparkle);  
                  
                setTimeout(() => {  
                    sparkle.remove();  
                }, 1000);  
            }, 100);  
              
            setTimeout(() => {  
                clearInterval(sparkleInterval);  
            }, 3000);  
        }  
  
        document.addEventListener('DOMContentLoaded', () => {  
            const noBtn = document.getElementById('noBtn');  
            noBtn.style.position = 'relative';  
            noBtn.style.left = '0';  
            noBtn.style.top = '0';  
        });  
    </script>  
</body>  
</html>  
