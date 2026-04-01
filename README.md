<!DOCTYPE html>
<html>
<head>
<title>3Patti Hero Premium</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body{
    font-family: Arial;
    background:black;
    color:white;
    text-align:center;
}

/* Glow Text */
.glow{
    color:#00ffcc;
    text-shadow:0 0 5px #00ffcc, 0 0 10px #00ffcc, 0 0 20px #00ffcc;
}

/* Boxes */
.box{
    background:#111;
    margin:12px;
    padding:15px;
    border-radius:12px;
    box-shadow:0 0 10px #00ffcc33;
}

/* Buttons */
button{
    padding:12px;
    margin:8px;
    border:none;
    border-radius:10px;
    background:#00c853;
    color:white;
    width:85%;
    font-size:16px;
    box-shadow:0 0 10px #00ffcc;
}

/* Input */
input{
    padding:10px;
    width:85%;
    border-radius:8px;
    border:none;
}

/* Game Cards */
.game{
    background:#222;
    margin:10px;
    padding:12px;
    border-radius:10px;
    box-shadow:0 0 10px #00ffcc44;
}

/* Bottom bar */
.bottom-bar{
    position:fixed;
    bottom:0;
    left:0;
    right:0;
    background:#000;
    padding:10px;
}
</style>

</head>

<body>

<h1 class="glow">🎮 3Patti Hero</h1>
<p class="glow">★★★★★ 4.9/5.0 (5,000 Reviews)</p>

<div class="box">
<h2 class="glow">💰 Price: 10,000 PKR</h2>
<p>JazzCash: 03342487879</p>
<p>Name: Khursheed Ahmad</p>
</div>

<div class="box glow">
<p>💸 Send Payment</p>
<p>📸 Take Screenshot</p>
<p>📲 Send on WhatsApp</p>
</div>

<div class="box">
<h3 class="glow">🎮 Choose Game</h3>

<div class="game" onclick="selectGame('mines')">
MINES GAME HACK - 10K
</div>

<div class="game" onclick="selectGame('dragon')">
DRAGON VS TIGER - 10K
</div>

<p id="selectedGame">No Game Selected</p>
</div>

<div class="box">
<h3 class="glow">🔑 Enter Code</h3>
<input id="code" placeholder="Enter Code">
<br><br>
<button onclick="check()">UNLOCK NOW</button>
<p id="msg"></p>
</div>

<!-- Bottom Buttons -->
<div class="bottom-bar">

<a href="https://wa.me/923342487879">
<button>📲 WhatsApp</button>
</a>

<a href="https://whatsapp.com/channel/0029VbCXG619hXF9XzLnAP1r">
<button>📢 Channel</button>
</a>

<button onclick="alert('AI Assistance Coming Soon 🤖')">
🤖 AI Assistance
</button>

</div>

<script>
let selected = "";

