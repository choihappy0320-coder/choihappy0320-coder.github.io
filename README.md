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

    <link href="https://fonts.googleapis.com/css2?family=Pretendard:wght@300;400;500;600;700&display=swap" rel="stylesheet">

</head>

<body>

<nav class="navbar">

<div class="logo">
Behind the Veil
</div>

<ul>

<li><a href="#about">About</a></li>

<li><a href="#learn">Learn</a></li>

<li><a href="#experience">Experience</a></li>

</ul>

</nav>



<header class="hero">

<div class="hero-content">

<h1>Behind the Veil</h1>

<h2>
Experience Rawls' Theory of Justice
</h2>

<p>

"What kind of society would you choose if you didn't know who you would become?"

</p>

<a href="#about" class="btn">
Start Experience
</a>

</div>

</header>




<section id="about" class="glass">

<h2>About</h2>

<p>

존 롤스(John Rawls)는 사람들이 자신이 어떤 사람으로 태어날지 모르는 상태,
즉 <strong>무지의 베일(Veil of Ignorance)</strong> 아래에서 사회를 설계한다면
가장 공정한 제도를 선택할 것이라고 주장했습니다.

</p>

<p>

이 사이트에서는 당신이 직접 사회 제도를 설계한 뒤,
무작위 사회적 위치를 부여받아
그 선택이 누구에게 어떤 영향을 미치는지 체험할 수 있습니다.

</p>

</section>





<section id="learn">

<h2>Rawls' Key Concepts</h2>

<div class="cards">

<div class="card">

<h3>Veil of Ignorance</h3>

<p>

자신의 능력,
부,
국적,
성별,
사회적 지위를 모르는 상태에서
사회를 설계하는 사고실험입니다.

</p>

</div>

<div class="card">

<h3>Equal Liberty</h3>

<p>

모든 사람은
동등한 자유를 누릴 권리가 있습니다.

</p>

</div>

<div class="card">

<h3>Difference Principle</h3>

<p>

불평등은
가장 불리한 사람에게도
이익이 될 때만 정당화될 수 있습니다.

</p>

</div>

</div>

</section>





<section id="experience">

<h2>Build Your Society</h2>

<p>

다음 질문에 답하며
당신이 생각하는 가장 정의로운 사회를 설계해 보세요.

</p>

<button id="startQuiz" class="btn">

Start

</button>

</section>






<section id="quiz" class="hidden">

<h2>Question</h2>

<div id="questionBox">

</div>

<div id="answerBox">

</div>

<button id="nextBtn" class="btn">

Next

</button>

</section>






<section id="result" class="hidden">

<h2>Your Result</h2>

<h3 id="identity">

</h3>

<p id="analysis">

</p>

<div class="score">

<span>

Justice Score

</span>

<h1 id="score">

0

</h1>

</div>

<button id="restart" class="btn">

Try Again

</button>

</section>






<section id="reflection" class="hidden">

<h2>Reflection</h2>

<p>

당신은 지금도 같은 사회를 선택하시겠습니까?

</p>

<textarea

id="reflectionText"

placeholder="이번 체험을 통해 느낀 점을 작성해 보세요."

></textarea>

<button id="saveBtn" class="btn">

Save Reflection

</button>

</section>






<footer>

<p>

Created by

<strong>최준우</strong>

</p>

<p>

Political Science &
International Relations

</p>

<p>

Inspired by John Rawls

</p>

</footer>

<script src="script.js"></script>

</body>

