# Ishita my love 💕
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Proposal Day for Ishita 💖</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body {
    margin: 0;
    font-family: 'Poppins', sans-serif;
    background: linear-gradient(120deg, #ff758c, #ff7eb3);
    color: white;
    text-align: center;
}
section {
    padding: 60px 20px;
}
h1, h2 {
    letter-spacing: 1px;
}
.card {
    background: rgba(255,255,255,0.15);
    padding: 25px;
    border-radius: 20px;
    max-width: 850px;
    margin: 20px auto;
    box-shadow: 0 15px 35px rgba(0,0,0,0.2);
}
button {
    padding: 12px 28px;
    border: none;
    border-radius: 30px;
    background: white;
    color: #ff4d6d;
    font-size: 16px;
    cursor: pointer;
    margin: 10px;
    transition: 0.3s;
}
button:hover {
    transform: scale(1.08);
    background: #ffe6ec;
}
.hidden {
    display: none;
}
.memory span {
    display: inline-block;
    width: 80px;
    height: 80px;
    line-height: 80px;
    margin: 8px;
    background: white;
    color: #ff4d6d;
    font-size: 28px;
    border-radius: 15px;
    cursor: pointer;
}
footer {
    padding: 30px;
    font-size: 14px;
    opacity: 0.8;
}
</style>
</head>

<body>

<section>
    <h1>Happy Proposal Day, Ishita 💖</h1>
    <div class="card">
        <p>
            Ishita, from the moment you came into my life, something quietly beautiful began.
            You didn’t just make my days brighter — you made my ordinary moments feel magical.
            The way you smile, the way you listen, the way you exist… it all feels like home.
        </p>
        <p>
            Every laugh we’ve shared, every conversation that went deep into the night,
            every small moment that felt insignificant to the world — meant everything to me.
            You unknowingly became my comfort, my happiness, and my favorite thought.
        </p>
        <p>
            So today isn’t just about proposing love.  
            It’s about choosing *you* — again and again — in every universe, in every lifetime.
        </p>
    </div>
</section>

<section>
    <h2>🎮 Game 1: Love Quiz</h2>
    <div class="card">
        <p>What do you think I love the most about you?</p>
        <button onclick="quiz(true)">Your smile</button>
        <button onclick="quiz(false)">Your figure 😭🤧🤧🥹</button>
        <button onclick="quiz(false)">love everything about u yrr 🥺 💗 💝 taste</button>
        <p id="quizResult"></p>
    </div>
</section>

<section>
    <h2>🧠 Game 2: Memory of Love</h2>
    <div class="card memory">
        <p>Tap all hearts 💖</p>
        <span onclick="flip(this)">💖</span>
        <span onclick="flip(this)">💖</span>
        <span onclick="flip(this)">🌸</span>
        <span onclick="flip(this)">💖</span>
        <span onclick="flip(this)">🌸</span>
        <p id="memoryResult"></p>
    </div>
</section>

<section>
    <h2>🔐 Final Challenge</h2>
    <div class="card">
        <p>Type the name written in my heart:</p>
        <input id="answer" placeholder="ISHITA"
               style="padding:12px;border-radius:20px;border:none;text-align:center;">
        <br><br>
        <button onclick="checkName()">Unlock</button>
        <p id="unlockMsg"></p>
    </div>
</section>

<section id="proposal" class="hidden">
    <h1>💍 My Proposal</h1>
    <div class="card">
        <p>
            Ishita, if love had a face, it would look like you.
            If happiness had a voice, it would sound like your laughter.
        </p>
        <p>
            I don’t promise perfection —  
            but I promise honesty, loyalty, support, and endless love.
            I promise to stand with you in every storm and celebrate every sunshine.
        </p>
        <h2>Will you be mine — today, tomorrow, and forever? ❤️</h2>
        <button onclick="yes()">YES 💖</button>
        <button onclick="no()">NO 🙈</button>
        <p id="finalMsg"></p>
    </div>
</section>

<footer>
    Made with ❤️ only for Ishita
</footer>

<script>
function quiz(correct) {
    document.getElementById("quizResult").innerHTML =
        correct ? "Correct 💕 Because your smile melts my heart!" : "Nice try 😄 But try again!";
}

let hearts = 0;
function flip(el) {
    if (el.innerHTML === "💖") {
        hearts++;
        el.style.background = "#ff4d6d";
        el.style.color = "white";
        if (hearts === 3) {
            document.getElementById("memoryResult").innerHTML =
                "You found all my hearts ❤️";
        }
    }
}

function checkName() {
    let name = document.getElementById("answer").value.toLowerCase();
    if (name === "ishita") {
        document.getElementById("unlockMsg").innerHTML = "Unlocked with love 💘";
        document.getElementById("proposal").classList.remove("hidden");
    } else {
        document.getElementById("unlockMsg").innerHTML = "Hmm… my heart says Ishita ❤️";
    }
}

function yes() {
    document.getElementById("finalMsg").innerHTML =
        "You just made me the happiest person alive 😭❤️";
}

function no() {
    document.getElementById("finalMsg").innerHTML =
        "Haha 😄 I’ll still keep loving you!";
}
</script>

</body>
</html>
