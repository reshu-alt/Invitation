# Invitation
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will you be my Valentine? 🌹</title>
    <style>
        body { 
            background: linear-gradient(135deg, #fff0f3 0%, #ffccd5 100%); 
            font-family: 'Georgia', serif; 
            display: flex; 
            justify-content: center; 
            align-items: center; 
            height: 100vh; 
            margin: 0; 
            overflow: hidden; 
            text-align: center; 
        }
        .container { 
            background: rgba(255, 255, 255, 0.9); 
            padding: 3rem; 
            border-radius: 30px; 
            box-shadow: 0 15px 35px rgba(255, 77, 109, 0.2); 
            border: 2px solid #ffffff; 
            max-width: 450px; 
            z-index: 10; 
            position: relative; 
        }
        h1 { 
            color: #ff4d6d; 
            font-size: 2.2rem; 
            margin-bottom: 1.5rem; 
        }
        p { 
            color: #590d22; 
            font-size: 1.25rem; 
            line-height: 1.6; 
        }
        .btn-container { 
            margin-top: 2.5rem; 
            display: flex; 
            justify-content: center; 
            gap: 15px; 
        }
        button { 
            padding: 14px 28px; 
            font-size: 1.1rem; 
            border: none; 
            border-radius: 50px; 
            cursor: pointer; 
            transition: all 00.3s ease; 
            font-weight: bold; 
        }
        #yesBtn { 
            background-color: #ff4d6d; 
            color: white; 
            box-shadow: 0 4px 15px rgba(255, 77, 109, 0.4); 
        }
        #yesBtn:hover { 
            transform: translateY(-3px) scale(1.05); 
            background-color: #ff758f; 
        }
        #noBtn { 
            background-color: #f8adbc; 
            color: #ffffff; 
        }
        #noBtn:hover { 
            background-color: #ff8fa3; 
        }
        /* Floating Hearts Animation */
        .heart { 
            position: absolute; 
            color: #ff8fa3; 
            font-size: 20px; 
            pointer-events: none; 
            animation: float 6s linear infinite; 
            top: 100vh; 
            opacity: 0.6; 
        }
        @keyframes float { 
            0% { 
                transform: translateY(0) rotate(0deg); 
                opacity: 0.8; 
            }
            100% { 
                transform: translateY(-110vh) rotate(360deg); 
                opacity: 0; 
            }
        }
    </style>
</head>
<body>
    <div class="container" id="mainCard">
        <h1>Will you be my Valentine? 🌹</h1>
        <p id="message"> Hey <strong>Gaurav sir</strong>,<br><br> From the moment I met you, I knew you'd be someone special. Will you be my Valentine? </p>
        <div class="btn-container">
            <button id="yesBtn" onclick="celebrate()">Yes!</button>
            <button id="noBtn" onclick="tooLate()">Hmm, let me think... 🤔</button>
        </div>
        <p style="font-style: italic; font-size: 0.95rem; margin-top: 2.5rem; color:                                                                         
    </div>
    <script>
                                 
        function createHeart() {
            const heart = document.createElement('"font-style: italic; font-size: 0.95rem; margin-top: 2.5rem; color:                                                                         
    </div>
    <script>
                                 
        function createHeart() {
            const heart = document.createElement('div');
            heart.classList.add('heart');
            heart.innerHTML = '🌸'; 
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.fontSize = (Math.random() * 20 + 10) + 'px';
            heart.style.animationDuration = Math.random() * 3 + 4 + 's';
            document.body.appendChild(heart);
            setTimeout(() => heart.remove(), 7000);
        }
        setInterval(createHeart, 400);

        function celebrate() {
            const card = document.getElementById('mainCard');
            card.innerHTML = `
                <h1 style="');
            card.innerHTML = `
                <h1 style="font-size: 3.5rem;">💖 Yay! 💖</h1>
                <p style="font-size: 1.4rem;">I’m the luckiest person to have you, Gaurav sir!</p>
                <div style="margin-top: 25px; padding: 15px; border-top: 1px solid                                                                                     
            `;
            for(let i=0; i<20; i++) setTimeout(createHeart, i*100);
        }

        function tooLate() {
            const card = document.getElementById('mainCard');
            card.innerHTML = `
                <h1 style="font-size: 2.5rem;">Nice try! 😂</h1>
                <p style="font-size: 1.6rem; color:                                                                                    
                <button id="yesBtn" style="margin-top: 25px;" onclick="celebrate()">I accept!</button>
            `;
        }
    </script>
</body>
</html>