</html>
/* =========================
   Behind the Veil
   style.css
========================= */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{

    font-family:
    "Pretendard",
    "Noto Sans KR",
    -apple-system,
    BlinkMacSystemFont,
    "Segoe UI",
    sans-serif;

    background:
    linear-gradient(
    135deg,
    #eef3ff,
    #f8fbff);

    color:#222;

    line-height:1.7;
}


/* ================= NAV ================= */

.navbar{

    position:fixed;

    top:0;

    width:100%;

    display:flex;

    justify-content:space-between;

    align-items:center;

    padding:18px 60px;

    backdrop-filter:blur(20px);

    background:rgba(255,255,255,.72);

    border-bottom:1px solid rgba(255,255,255,.4);

    z-index:999;

}

.logo{

    font-size:24px;

    font-weight:700;

    color:#2b4eff;

}

.navbar ul{

    display:flex;

    list-style:none;

    gap:40px;

}

.navbar a{

    color:#333;

    text-decoration:none;

    font-weight:600;

    transition:.25s;

}

.navbar a:hover{

    color:#2b4eff;

}


/* ================= HERO ================= */

.hero{

    height:100vh;

    display:flex;

    justify-content:center;

    align-items:center;

    text-align:center;

    padding:40px;

    background:
    radial-gradient(circle at top,
    #dce9ff,
    #eef3ff,
    white);

}

.hero-content{

    max-width:850px;

}

.hero h1{

    font-size:72px;

    font-weight:800;

    margin-bottom:15px;

    color:#1d2d50;

}

.hero h2{

    font-size:32px;

    font-weight:600;

    color:#4d5f80;

    margin-bottom:35px;

}

.hero p{

    font-size:21px;

    color:#666;

    margin-bottom:45px;

}


/* ================= BUTTON ================= */

.btn{

    display:inline-block;

    padding:16px 38px;

    border:none;

    border-radius:999px;

    background:#2b4eff;

    color:white;

    font-size:18px;

    font-weight:600;

    cursor:pointer;

    text-decoration:none;

    transition:.3s;

    box-shadow:
    0 10px 25px
    rgba(43,78,255,.25);

}

.btn:hover{

    transform:translateY(-3px);

    background:#2142dd;

}

.btn:active{

    transform:scale(.97);

}


/* ================= SECTION ================= */

section{

    max-width:1100px;

    margin:120px auto;

    padding:0 25px;

}

section h2{

    text-align:center;

    font-size:42px;

    margin-bottom:30px;

    color:#23395d;

}


/* ================= GLASS ================= */

.glass{

    background:rgba(255,255,255,.72);

    backdrop-filter:blur(18px);

    border-radius:28px;

    padding:55px;

    box-shadow:

    0 20px 40px

    rgba(0,0,0,.08);

}


/* ================= CARDS ================= */

.cards{

    display:grid;

    grid-template-columns:

    repeat(auto-fit,minmax(250px,1fr));

    gap:30px;

}

.card{

    background:white;

    border-radius:22px;

    padding:35px;

    text-align:center;

    transition:.35s;

    box-shadow:

    0 15px 30px

    rgba(0,0,0,.06);

}

.card:hover{

    transform:translateY(-8px);

}

.card h3{

    margin-bottom:18px;

    color:#2b4eff;

}


/* ================= EXPERIENCE ================= */

#experience{

    text-align:center;

}

#experience p{

    margin-bottom:35px;

    font-size:20px;

}


/* ================= QUIZ ================= */

#quiz{

    background:white;

    border-radius:25px;

    padding:50px;

    box-shadow:

    0 15px 35px

    rgba(0,0,0,.08);

}

#questionBox{

    font-size:30px;

    font-weight:700;

    margin-bottom:35px;

    color:#23395d;

}

#answerBox{

    display:flex;

    flex-direction:column;

    gap:15px;

    margin-bottom:40px;

}

.option{

    padding:18px;

    border-radius:16px;

    background:#edf3ff;

    cursor:pointer;

    transition:.25s;

    border:2px solid transparent;

}

.option:hover{

    border-color:#2b4eff;

    background:white;

}

.option.selected{

    border-color:#2b4eff;

    background:#dfe8ff;

}


/* ================= RESULT ================= */

#result{

    text-align:center;

    background:white;

    border-radius:25px;

    padding:55px;

    box-shadow:

    0 15px 35px

    rgba(0,0,0,.08);

}

.score{

    margin:45px auto;

}

.score span{

    font-size:18px;

    color:#777;

}

.score h1{

    font-size:90px;

    color:#2b4eff;

}


/* ================= REFLECTION ================= */

#reflection{

    text-align:center;

}

textarea{

    width:100%;

    min-height:220px;

    margin:35px 0;

    padding:20px;

    border-radius:18px;

    border:1px solid #d8d8d8;

    resize:vertical;

    font-size:17px;

    font-family:inherit;

}


/* ================= FOOTER ================= */

footer{

    margin-top:120px;

    padding:60px;

    text-align:center;

    background:#1f2a44;

    color:white;

}

footer p{

    margin:10px 0;

}


/* ================= UTIL ================= */

.hidden{

    display:none;

}


/* ================= ANIMATION ================= */

