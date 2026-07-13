# choihappy0320-coder.github.io
<!DOCTYPE html>
<html lang="ko">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Behind the Veil | Experience Rawls' Theory of Justice</title>

<link rel="stylesheet" href="style.css">

<link rel="preconnect" href="https://fonts.googleapis.com">

<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@300;400;500;700;900&display=swap" rel="stylesheet">

</head>

<body>

<nav>

<div class="logo">

Behind the Veil

</div>

<ul>

<li><a href="#about">About</a></li>

<li><a href="#learn">Theory</a></li>

<li><a href="#experience">Experience</a></li>

</ul>

</nav>

<header class="hero">

<div class="overlay">

<h1>

Behind the Veil

</h1>

<h2>

Experience Rawls' Theory of Justice

</h2>

<p>

What kind of society would you choose if you didn't know who you would become?

</p>

<a href="#about" class="btn">

Start Experience

</a>

</div>

</header>

<section id="about">

<div class="container">

<h2>

About This Project

</h2>

<p>

이 웹사이트는 정치철학자 존 롤스(John Rawls)의

<strong>무지의 베일(Veil of Ignorance)</strong>

사고실험을 직접 체험할 수 있도록 제작되었습니다.

</p>

<p>

당신은 자신이 어떤 사람으로 태어날지 모르는 상태에서

사회제도를 설계하게 됩니다.

그 후 무작위 사회적 위치를 부여받아

자신의 선택을 다시 돌아보게 됩니다.

</p>

</div>

</section>

<section id="learn">

<div class="container">

<h2>

Key Concepts

</h2>

<div class="card-grid">

<div class="card">

<h3>

Veil of Ignorance

</h3>

<p>

자신의 능력,

경제력,

국적,

성별,

사회적 지위를 모르는 상태에서

사회를 설계하는 사고실험입니다.

</p>

</div>

<div class="card">

<h3>

Equal Liberty

</h3>

<p>

모든 사람은

동등한 기본적 자유를

누릴 권리를 가진다는 원칙입니다.

</p>

</div>

<div class="card">

<h3>

Difference Principle

</h3>

<p>

사회적 불평등은

가장 불리한 사람에게도

이익이 될 때만

정당화될 수 있습니다.

</p>

</div>

</div>

</div>

</section>

<section id="experience">

<div class="container">

<h2>

Design Your Society

</h2>

<p>

다음 질문에 답하면서

당신만의 사회를 설계해보세요.

</p>

<button id="startQuiz">

Begin

</button>

</div>

</section>

<section id="quiz" class="hidden">

<div class="container">

<div id="progress">

Question

<span id="currentQuestion">

1

</span>

/ 10

</div>

<h2 id="questionBox">

</h2>

<div id="answerBox">

</div>

<button id="nextBtn">

Next

</button>

</div>

</section>
<section id="result" class="hidden">

<div class="container">

<h2>

Your Result

</h2>

<div class="result-card">

<h3 id="identity">

</h3>

<p id="analysis">

</p>

<div class="score-box">

<h4>

Justice Score

</h4>

<h1 id="score">

0

</h1>

<p>

/100</p>

</div>

<button id="restart">

Try Again

</button>

</div>

</div>

</section>

<section id="reflection" class="hidden">

<div class="container">

<h2>

Reflection

</h2>

<p>

무지의 베일 아래에서 설계한 사회를 다시 돌아보세요.

현재도 같은 선택을 하시겠습니까?

</p>

<textarea

id="reflectionText"

placeholder="이번 체험을 통해 느낀 점을 자유롭게 작성해보세요."

></textarea>

<div class="reflection-buttons">

<button id="saveBtn">

Save Reflection

</button>

<button id="clearBtn">

Clear

</button>

</div>

</div>

</section>

<footer>

<div class="container">

<h2>

Behind the Veil

</h2>

<p>

Experience Rawls' Theory of Justice

</p>

<hr>

<p>

Created by

<strong>

최준우

</strong>

</p>

<p>

Political Science · International Relations

</p>

<p>

Educational Web Project based on John Rawls

</p>

</div>

</footer>

<script src="script.js"></script>

</body>

</html>
/* =========================================
   Behind the Veil
   style.css
========================================= */

*{
margin:0;
padding:0;
box-sizing:border-box;
}

