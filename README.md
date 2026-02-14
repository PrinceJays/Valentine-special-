<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Prince ❤️ Iksha Forever</title>

<link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Poppins:wght@300;500&display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>

<style>
*{margin:0;padding:0;box-sizing:border-box;}

body{
font-family:'Poppins',sans-serif;
background:linear-gradient(135deg,#ff758c,#ff7eb3);
color:white;
text-align:center;
overflow-x:hidden;
scroll-behavior:smooth;
}

section{
min-height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
padding:40px;
position:relative;
}

h1{
font-family:'Great Vibes',cursive;
font-size:65px;
margin-bottom:20px;
}

h2{
font-size:35px;
margin-bottom:20px;
}

p{
max-width:800px;
line-height:1.8;
font-size:18px;
margin-bottom:20px;
}

button{
padding:15px 35px;
font-size:18px;
border:none;
border-radius:30px;
background:white;
color:#ff4e8d;
cursor:pointer;
transition:0.4s;
}

button:hover{transform:scale(1.1);}

img{
width:320px;
border-radius:20px;
box-shadow:0 0 30px rgba(255,255,255,0.6);
margin-top:20px;
}

.timeline{
text-align:left;
max-width:600px;
}

.timeline div{
margin:20px 0;
padding:15px;
background:rgba(255,255,255,0.2);
border-radius:15px;
}

.hidden{display:none;}

.heart{
position:fixed;
bottom:-10px;
color:rgba(255,255,255,0.7);
animation:float 8s infinite;
}

@keyframes float{
0%{transform:translateY(0) scale(1);}
100%{transform:translateY(-100vh) scale(1.5);}
}

#letter{
border-right:2px solid white;
white-space:pre-line;
overflow:hidden;
max-width:800px;
margin-top:20px;
}

</style>
</head>

<body>

<audio autoplay loop>
<source src="love.mp3" type="audio/mpeg">
</audio>

<!-- Floating Hearts Script -->
<script>
setInterval(()=>{
let heart=document.createElement("div");
heart.className="heart";
heart.innerHTML="❤️";
heart.style.left=Math.random()*100+"vw";
heart.style.fontSize=(Math.random()*20+20)+"px";
document.body.appendChild(heart);
setTimeout(()=>{heart.remove();},8000);
},500);
</script>

<!-- Welcome -->
<section>
<h1>Prince ❤️ Iksha</h1>
<h2>6 Months of Pure Love</h2>
<p>From strangers online… to soulmates connected by heart.</p>
<button onclick="window.scrollBy({top:window.innerHeight,behavior:'smooth'})">
Begin Our Story ↓
</button>
</section>

<!-- Memory Timeline -->
<section>
<h2>Our Beautiful Journey</h2>
<div class="timeline">
<div>💬 The Day We First Texted — Just a simple hello… but destiny started.</div>
<div>😊 First Late Night Talk — When hours felt like minutes.</div>
<div>❤️ The Day We Said "I Love You" — The most beautiful feeling ever.</div>
<div>🎉 6 Months Together — Stronger bond, deeper love.</div>
</div>
<img src="ourlove.jpg" alt="Prince and Iksha">
</section>

<!-- Love Letter -->
<section>
<h2>A Letter From My Heart</h2>
<p id="letter"></p>
</section>

<!-- Gift Section -->
<section>
<h2>My Valentine Surprise For You</h2>
<p>
🌹 A bouquet of flowers to show my admiration  
🎂 A sweet cake to celebrate our love  
💍 A ring carrying my promise of forever  
</p>
</section>

<!-- Future Promise -->
<section>
<h2>My Promise To You</h2>
<p>
Iksha Thamsung…  
I don’t just want today.  
I want every tomorrow with you.  
I want to grow, succeed, and build our dream life together.  
No distance can weaken what we have.  
You are my peace. My happiness. My forever.
</p>
</section>

<!-- Final Proposal -->
<section>
<h2>Iksha…</h2>
<p>
Will you be my wifey…  
my Valentine…  
and my forever partner in this life?
</p>
<button onclick="finalProposal()">YES 💍❤️</button>

<div id="finalMessage" class="hidden">
<h2>She Said YES!!! 😭💖</h2>
<p>
Prince ❤️ Iksha  
Forever Begins Today.
</p>
</div>
</section>

<script>

// Typing Love Letter
const text = `My dearest Iksha,

Meeting you online was the best accident of my life.
In just six months, you became my safest place,
my biggest support,
and my sweetest love.

Even miles apart,
I feel you in my heart every single day.

I promise to work hard,
to build our future,
to protect our love,
and to choose you — always.

You are not just my girlfriend…
You are my forever.

Love,
Prince ❤️`;

let i=0;
function typing(){
if(i<text.length){
document.getElementById("letter").innerHTML+=text.charAt(i);
i++;
setTimeout(typing,40);
}
}
typing();

function finalProposal(){
confetti({particleCount:400,spread:160,origin:{y:0.6}});
document.getElementById("finalMessage").classList.remove("hidden");
}

</script>

</body>
</html>