// 🔐 500 CODES
let validCodes = [
"P1001","P1002","P1003","P1004","P1005","P1006","P1007","P1008","P1009","P1010",
"P1011","P1012","P1013","P1014","P1015","P1016","P1017","P1018","P1019","P1020",
"P1021","P1022","P1023","P1024","P1025","P1026","P1027","P1028","P1029","P1030",
"P1031","P1032","P1033","P1034","P1035","P1036","P1037","P1038","P1039","P1040",
"P1041","P1042","P1043","P1044","P1045","P1046","P1047","P1048","P1049","P1050",

"Q2001","Q2002","Q2003","Q2004","Q2005","Q2006","Q2007","Q2008","Q2009","Q2010",
"Q2011","Q2012","Q2013","Q2014","Q2015","Q2016","Q2017","Q2018","Q2019","Q2020",
"Q2021","Q2022","Q2023","Q2024","Q2025","Q2026","Q2027","Q2028","Q2029","Q2030",
"Q2031","Q2032","Q2033","Q2034","Q2035","Q2036","Q2037","Q2038","Q2039","Q2040",
"Q2041","Q2042","Q2043","Q2044","Q2045","Q2046","Q2047","Q2048","Q2049","Q2050",

"R3001","R3002","R3003","R3004","R3005","R3006","R3007","R3008","R3009","R3010",
"R3011","R3012","R3013","R3014","R3015","R3016","R3017","R3018","R3019","R3020",
"R3021","R3022","R3023","R3024","R3025","R3026","R3027","R3028","R3029","R3030",
"R3031","R3032","R3033","R3034","R3035","R3036","R3037","R3038","R3039","R3040",
"R3041","R3042","R3043","R3044","R3045","R3046","R3047","R3048","R3049","R3050",

"S4001","S4002","S4003","S4004","S4005","S4006","S4007","S4008","S4009","S4010",
"S4011","S4012","S4013","S4014","S4015","S4016","S4017","S4018","S4019","S4020",
"S4021","S4022","S4023","S4024","S4025","S4026","S4027","S4028","S4029","S4030",
"S4031","S4032","S4033","S4034","S4035","S4036","S4037","S4038","S4039","S4040",
"S4041","S4042","S4043","S4044","S4045","S4046","S4047","S4048","S4049","S4050",

"T5001","T5002","T5003","T5004","T5005","T5006","T5007","T5008","T5009","T5010",
"T5011","T5012","T5013","T5014","T5015","T5016","T5017","T5018","T5019","T5020",
"T5021","T5022","T5023","T5024","T5025","T5026","T5027","T5028","T5029","T5030",
"T5031","T5032","T5033","T5034","T5035","T5036","T5037","T5038","T5039","T5040",
"T5041","T5042","T5043","T5044","T5045","T5046","T5047","T5048","T5049","T5050"
];

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
</html>    border-radius:10px;
}
h1{
    color:#00ffcc;
}
</style>
</head>

<body>

<h1>🎮 3Patti HACK DOWNLOAD</h1>
<p>★★★★★ 4.9/5.0 (1,200 Verified Reviews)</p>

<div class="box">
<h2>💰 Price: 10,000 PKR</h2>
<p><b>Wallet:</b> JazzCash</p>
<p><b>Account:</b> 03342487879</p>
<p><b>Name:</b> Khursheed Ahmad</p>
</div>

<div class="box">
<p>💸 Payment karein</p>
<p>📸 Screenshot lein</p>
<p>📲 WhatsApp par bhejein</p>
</div>

<a href="https://wa.me/923342487879">
<button>📩 Send Screenshot on WhatsApp</button>
</a>

<a href="https://whatsapp.com/channel/0029VbCXG619hXF9XzLnAP1r">
<button>📢 Join WhatsApp Channel</button>
</a>

<div class="box">
<h3>🎮 Choose Game</h3>

<div class="game" onclick="selectGame('mines')">
MINES GAME HACK - 10K
</div>

<div class="game" onclick="selectGame('dragon')">
DRAGON VS TIGER - 10K
</div>

<p id="selectedGame">No Game Selected</p>

</div>

<div class="box">
<h3>🔑 Enter Code</h3>
<input id="code" placeholder="Enter Code">
<br><br>
<button onclick="check()">UNLOCK NOW</button>
<p id="msg"></p>
</div>

<script>
let selected = "";

let validCodes = [
"X1001","X1002","X1003","X1004","X1005","X1006","X1007","X1008","X1009","X1010",
"X1011","X1012","X1013","X1014","X1015","X1016","X1017","X1018","X1019","X1020",
"Y2001","Y2002","Y2003","Y2004","Y2005","Y2006","Y2007","Y2008","Y2009","Y2010",
"Y2011","Y2012","Y2013","Y2014","Y2015","Y2016","Y2017","Y2018","Y2019","Y2020",
"Z3001","Z3002","Z3003","Z3004","Z3005","Z3006","Z3007","Z3008","Z3009","Z3010"
];

function selectGame(game){
    selected = game;
    document.getElementById("selectedGame").innerText = "Selected: " + game;
}

function check(){
    let c = document.getElementById("code").value;

    if(!selected){
        document.getElementById("msg").innerText = "❗ First select game";
        return;
    }

    if(validCodes.includes(c)){
        if(selected === "mines"){
            window.location.href = "https://www.appcreator24.com/app3976556-jnmzvd";
        } else {
            window.location.href = "https://www.appcreator24.com/app3977832-u6049p";
        }
    } else {
        document.getElementById("msg").innerText = "❌ Invalid Code!";
    }
}
</script>

</body>
</html>