html{
scroll-behavior:smooth;
}

body{

font-family:"Noto Sans KR",sans-serif;

background:#f5f7fb;

color:#222;

line-height:1.8;

}

/* ---------------- NAV ---------------- */

nav{

position:fixed;

top:0;

left:0;

width:100%;

display:flex;

justify-content:space-between;

align-items:center;

padding:20px 80px;

background:rgba(255,255,255,.82);

backdrop-filter:blur(18px);

box-shadow:0 2px 12px rgba(0,0,0,.05);

z-index:1000;

}

.logo{

font-size:28px;

font-weight:900;

color:#1d4ed8;

}

nav ul{

display:flex;

gap:35px;

list-style:none;

}

nav a{

text-decoration:none;

color:#333;

font-weight:600;

transition:.3s;

}

nav a:hover{

color:#2563eb;

}

/* ---------------- HERO ---------------- */

.hero{

height:100vh;

display:flex;

justify-content:center;

align-items:center;

text-align:center;

background:

linear-gradient(

135deg,

#dbeafe,

#eff6ff,

white);

}

.overlay{

max-width:900px;

padding:40px;

}

.hero h1{

font-size:78px;

font-weight:900;

margin-bottom:15px;

color:#1e3a8a;

}

.hero h2{

font-size:32px;

font-weight:600;

margin-bottom:30px;

color:#475569;

}

.hero p{

font-size:22px;

margin-bottom:45px;

color:#555;

}

/* ---------------- BUTTON ---------------- */

.btn,

button{

padding:16px 40px;

border:none;

border-radius:999px;

background:#2563eb;

color:white;

font-size:18px;

font-weight:700;

cursor:pointer;

transition:.3s;

}

.btn{

display:inline-block;

text-decoration:none;

}

button:hover,

.btn:hover{

background:#1d4ed8;

transform:translateY(-3px);

}

/* ---------------- SECTION ---------------- */

section{

padding:100px 20px;

}

.container{

max-width:1100px;

margin:auto;

}

section h2{

text-align:center;

font-size:42px;

margin-bottom:35px;

color:#1e3a8a;

}

section p{

font-size:18px;

margin-bottom:20px;

}

/* ---------------- CARD ---------------- */

.card-grid{

display:grid;

grid-template-columns:

repeat(auto-fit,minmax(260px,1fr));

gap:30px;

margin-top:40px;

}

.card{

background:white;

padding:35px;

border-radius:25px;

box-shadow:

0 12px 30px

rgba(0,0,0,.08);

transition:.3s;

}

.card:hover{

transform:translateY(-8px);

}

.card h3{

color:#2563eb;

margin-bottom:15px;

}

/* ---------------- EXPERIENCE ---------------- */

#experience{

text-align:center;

}

/* ---------------- QUIZ ---------------- */

#quiz{

text-align:center;

}

#progress{

font-size:18px;

color:#666;

margin-bottom:25px;

}

#questionBox{

font-size:34px;

margin-bottom:40px;

font-weight:700;

}

#answerBox{

display:flex;

flex-direction:column;

gap:20px;

margin-bottom:35px;

}

.option{

padding:18px;

border-radius:18px;

background:white;

border:2px solid #dbeafe;

cursor:pointer;

transition:.25s;

font-size:18px;

}

.option:hover{

border-color:#2563eb;

transform:translateY(-2px);

}

.option.selected{

background:#dbeafe;

border-color:#2563eb;

}
/* ---------------- RESULT ---------------- */

#result{

text-align:center;

}

.result-card{

background:white;

padding:50px;

border-radius:30px;

box-shadow:

0 15px 35px

rgba(0,0,0,.08);

max-width:700px;

margin:auto;

}

#identity{

font-size:32px;

color:#2563eb;

margin-bottom:25px;

}

#analysis{

font-size:19px;

margin-bottom:40px;

color:#444;

line-height:1.8;

}

.score-box{

margin:35px auto;

padding:30px;

border-radius:25px;

background:

linear-gradient(

135deg,

#dbeafe,

white);

}

.score-box h4{

font-size:20px;

color:#555;

margin-bottom:10px;

}

.score-box h1{

font-size:90px;

color:#1d4ed8;

margin-bottom:5px;

}

/* ---------------- REFLECTION ---------------- */

