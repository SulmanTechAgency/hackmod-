<!DOCTYPE html>
<html>
<head>
<title>3Patti Hero</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body{
    font-family: Arial;
    background:black;
    color:white;
    text-align:center;
    margin:0;
}

/* Glow */
.glow{
    color:#00ffcc;
    text-shadow:0 0 5px #00ffcc,0 0 10px #00ffcc;
}

/* Boxes */
.box{
    background:#111;
    margin:8px;
    padding:12px;
    border-radius:10px;
}

/* Small Buttons */
button{
    padding:10px;
    margin:6px;
    border:none;
    border-radius:8px;
    background:#00c853;
    color:white;
    width:90%;
    font-size:14px;
}

/* Input */
input{
    padding:8px;
    width:85%;
    border-radius:6px;
    border:none;
}

/* Game cards */
.game{
    background:#222;
    margin:6px;
    padding:10px;
    border-radius:8px;
    font-size:14px;
}

/* Floating circle buttons */
.floating{
    position:fixed;
    bottom:15px;
    width:50px;
    height:50px;
    border-radius:50%;
    display:flex;
    justify-content:center;
    align-items:center;
    font-size:20px;
    box-shadow:0 0 10px #00ffcc;
}

/* WhatsApp button */
.whatsapp{
    right:15px;
    background:#25D366;
}

/* AI button */
.ai{
    left:15px;
    background:#00c853;
}
</style>

</head>

<body>

<h2 class="glow">🎮 3Patti Hero</h2>
<p class="glow">★★★★★ 4.9 (5000 Reviews)</p>

<div class="box">
<p class="glow">💰 10,000 PKR</p>
<p>JazzCash: 03342487879</p>
<p>Name: Khursheed Ahmad</p>
</div>

<div class="box">
<p>💸 Payment karein</p>
<p>📸 Screenshot lein</p>
<p>📲 WhatsApp par bhejein</p>
</div>

<div class="box">
<p class="glow">🎮 Select Game</p>

<div class="game" onclick="selectGame('mines')">
MINES GAME - 10K
</div>

<div class="game" onclick="selectGame('dragon')">
DRAGON VS TIGER - 10K
</div>

<p id="selectedGame"></p>
</div>

<div class="box">
<p class="glow">🔑 Enter Code</p>
<input id="code" placeholder="Code">
<br><br>
<button onclick="check()">UNLOCK</button>
<p id="msg"></p>
</div>

<!-- Bottom Text -->
<div class="box">
<p class="glow">📢 JOIN FOR NEW UPDATES</p>
<a href="https://whatsapp.com/channel/0029VbCXG619hXF9XzLnAP1r">
<button>Join Channel</button>
</a>
</div>

<!-- Floating Buttons -->
<a href="https://wa.me/923342487879" class="floating whatsapp">💬</a>

<div class="floating ai" onclick="alert('AI Coming Soon 🤖')">🤖</div>

<script>
let selected = "";

let validCodes = ["P1001","P1002","P1003","P1004","P1005"]; // sample (baaki tum add kar sakte ho)

function selectGame(game){
    selected = game;
    document.getElementById("selectedGame").innerText = "Selected: " + game;
}

function check(){
    let c = document.getElementById("code").value;

    if(!selected){
        document.getElementById("msg").innerText = "Select game first!";
        return;
    }

    if(validCodes.includes(c)){
        if(selected === "mines"){
            window.location.href = "https://www.appcreator24.com/app3976556-jnmzvd";
        } else {
            window.location.href = "https://www.appcreator24.com/app3977832-u6049p";
        }
    } else {
        document.getElementById("msg").innerText = "Invalid Code!";
    }
}
</script>

</body>
</html>