.hero-content{

    animation:fadeUp 1s ease;

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


/* ================= MOBILE ================= */

@media(max-width:768px){

.navbar{

padding:18px 22px;

}

.navbar ul{

display:none;

}

.hero h1{

font-size:46px;

}

.hero h2{

font-size:24px;

}

.hero p{

font-size:18px;

}

section h2{

font-size:32px;

}

.glass{

padding:35px;

}

.score h1{

font-size:60px;

}

}
// ------------------------
// Behind the Veil
// script.js
// ------------------------

const questions = [
{
question: "교육 제도를 선택하세요.",
answers: [
{ text: "모든 교육 무상", score: 10 },
{ text: "대학만 지원", score: 5 },
{ text: "개인 부담", score: 0 }
]
},
{
question: "의료 제도를 선택하세요.",
answers: [
{ text: "무상의료", score: 10 },
{ text: "혼합형", score: 5 },
{ text: "민간보험", score: 0 }
]
},
{
question: "세금 정책을 선택하세요.",
answers: [
{ text: "누진세", score: 10 },
{ text: "비례세", score: 5 },
{ text: "감세", score: 0 }
]
},
{
question: "기후변화 책임은?",
answers: [
{ text: "선진국이 더 부담", score: 10 },
{ text: "공동 부담", score: 5 },
{ text: "각국 자율", score: 0 }
]
},
{
question: "난민 정책은?",
answers: [
{ text: "적극 수용", score: 10 },
{ text: "제한적 수용", score: 5 },
{ text: "수용 거부", score: 0 }
]
},
{
question: "복지 수준은?",
answers: [
{ text: "높은 복지", score: 10 },
{ text: "적당한 복지", score: 5 },
{ text: "최소 복지", score: 0 }
]
},
{
question: "최저임금 정책은?",
answers: [
{ text: "생활임금 보장", score: 10 },
{ text: "현행 유지", score: 5 },
{ text: "시장 자율", score: 0 }
]
},
{
question: "장애인 지원은?",
answers: [
{ text: "국가 적극 지원", score: 10 },
{ text: "일부 지원", score: 5 },
{ text: "개인 책임", score: 0 }
]
},
{
question: "국제원조는?",
answers: [
{ text: "확대", score: 10 },
{ text: "현행 유지", score: 5 },
{ text: "축소", score: 0 }
]
},
{
question: "당신은 어떤 사회를 만들겠습니까?",
answers: [
{ text: "약자를 우선 보호", score: 10 },
{ text: "균형 추구", score: 5 },
{ text: "자유 경쟁", score: 0 }
]
}
];

const identities = [
"대한민국 일반고 학생",
"대한민국 저소득층 청소년",
"미국 CEO",
"방글라데시 농민",
"기후난민",
"시각장애인",
"청각장애인",
"한부모 가정 자녀",
"북한 주민",
"독일 대학생",
"투발루 주민",
"중증질환 환자",
"소규모 자영업자",
"아프리카 농촌 주민",
"UN 난민캠프 청소년"
];

let current = 0;
let score = 0;

const startBtn = document.getElementById("startQuiz");
const quiz = document.getElementById("quiz");
const questionBox = document.getElementById("questionBox");
const answerBox = document.getElementById("answerBox");
const nextBtn = document.getElementById("nextBtn");

const result = document.getElementById("result");
const identity = document.getElementById("identity");
const analysis = document.getElementById("analysis");
const scoreText = document.getElementById("score");

const reflection = document.getElementById("reflection");
const restart = document.getElementById("restart");

let selected = null;

startBtn.addEventListener("click", function(){

document.getElementById("experience").style.display="none";

quiz.classList.remove("hidden");

showQuestion();

});

function showQuestion(){

selected = null;

nextBtn.disabled = true;

const q = questions[current];

questionBox.innerHTML =
`<h3>${current+1}. ${q.question}</h3>`;

answerBox.innerHTML = "";

q.answers.forEach(function(answer){

const div = document.createElement("div");

div.className = "option";

div.innerText = answer.text;

div.onclick = function(){

document.querySelectorAll(".option").forEach(function(o){

o.classList.remove("selected");

});

div.classList.add("selected");

selected = answer.score;

nextBtn.disabled = false;

}

answerBox.appendChild(div);

});

}

nextBtn.addEventListener("click",function(){

if(selected===null) return;

score += selected;

current++;

if(current<questions.length){

showQuestion();

}else{

finish();

}

});

function finish(){

quiz.classList.add("hidden");

result.classList.remove("hidden");

reflection.classList.remove("hidden");

const person =
identities[Math.floor(Math.random()*identities.length)];

identity.innerHTML =
`🎲 당신은 <strong>${person}</strong>(으)로 태어났습니다.`;

let message="";

if(score>=80){

message=
"당신은 가장 불리한 사람도 고려하는 사회를 설계했습니다. 롤스의 차등의 원리에 비교적 가까운 선택입니다.";

}else if(score>=50){

message=
"자유와 평등을 모두 고려했지만, 일부 제도는 사회적 약자를 충분히 보호하지 못할 수 있습니다.";

}else{

message=
"당신은 자유 경쟁을 우선하는 사회를 설계했습니다. 무지의 베일 아래에서도 같은 선택을 할지 다시 생각해 볼 필요가 있습니다.";

}

analysis.innerHTML=message;

scoreText.innerHTML=score+" / 100";

}

restart.addEventListener("click",function(){

location.reload();

});

document.getElementById("saveBtn").addEventListener("click",function(){

const text=document.getElementById("reflectionText").value;

localStorage.setItem("BehindTheVeilReflection",text);

alert("성찰 내용이 저장되었습니다.");

});

window.onload=function(){

const saved=
localStorage.getItem("BehindTheVeilReflection");

if(saved){

document.getElementById("reflectionText").value=saved;

}

}