#reflection{

text-align:center;

}

#reflection textarea{

width:100%;

max-width:900px;

height:220px;

padding:20px;

margin-top:30px;

margin-bottom:30px;

font-size:17px;

border-radius:20px;

border:1px solid #d1d5db;

resize:vertical;

outline:none;

transition:.3s;

}

#reflection textarea:focus{

border-color:#2563eb;

box-shadow:

0 0 10px

rgba(37,99,235,.15);

}

.reflection-buttons{

display:flex;

justify-content:center;

gap:20px;

flex-wrap:wrap;

}

#clearBtn{

background:#6b7280;

}

#clearBtn:hover{

background:#4b5563;

}

/* ---------------- FOOTER ---------------- */

footer{

margin-top:100px;

padding:60px 20px;

background:#0f172a;

color:white;

text-align:center;

}

footer h2{

font-size:34px;

margin-bottom:10px;

}

footer hr{

width:120px;

margin:25px auto;

border:none;

height:2px;

background:rgba(255,255,255,.3);

}

footer p{

margin:10px 0;

color:#d1d5db;

}

/* ---------------- UTIL ---------------- */

.hidden{

display:none;

}

/* ---------------- SCROLL ANIMATION ---------------- */

.hero,

.card,

.result-card{

animation:fadeUp .9s ease;

}

@keyframes fadeUp{

from{

opacity:0;

transform:translateY(40px);

}

to{

opacity:1;

transform:translateY(0);

}

}

/* ---------------- MOBILE ---------------- */

@media(max-width:900px){

nav{

padding:18px 25px;

}

nav ul{

display:none;

}

.hero h1{

font-size:52px;

}

.hero h2{

font-size:24px;

}

.hero p{

font-size:18px;

}

section h2{

font-size:34px;

}

#questionBox{

font-size:26px;

}

.score-box h1{

font-size:60px;

}

.result-card{

padding:30px;

}

}

@media(max-width:600px){

button,

.btn{

width:100%;

}

.option{

font-size:16px;

padding:16px;

}

.reflection-buttons{

flex-direction:column;

}

footer h2{

font-size:28px;

}

}
// =====================================
// Behind the Veil
// script.js
// Part 1
// =====================================

const questions = [

{
question:"교육 제도를 선택하세요.",
answers:[
{text:"모든 교육 무상",score:10},
{text:"초중등 무상",score:7},
{text:"대학만 지원",score:5},
{text:"개인 부담",score:0}
]
},

{
question:"의료 제도를 선택하세요.",
answers:[
{text:"무상의료",score:10},
{text:"혼합형",score:5},
{text:"민간보험 중심",score:0}
]
},

{
question:"세금 정책을 선택하세요.",
answers:[
{text:"누진세 강화",score:10},
{text:"현행 유지",score:5},
{text:"감세",score:0}
]
},

{
question:"기후변화 책임은?",
answers:[
{text:"선진국이 더 부담",score:10},
{text:"공동 부담",score:5},
{text:"각국 자율",score:0}
]
},

{
question:"난민 정책은?",
answers:[
{text:"적극 수용",score:10},
{text:"제한적 수용",score:5},
{text:"수용 거부",score:0}
]
},

{
question:"복지 수준은?",
answers:[
{text:"높은 복지",score:10},
{text:"중간 수준",score:5},
{text:"최소 복지",score:0}
]
},

{
question:"장애인 지원은?",
answers:[
{text:"국가 적극 지원",score:10},
{text:"일부 지원",score:5},
{text:"민간 중심",score:0}
]
},

{
question:"국제 원조는?",
answers:[
{text:"확대",score:10},
{text:"현행 유지",score:5},
{text:"축소",score:0}
]
},

{
question:"최저임금 정책은?",
answers:[
{text:"생활임금 보장",score:10},
{text:"현행 유지",score:5},
{text:"시장 자율",score:0}
]
},

{
question:"당신이 가장 중요하게 생각하는 가치는?",
answers:[
{text:"사회적 약자 보호",score:10},
{text:"자유와 평등의 균형",score:5},
{text:"자유 경쟁",score:0}
]
}

];

