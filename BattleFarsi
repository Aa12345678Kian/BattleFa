<!DOCTYPE html>
<html lang="fa">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Battle Fa 🇮🇷</title>

<style>
body {
    margin: 0;
    font-family: sans-serif;
    background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

.card {
    background: rgba(0,0,0,0.4);
    padding: 25px;
    border-radius: 16px;
    width: 280px;
    text-align: center;
}

input {
    width: 100%;
    padding: 10px;
    border-radius: 8px;
    border: none;
    margin-top: 10px;
    font-size: 14px;
}

button {
    width: 100%;
    padding: 12px;
    margin-top: 15px;
    border-radius: 10px;
    border: none;
    background: #3ddc97;
    font-size: 15px;
    cursor: pointer;
}

button:hover {
    opacity: 0.9;
}

#game {
    display: none;
    text-align: center;
}

.hit-btn {
    margin-top: 20px;
    background: #ff5252;
    color: white;
}
</style>
</head>

<body>

<!-- صفحه ورود -->
<div class="card" id="login">
    <h2>Battle Fa 🇮🇷</h2>
    <p>به میدان نبرد خوش آمدی</p>
    <input type="text" id="username" placeholder="نام بازیکن">
    <button onclick="startGame()">ورود به بازی</button>
</div>

<!-- صفحه بازی -->
<div class="card" id="game">
    <h2 id="playerName"></h2>
    <p>ضربه‌های باقی‌مانده:</p>
    <h1 id="hits">30</h1>
    <button class="hit-btn" onclick="hit()">🥷 ضربه نینجا</button>
    <p id="msg"></p>
</div>

<script>
let hits = 30;

function startGame() {
    const name = document.getElementById("username").value.trim();
    if (name === "") {
        alert("نام را وارد کن");
        return;
    }

    document.getElementById("playerName").innerText = "نیاجا " + name;
    document.getElementById("login").style.display = "none";
    document.getElementById("game").style.display = "block";
}

function hit() {
    if (hits <= 0) {
        document.getElementById("msg").innerText = "❌ ضربه‌های امروز تموم شد";
        return;
    }

    hits--;
    document.getElementById("hits").innerText = hits;
    document.getElementById("msg").innerText = "✅ ضربه زده شد";
}
</script>

</body>
</html>
