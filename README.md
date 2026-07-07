<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Preeti ❤️ Shubham</title>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial;
}

body{
background:#140012;
overflow-x:hidden;
color:white;
text-align:center;
}

h1{
margin-top:40px;
font-size:50px;
color:#ff5fa2;
animation:beat 1s infinite;
}

@keyframes beat{
0%{transform:scale(1);}
50%{transform:scale(1.08);}
100%{transform:scale(1);}
}

button{
padding:18px 35px;
font-size:22px;
border:none;
border-radius:40px;
background:#ff2d75;
color:white;
cursor:pointer;
margin-top:30px;
}

#content{
display:none;
padding:20px;
}

.photo{
width:250px;
border-radius:20px;
margin:10px;
box-shadow:0 0 20px hotpink;
}

.message{
font-size:22px;
margin-top:20px;
line-height:1.8;
}

.timer{
font-size:30px;
margin-top:20px;
color:#ffd2e8;
}

.heart{
position:fixed;
top:-30px;
font-size:25px;
animation:fall linear infinite;
}

@keyframes fall{
to{
transform:translateY(110vh);
}
}

.sparkle{
position:fixed;
width:4px;
height:4px;
background:white;
border-radius:50%;
animation:blink 2s infinite;
}

@keyframes blink{
50%{
opacity:.2;
}
}

</style>
</head>

<body>

<h1>❤️ Preeti ❤️ Shubham ❤️</h1>

<button onclick="openHeart()">
Open My Heart
</button>

<div id="content">

<img src="photo1.jpg" class="photo">
<img src="photo2.jpg" class="photo">

<p class="message">

The day we met became the most special day of my life ❤️

You are my smile...
My happiness...
My forever...

I Love You Shubham ❤️

Forever Yours,
Preeti

</p>

<div class="timer" id="timer"></div>

<audio controls autoplay loop>
<source src="song.mp3" type="audio/mpeg">
</audio>

</div>

<script>

function openHeart(){

document.querySelector("button").style.display="none";

document.getElementById("content").style.display="block";

}

for(let i=0;i<40;i++){

let h=document.createElement("div");

h.className="heart";

h.innerHTML=Math.random()>0.5?"❤️":"🌹";

h.style.left=Math.random()*100+"vw";

h.style.animationDuration=(5+Math.random()*5)+"s";

h.style.fontSize=(20+Math.random()*20)+"px";

document.body.appendChild(h);

}

for(let i=0;i<150;i++){

let s=document.createElement("div");

s.className="sparkle";

s.style.left=Math.random()*100+"vw";

s.style.top=Math.random()*100+"vh";

s.style.animationDelay=Math.random()*2+"s";

document.body.appendChild(s);

}

let start=new Date("2026-01-01");

setInterval(function(){

let now=new Date();

let diff=now-start;

let days=Math.floor(diff/86400000);

document.getElementById("timer").innerHTML=

"❤️ Together for "+days+" Days ❤️";

},1000);

</script>

</body>
</html># loves