const identities=[

"대한민국 일반고 학생",
"대한민국 저소득층 청소년",
"대한민국 농어촌 학생",
"기후난민",
"투발루 주민",
"방글라데시 농민",
"미국 CEO",
"독일 대학생",
"북한 주민",
"UN 난민캠프 청소년",
"한부모 가정 자녀",
"시각장애인",
"청각장애인",
"중증질환 환자",
"소규모 자영업자",
"아프리카 농촌 주민",
"개발도상국 여성",
"국제기구 직원",
"고령 독거노인",
"신생아"

];

let currentQuestion=0;
let totalScore=0;
let selectedScore=null;

const startQuiz=document.getElementById("startQuiz");

const quiz=document.getElementById("quiz");

const questionBox=document.getElementById("questionBox");

const answerBox=document.getElementById("answerBox");

const nextBtn=document.getElementById("nextBtn");

const current=document.getElementById("currentQuestion");

startQuiz.addEventListener("click",()=>{

document.getElementById("experience").classList.add("hidden");

quiz.classList.remove("hidden");

showQuestion();

});

function showQuestion(){

selectedScore=null;

nextBtn.disabled=true;

current.textContent=currentQuestion+1;

const q=questions[currentQuestion];

questionBox.textContent=q.question;

answerBox.innerHTML="";

q.answers.forEach(answer=>{

const div=document.createElement("div");

div.className="option";

div.textContent=answer.text;

div.addEventListener("click",()=>{

document.querySelectorAll(".option").forEach(op=>{

op.classList.remove("selected");

});

div.classList.add("selected");

selectedScore=answer.score;

nextBtn.disabled=false;

});

answerBox.appendChild(div);

});

}
// =====================================
// Behind the Veil
// script.js
// Part 2
// =====================================

nextBtn.addEventListener("click",()=>{

if(selectedScore===null)return;

totalScore+=selectedScore;

currentQuestion++;

if(currentQuestion<questions.length){

showQuestion();

}else{

showResult();

}

});

function showResult(){

quiz.classList.add("hidden");

document.getElementById("result").classList.remove("hidden");

document.getElementById("reflection").classList.remove("hidden");

const randomIdentity=
identities[Math.floor(Math.random()*identities.length)];

document.getElementById("identity").innerHTML=
"🎲 당신은 <strong>"+randomIdentity+"</strong>(으)로 태어났습니다.";

let message="";

if(totalScore>=90){

message=
"당신은 가장 불리한 사람도 충분히 고려하는 사회를 설계했습니다. 이는 롤스의 차등의 원리와 평등한 자유의 원칙에 매우 가까운 선택입니다.";

}

else if(totalScore>=70){

message=
"당신은 자유와 평등의 균형을 고려한 사회를 설계했습니다. 다만 일부 제도는 사회적 약자를 충분히 보호하지 못할 수도 있습니다.";

}

else if(totalScore>=40){

message=
"당신의 사회는 개인의 자유를 비교적 중요하게 생각합니다. 무지의 베일 아래에서도 같은 선택을 할 것인지 다시 생각해 볼 필요가 있습니다.";

}

else{

message=
"당신의 사회는 경쟁과 효율을 우선합니다. 롤스의 관점에서는 가장 불리한 사람의 권리가 충분히 보장되지 않을 가능성이 큽니다.";

}

document.getElementById("analysis").innerHTML=message;

document.getElementById("score").textContent=totalScore;

}

document.getElementById("restart").addEventListener("click",()=>{

location.reload();

});

const saveBtn=document.getElementById("saveBtn");

const clearBtn=document.getElementById("clearBtn");

const reflection=document.getElementById("reflectionText");

window.addEventListener("load",()=>{

const saved=localStorage.getItem("veilReflection");

if(saved){

reflection.value=saved;

}

});

saveBtn.addEventListener("click",()=>{

localStorage.setItem("veilReflection",reflection.value);

alert("성찰 내용이 저장되었습니다.");

});

clearBtn.addEventListener("click",()=>{

if(confirm("작성한 내용을 삭제하시겠습니까?")){

localStorage.removeItem("veilReflection");

reflection.value="";

}

});

// Enter 키 방지
reflection.addEventListener("keydown",(e)=>{

if(e.key==="Tab") return;

});

// 콘솔 메시지
console.log("Behind the Veil");
console.log("Experience Rawls' Theory of Justice");

// 제작자 정보
console.log("Created by Choi Junwoo");
