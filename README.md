<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Love Dashboard ❤️</title>

<style>
body{
    margin:0;
    padding:0;
    font-family:Arial;
    background:linear-gradient(135deg,#ff4d6d,#111);
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    color:white;
}

.box{
    text-align:center;
    background:rgba(0,0,0,0.5);
    padding:40px;
    border-radius:20px;
    width:320px;
    box-shadow:0 0 20px rgba(255,255,255,0.3);
}

h1{
    font-size:40px;
    margin-bottom:20px;
}

button{
    padding:12px 25px;
    margin:10px;
    border:none;
    border-radius:12px;
    font-size:18px;
    cursor:pointer;
    transition:0.3s;
}

button:hover{
    transform:scale(1.1);
}

.love{
    background:#00ff88;
    color:black;
}

.hate{
    background:#ff0033;
    color:white;
}
</style>
</head>

<body>

<div class="box" id="mainBox">

    <h1>WELCOME ❤️</h1>

    <button onclick="openDashboard()">WELCOME</button>

</div>

<script>

function openDashboard(){

document.getElementById("mainBox").innerHTML = `

<h1>Do you play Minecraft</h1>

<p style="font-size:22px;">Choose One 👇</p>

<button class="love" onclick="love()">Yes💖</button>

<button class="hate" onclick="hate()">No💔</button>

`;

}

function love(){

document.getElementById("mainBox").innerHTML = `

<h1>Thanks 😍</h1>

<p style="font-size:25px;">thanks  💖</p>

`;

}

function hate(){

document.getElementById("mainBox").innerHTML = `

<h1>Do You Sure? 😢</h1>

<p>Choose Again 👇</p>

<button class="love" onclick="love()">Yes 💖</button>

<button class="hate" onclick="hate()">No💔</button>

`;

}

</script>

</body>
</html>
