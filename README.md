<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>One Year of Best Friendship 💗</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: Georgia, serif;
    background: linear-gradient(135deg, #ffe0eb, #e8dcff, #fff0f5);
    padding: 20px;
    overflow-x: hidden;
    color: #693c59;
}

.heart {
    position: fixed;
    bottom: -40px;
    animation: float 8s linear infinite;
    opacity: 0.7;
    pointer-events: none;
}

@keyframes float {
    0% {
        transform: translateY(0) rotate(0);
        opacity: 0;
    }
    20% { opacity: 0.7; }
    100% {
        transform: translateY(-110vh) rotate(360deg);
        opacity: 0;
    }
}

.card {
    width: 100%;
    max-width: 440px;
    padding: 30px 23px;
    background: rgba(255,255,255,0.88);
    border: 1px solid white;
    border-radius: 25px;
    box-shadow: 0 12px 40px #b989bd40;
    text-align: center;
    position: relative;
    z-index: 1;
}

.small {
    font-size: 12px;
    letter-spacing: 2px;
    color: #bb7299;
    text-transform: uppercase;
}

h1 {
    font-size: 30px;
    margin: 18px 0;
    line-height: 1.3;
}

.subtitle {
    font-size: 16px;
    line-height: 1.8;
    margin-bottom: 25px;
}

button {
    border: none;
    padding: 14px 25px;
    background: #d77ba5;
    color: white;
    font-size: 16px;
    border-radius: 30px;
    cursor: pointer;
    box-shadow: 0 5px 15px #d77ba555;
    transition: 0.3s;
}

button:hover {
    transform: scale(1.05);
    background: #c86494;
}

#letter {
    display: none;
    text-align: left;
    margin-top: 25px;
    line-height: 1.9;
    font-size: 15px;
    animation: appear 1s ease;
}

#letter h2 {
    text-align: center;
    margin-bottom: 20px;
    color: #bc6791;
}

#letter p {
    margin-bottom: 16px;
}

.signature {
    text-align: right;
    color: #bd6894;
    font-style: italic;
}

@keyframes appear {
    from {
        opacity: 0;
        transform: translateY(15px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.footer {
    margin-top: 25px;
    font-size: 12px;
    opacity: 0.7;
}
</style>
</head>

<body>

<div id="hearts"></div>

<main class="card">

    <div class="small">
        October 29 · A Special Day 🌷
    </div>

    <h1>
        One Year of Best Friendship 💗
    </h1>

    <p class="subtitle">
        One year of being best friends,<br>
        countless memories, and a bond<br>
        that means more than words can say.
        <br><br>
        Maisha, I made something just for you. 🫶🏻
    </p>

    <button id="openBtn" onclick="openLetter()">
        Open Your Surprise 💌
    </button>

    <section id="letter">

        <h2>To My Best Friend, Maisha 🌸</h2>

        <p>
            Hey Maisha, 💗
        </p>

        <p>
            Can you believe it's been one whole year
            of our best friendship? Honestly, it feels
            so special to look back and realize how
            much we've become a part of each other's lives.
        </p>

        <p>
            You know, not everyone gets a best friend
            with whom they can share random thoughts,
            silly jokes, little problems, and those
            moments when words aren't even needed.
            I'm genuinely glad I found that kind of
            friendship with you.
        </p>

        <p>
            You mean a lot to me, Maisha.
            Maybe I don't always express it perfectly,
            but I really appreciate having you in my life.
            Thank you for understanding me, listening
            to me, and being someone I can share so
            many things with.
        </p>

        <p>
            I know we're not perfect. Sometimes we may
            misunderstand each other, disagree, or fail
            to explain what we actually mean.
            But I hope we always try to understand
            each other instead of letting small things
            come between our friendship.
        </p>

        <p>
            One thing I really love about us is how
            we can be ourselves together. The random
            conversations, our usual talks, the jokes,
            and all those little moments might seem
            ordinary, but they mean a lot to me.
        </p>

        <p>
            I don't know what the future holds for us,
            or how much life will change, but I genuinely
            hope we keep this friendship alive.
            I hope we continue growing together,
            supporting each other, and making more
            memories that we'll look back on someday
            and smile about.
        </p>

        <p>
            Thank you for being my best friend, Maisha.
            Thank you for being a part of my life
            and making this past year more meaningful.
            I'm proud of the friendship we've built,
            and I hope we have many more years of
            friendship, trust, laughter, and understanding
            ahead of us. 🥹💗
        </p>

        <p>
            Happy one year of best friendship to us!
            Here's to all the memories we've made
            and all the ones still waiting for us.
            No matter how busy life gets, I hope
            we never lose the bond we've built.
        </p>

        <p class="signature">
            Always wishing the best for you,<br>
            Your best friend,<br>
            Jisan 💗
        </p>

    </section>

    <div class="footer">
        A little surprise, made with care by Jisan ✨
    </div>

</main>

<script>
function openLetter() {
    document.getElementById("letter").style.display = "block";
    document.getElementById("openBtn").style.display = "none";
}

const hearts = document.getElementById("hearts");
const symbols = ["💗", "💕", "🌸", "♡", "✨"];

for (let i = 0; i < 25; i++) {
    const heart = document.createElement("span");

    heart.className = "heart";

    heart.textContent = symbols[
        Math.floor(Math.random() * symbols.length)
    ];

    heart.style.left = Math.random() * 100 + "vw";
    heart.style.animationDelay = Math.random() * 8 + "s";
    heart.style.animationDuration =
        (5 + Math.random() * 6) + "s";
    heart.style.fontSize =
        (14 + Math.random() * 18) + "px";

    hearts.appendChild(heart);
}
</script>

</body>
</html>
