<!DOCTYPE html>
<html>
<head>
    <title>Happy Birthday Shubhashree 🖤</title>

    <style>
        body {
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
            font-family: 'Poppins', sans-serif;
            text-align: center;
            color: white;
            overflow: hidden;
        }

        .container {
            margin-top: 60px;
            padding: 20px;
            position: relative;
            z-index: 2;
        }

        img {
            width: 260px;
            border-radius: 20px;
            box-shadow: 0 0 25px #ff4e88;
            margin-bottom: 20px;
        }

        h1 {
            font-size: 38px;
            color: #ff4e88;
            text-shadow: 0 0 20px #ff4e88;
        }

        p {
            font-size: 20px;
            margin: 15px;
        }

        button {
            padding: 12px 25px;
            font-size: 18px;
            border: none;
            border-radius: 25px;
            background-color: #ff4e88;
            color: white;
            cursor: pointer;
            transition: 0.3s;
        }

        button:hover {
            background-color: white;
            color: #ff4e88;
        }

        /* Floating hearts */
        .heart {
            position: absolute;
            color: #ff4e88;
            font-size: 20px;
            animation: float 6s linear infinite;
        }

        @keyframes float {
            0% {
                transform: translateY(100vh);
                opacity: 1;
            }
            100% {
                transform: translateY(-10vh);
                opacity: 0;
            }
        }
    </style>
</head>

<body>

<!-- Background Music -->
<audio autoplay loop>
    <!-- Replace music.mp3 with your song file -->
    <source src="music.mp3" type="audio/mpeg">
</audio>

<div class="container">
    <img src="image.jpg" alt="Shubhashree">

    <h1>Happy Birthday Shubhashree 🖤✨</h1>

    <p>Thank you for being my friend 💎🥹</p>
    <p>I love you so much 💕</p>

    <button onclick="showSurprise()">Click for Surprise 💌</button>

    <p id="surprise"></p>
</div>

<script>
function showSurprise() {
    document.getElementById("surprise").innerHTML =
    "Aashiqana… Tera paas, tere rehna 🖤✨ Always with you forever 💘";
}

/* Create Floating Hearts */
function createHeart() {
    const heart = document.createElement("div");
    heart.classList.add("heart");
    heart.innerHTML = "❤";
    heart.style.left = Math.random() * 100 + "vw";
    heart.style.fontSize = Math.random() * 20 + 15 + "px";
    heart.style.animationDuration = Math.random() * 3 + 3 + "s";
    document.body.appendChild(heart);

    setTimeout(() => {
        heart.remove();
    }, 6000);
}

setInterval(createHeart, 500);
</script>

</body>
</html>
