# choihappy0320-coder.github.io
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
