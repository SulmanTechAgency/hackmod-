<!DOCTYPE html>
<html>
<head>
<title>3Patti Hack Apk</title>
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

/* Box */
.box{
    background:#111;
    margin:8px;
    padding:12px;
    border-radius:10px;
}

/* Button */
button{
    padding:10px;
    margin:6px;
    border:none;
    border-radius:8px;
    background:#00c853;
    color:white;
    width:90%;
}

/* Floating */
.floating{
    position:fixed;
    bottom:15px;
    width:50px;
    height:50px;
    border-radius:50%;
    display:flex;
    justify-content:center;
    align-items:center;
}
.whatsapp{ right:15px; background:#25D366; }
.ai{ left:15px; background:#00c853; }

/* Live counter */
#liveUsers{
    position:fixed;
    top:10px;
    right:10px;
    background:#111;
    padding:8px;
    border-radius:8px;
    font-size:12px;
}

/* Popup */
.popup{
    position:fixed;
    bottom:80px;
    left:-300px;
    background:#111;
    padding:10px;
    border-radius:10px;
    transition:0.5s;
}
</style>

</head>

<body>

<h2 class="glow">🎮 3Patti Hack Download</h2>

<!-- Live Users -->
<div id="liveUsers" class="glow">👥 5234 Online</div>

<div class="box">
<p class="glow">💰 10,000 PKR</p>
</div>

<!-- Popup -->
<div id="popup" class="popup glow"></div>

<!-- Floating -->
<a href="https://wa.me/923342487879" class="floating whatsapp">💬</a>
<div class="floating ai" onclick="alert('AI 🤖')">🤖</div>

<script>

// 🔥 Live Users Counter
let users = 5200;

setInterval(()=>{
    let change = Math.floor(Math.random()*20);

    if(Math.random() > 0.5){
        users += change;
    } else {
        users -= Math.floor(Math.random()*3);
    }

    if(users < 5000) users = 5000;

    document.getElementById("liveUsers").innerText = "👥 " + users + " Online";
},3000);

// 🔔 Activity Popup
let names = ["Ali","Ahmed","Usman","Zain","Hamza","Bilal","Zainab","latif","sulman","rafeeq","rasheed","haneef","kashif","sabir","sadiq","shareef","ramzan","rajab","farooq","sona","Ahmad Raza"];

setInterval(()=>{
    let popup = document.getElementById("popup");
    let name = names[Math.floor(Math.random()*names.length)];

    popup.innerText = name + " unlocked premium access";

    popup.style.left = "10px";

    et selected = "";

let validCodes = ["P1001","P1002","P1003","P1004","P1005"]; // sample (baaki tum add kar sakte ho)
    

    setTimeout(()=>{
        popup.style.left = "-300px";
    },2000);

},4000);

</script>

</body>
</html>
