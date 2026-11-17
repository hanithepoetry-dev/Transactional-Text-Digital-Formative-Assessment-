<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Formative Assessment: Identity and Family</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@500;600&family=Nunito:wght@500;700;800&display=swap" rel="stylesheet">
<style>
:root{--bg:#EAF6F3;--card:#fff;--ink:#17323A;--mute:#52707A;--teal:#0E6F73;--on:#fff;--sun:#FFC93C;--ok:#13805A;--okbg:#DDF5EA;--bad:#C23652;--badbg:#FDE5E9;--line:#C9E0DC;--soft:#F3FAF8;
--f1:"Fredoka","Trebuchet MS",sans-serif;--f2:"Nunito","Segoe UI",Arial,sans-serif;
box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#0F2327;--card:#17343A;--ink:#EAF4F2;--mute:#A3BDC1;--teal:#4CC3C0;--on:#0F2327;--ok:#5ADBA3;--okbg:#14412F;--bad:#FF93A5;--badbg:#4A1E28;--line:#2B4D53;--soft:#1C3D44}}
:root[data-theme="dark"]{--bg:#0F2327;--card:#17343A;--ink:#EAF4F2;--mute:#A3BDC1;--teal:#4CC3C0;--on:#0F2327;--ok:#5ADBA3;--okbg:#14412F;--bad:#FF93A5;--badbg:#4A1E28;--line:#2B4D53;--soft:#1C3D44}
*,*::before,*::after{box-sizing:inherit}
html{scroll-padding-top:env(safe-area-inset-top,0px);height:100%}
body{margin:0;min-height:100%;background:var(--bg);color:var(--ink);font:600 17px/1.55 var(--f2)}
.wrap{max-width:720px;margin:0 auto;padding:18px 16px 40px}
h1,h2,h3{font-family:var(--f1);font-weight:600;line-height:1.2;margin:0}
button{font:inherit;cursor:pointer;color:inherit}
:focus-visible{outline:3px solid var(--sun);outline-offset:2px}
.card{background:var(--card);border:2px solid var(--line);border-radius:22px;padding:22px}
.btn{border:0;border-radius:14px;padding:12px 22px;font-weight:800;background:var(--teal);color:var(--on);transition:transform .12s}
.btn:hover:not(:disabled){transform:translateY(-2px)}
.btn:disabled{opacity:.4;cursor:not-allowed}
.btn.alt{background:transparent;color:var(--teal);border:2px solid var(--teal)}
.hide{display:none!important}
/* welcome */
.pass{background:var(--teal);color:var(--on);border-radius:22px 22px 0 0;padding:26px 22px 20px;position:relative;overflow:hidden}
.pass h1{font-size:clamp(26px,6vw,38px)}
.pass p{margin:8px 0 0;font-weight:700;opacity:.92}
.pass::after{content:"";position:absolute;right:-30px;top:-30px;width:130px;height:130px;border-radius:50%;border:14px solid var(--sun);opacity:.85}
.body{background:var(--card);border:2px solid var(--line);border-top:0;border-radius:0 0 22px 22px;padding:22px}
.how{list-style:none;padding:0;margin:0 0 20px;display:grid;gap:10px}
.how li{display:flex;gap:12px;align-items:flex-start;background:var(--soft);border-radius:14px;padding:12px 14px}
.how b{flex:none;width:30px;height:30px;border-radius:50%;background:var(--sun);color:#17323A;display:grid;place-items:center;font-family:var(--f1)}
.meta{display:flex;gap:8px;flex-wrap:wrap;margin:0 0 18px}
.chip{background:var(--soft);border:2px solid var(--line);border-radius:99px;padding:3px 12px;font-size:14px;font-weight:800;color:var(--mute)}
/* stamps */
.stamps{display:flex;gap:6px;justify-content:space-between;margin-bottom:14px}
.st{flex:1;max-width:44px;aspect-ratio:1;border-radius:50%;border:2px dashed var(--line);background:var(--card);font:600 14px var(--f1);display:grid;place-items:center;padding:0;color:var(--mute)}
.st.cur{border:3px solid var(--teal);color:var(--teal);transform:scale(1.1)}
.st.ok{background:var(--okbg);border:2px solid var(--ok);color:var(--ok)}
.st.bad{background:var(--badbg);border:2px solid var(--bad);color:var(--bad)}
.bar{height:8px;background:var(--line);border-radius:9px;overflow:hidden;margin-bottom:6px}
.bar i{display:block;height:100%;background:var(--sun);width:0;transition:width .35s}
.count{display:flex;justify-content:space-between;font-size:15px;color:var(--mute);font-weight:800;margin-bottom:12px}
/* question */
.passage{background:var(--soft);border-left:6px solid var(--sun);border-radius:12px;padding:12px 14px;margin:0 0 14px;font-weight:700}
.passage div+div{margin-top:4px}
.q{font-size:clamp(20px,4.6vw,24px);margin:10px 0 16px}
.opts{display:grid;gap:10px}
.opt{display:flex;gap:12px;align-items:center;text-align:left;background:var(--card);border:2px solid var(--line);border-radius:16px;padding:12px 14px;width:100%;transition:border-color .15s,background .15s}
.opt:hover:not(:disabled){border-color:var(--teal);background:var(--soft)}
.opt .l{flex:none;width:34px;height:34px;border-radius:10px;background:var(--soft);border:2px solid var(--line);display:grid;place-items:center;font-family:var(--f1)}
.opt.picked{border-color:var(--teal)}
.opt.right{background:var(--okbg);border-color:var(--ok)}
.opt.right .l{background:var(--ok);border-color:var(--ok);color:var(--card)}
.opt.wrong{background:var(--badbg);border-color:var(--bad);animation:shake .35s}
.opt.wrong .l{background:var(--bad);border-color:var(--bad);color:var(--card)}
.opt:disabled{cursor:default}
.opt:disabled:not(.right):not(.wrong){opacity:.6}
@keyframes shake{25%{transform:translateX(-5px)}75%{transform:translateX(5px)}}
.fb{display:flex;gap:10px;margin-top:16px;align-items:flex-start}
.av{flex:none;width:40px;height:40px;border-radius:50%;background:var(--sun);display:grid;place-items:center;font-size:22px}
.bub{flex:1;border-radius:4px 16px 16px 16px;padding:12px 14px;border:2px solid}
.bub.ok{background:var(--okbg);border-color:var(--ok)}
.bub.no{background:var(--badbg);border-color:var(--bad)}
.bub strong{font-family:var(--f1);font-size:19px;display:block}
.bub p{margin:2px 0 0;font-weight:700}
.nav{display:flex;justify-content:space-between;gap:10px;margin-top:20px}
.warn{color:var(--bad);font-weight:800;margin:12px 0 0;min-height:1.4em}
/* result */
.res{text-align:center}
.ring{width:170px;height:170px;margin:6px auto 4px;position:relative}
.ring svg{transform:rotate(-90deg)}
.ring .n{position:absolute;inset:0;display:grid;place-content:center;font:600 46px/1 var(--f1)}
.ring .n small{font-size:15px;font-family:var(--f2);color:var(--mute);font-weight:800}
.tally{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin:16px 0}
.tally div{border-radius:16px;padding:12px;font-weight:800}
.tally b{display:block;font:600 30px var(--f1)}
.t1{background:var(--okbg);color:var(--ok)}.t2{background:var(--badbg);color:var(--bad)}
.msg{background:var(--soft);border:2px solid var(--line);border-radius:16px;padding:14px;text-align:left}
.msg h2{font-size:22px;margin-bottom:4px}
.rv{text-align:left;margin-top:22px}
.rv h2{font-size:22px;margin-bottom:10px}
.ri{border:2px solid var(--line);border-radius:16px;padding:12px 14px;margin-bottom:10px;background:var(--card)}
.ri.ok{border-left:8px solid var(--ok)}.ri.no{border-left:8px solid var(--bad)}
.ri h3{font-size:17px;font-family:var(--f2);font-weight:800}
.ri p{margin:6px 0 0;font-size:16px}
.ri .a{font-weight:800}
.acts{display:flex;gap:10px;justify-content:center;flex-wrap:wrap;margin-top:20px}
@media (prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important}}
@media (max-width:420px){.card,.body{padding:16px}.stamps{gap:3px}.st{font-size:12px}}
.idc{display:flex;gap:14px;align-items:center;background:linear-gradient(135deg,var(--teal),#1B9AA0);color:var(--on);border-radius:18px;padding:16px;margin:0 0 16px;box-shadow:0 8px 0 rgba(0,0,0,.12);animation:flip .9s cubic-bezier(.2,.8,.3,1.2) both}
@keyframes flip{from{transform:perspective(700px) rotateX(-80deg);opacity:0}}
.idc .ph{flex:none;width:64px;height:64px;border-radius:14px;background:var(--sun);color:#17323A;display:grid;place-items:center;font:600 30px var(--f1)}
.idc .ph.bump{animation:bump .3s}
@keyframes bump{50%{transform:scale(1.18) rotate(-6deg)}}
.idc small{display:block;opacity:.8;font-weight:800}
.idc strong{font:600 22px var(--f1);word-break:break-word}
.fm{display:grid;gap:10px;margin-bottom:14px}
.fm label{font-weight:800;font-size:15px;display:grid;gap:4px}
.fm input,.fm select{font:inherit;font-weight:700;padding:11px 12px;border-radius:12px;border:2px solid var(--line);background:var(--card);color:var(--ink)}
.fb.pop .bub{animation:pop .4s cubic-bezier(.2,.9,.3,1.3)}
.fb.pop .av{animation:bump .5s}
@keyframes pop{from{transform:scale(.7) translateY(14px);opacity:0}}
.st.pop{animation:bump .45s}
.card{animation:rise .35s both}
@keyframes rise{from{transform:translateY(10px);opacity:.3}}
.cf{position:fixed;pointer-events:none;z-index:50;font-size:22px}
.lnk{background:none;border:0;color:var(--mute);text-decoration:underline;font-weight:800;padding:8px}
.foot{text-align:center;margin:14px 0 0}
.tw{overflow-x:auto;margin:12px 0}
table{border-collapse:collapse;width:100%;min-width:480px;font-size:16px}
th,td{padding:9px 10px;text-align:left;border-bottom:2px solid var(--line)}
th{font-family:var(--f1);font-weight:600;background:var(--soft)}
.sm{font-size:15px;color:var(--mute);margin:0}
/* added: steps, modal, helpers */
.steps{display:flex;gap:6px;margin:0 0 14px}
.steps span{flex:1;text-align:center;padding:7px 4px;border-radius:99px;border:2px solid var(--line);background:var(--card);font-size:14px;font-weight:800;color:var(--mute)}
.steps span.on{background:var(--teal);border-color:var(--teal);color:var(--on)}
.steps span.dn{border-color:var(--teal);color:var(--teal)}
.btn.sun{background:var(--sun);color:#17323A}
.btn.small{padding:8px 14px;font-size:15px}
.fm input[readonly]{background:var(--soft);color:var(--mute)}
.fm label .sm{font-weight:700}
details.sm{margin:0 0 14px}
details.sm summary{cursor:pointer;font-weight:800}
details.sm p{margin:8px 0 0}
.mo{position:fixed;inset:0;background:rgba(15,35,39,.6);display:grid;place-items:center;padding:16px;z-index:60}
.md{background:var(--card);border:2px solid var(--line);border-radius:22px;padding:22px;max-width:560px;width:100%;max-height:85vh;overflow:auto;position:relative}
.md .x{position:absolute;right:10px;top:8px;font-size:20px;text-decoration:none}
.md ul{margin:8px 0 0;padding-left:20px}
</style>
</head>
<body>
<div class="wrap">
<div class="steps" id="steps" aria-hidden="true"><span>1 · About you</span><span>2 · Quiz</span><span>3 · Result</span></div>

<section id="welcome">
  <div class="pass">
    <h1>Formative Assessment: Identity and Family</h1>
    <p>Chapter 1 · Transactional Conversations</p>
  </div>
  <div class="body">
    <ul class="how">
      <li><b>1</b><span>Read each question and choose <strong>one</strong> answer: A, B, C, or D.</span></li>
      <li><b>2</b><span>You get feedback right after you answer. Read it to learn why.</span></li>
      <li><b>3</b><span>Use Previous and Next to move around. Tap a number to jump to a question.</span></li>
      <li><b>4</b><span>Answer all 10 questions, then press See my score.</span></li>
    </ul>
    <div class="meta"><span class="chip">10 questions</span><span class="chip">10 points each</span><span class="chip">Maximum score: 100</span><span class="chip">One attempt only</span></div>
    <div class="idc" aria-hidden="true"><div class="ph" id="ph">?</div><div><small>Student ID card</small><strong id="idn">Your name</strong><small id="idc">Class</small></div></div>
    <div class="fm">
      <label>Your full name<input id="nm" maxlength="40" autocomplete="name" placeholder="Example: Rina Nugroho"></label>
      <label>Your class<input id="cl" maxlength="12" placeholder="Example: VIII-A"></label>
      <label>Date<input id="dt" type="date"></label>
      <label id="tew">Your teacher’s email<input id="te" type="email" maxlength="80" autocomplete="off" placeholder="teacher@example.com"><span class="sm">Your result will be sent to this address.</span></label>
    </div>
    <details class="sm"><summary>For teachers</summary><p>Results go to the email typed above through FormSubmit. The first time, FormSubmit sends a one-time activation email to that address. Open the link in it (check spam), then send one test result. After that, every result arrives automatically.</p><p>To skip typing for students, share the link with your email added: <b>?to=teacher@example.com</b> at the end of the web address. Or write your email in CFG.teacher at the top of the script.</p></details>
    <button class="btn" id="start" type="button" disabled>Start Quiz</button>
    <p class="warn" id="ws" aria-live="polite"></p>
  </div>
</section>

<section id="quiz" class="hide">
  <div class="card">
    <div style="text-align:right;margin:0 0 12px"><button class="btn sun small" id="refbtn" type="button">📋 Quick guide</button></div>
    <div class="stamps" id="stamps" role="group" aria-label="Question numbers"></div>
    <div class="bar" aria-hidden="true"><i id="fill"></i></div>
    <div class="count"><span id="cnt">Question 1 of 10</span><span id="tag"></span></div>
    <div id="passage" class="passage hide"></div>
    <h2 class="q" id="qtext"></h2>
    <div class="opts" id="opts"></div>
    <div id="fb" aria-live="polite"></div>
    <div class="nav">
      <button class="btn alt" id="prev" type="button">Previous</button>
      <button class="btn" id="next" type="button">Next</button>
    </div>
    <p class="warn" id="warn" aria-live="polite"></p>
  </div>
</section>

<section id="result" class="hide">
  <div class="card res">
    <div class="ring"><svg width="170" height="170" viewBox="0 0 170 170"><circle cx="85" cy="85" r="74" fill="none" stroke="var(--line)" stroke-width="14"/><circle id="arc" cx="85" cy="85" r="74" fill="none" stroke="var(--sun)" stroke-width="14" stroke-linecap="round" stroke-dasharray="465" stroke-dashoffset="465" style="transition:stroke-dashoffset 1s"/></svg>
      <div class="n"><span id="score">0</span><small>out of 100</small></div></div>
    <div class="tally"><div class="t1"><b id="nok">0</b>Correct</div><div class="t2"><b id="nbad">0</b>Incorrect</div></div>
    <p class="chip" id="sent" style="margin:0 0 12px"></p>
    <div class="acts" style="margin:0 0 14px"><button class="btn alt" id="copy" type="button">Copy my result</button><button class="btn alt hide" id="resend" type="button">Send again</button></div>
    <div class="msg"><h2 id="mh"></h2><p id="mp" style="margin:0"></p></div>
    <div class="rv"><h2>Answer key and explanations</h2><div id="review"></div></div>
  </div>
</section>

<section id="dash" class="hide">
  <div class="card">
    <h2>Teacher dashboard</h2>
    <div id="lock" class="fm" style="margin-top:12px"><label>Teacher PIN<input id="pin" type="password" autocomplete="off"></label><button class="btn" id="unlock" type="button">Open dashboard</button></div>
    <div id="dbody" class="hide">
      <div class="acts" style="justify-content:flex-start;margin:10px 0 0"><select id="cf" class="chip" aria-label="Filter by class"></select><button class="btn alt" id="rf" type="button">Refresh</button><button class="btn alt" id="csv" type="button">Download CSV</button></div>
      <p class="sm" id="dsum" style="margin-top:10px"></p>
      <div class="tw"><table><thead><tr><th>Rank</th><th>Name</th><th>Class</th><th>Best score</th><th>Attempts</th></tr></thead><tbody id="rows"></tbody></table></div>
    </div>
    <p class="warn" id="dw"></p>
    <div class="acts"><button class="btn alt" id="back" type="button">Back to quiz</button></div>
  </div>
</section>
<p class="foot"><button class="lnk" id="tlink" type="button">Teacher dashboard</button></p>

</div>
<div class="mo hide" id="mo" role="dialog" aria-modal="true" aria-labelledby="mt">
  <div class="md">
    <button class="lnk x" id="mx" type="button" aria-label="Close">✕</button>
    <h2 id="mt">Quick guide</h2>
    <div class="tw"><table style="min-width:0"><thead><tr><th>Subject</th><th>Object</th><th>Possessive adjective</th><th>Possessive pronoun</th></tr></thead><tbody>
      <tr><td>I</td><td>me</td><td>my</td><td>mine</td></tr>
      <tr><td>you</td><td>you</td><td>your</td><td>yours</td></tr>
      <tr><td>he</td><td>him</td><td>his</td><td>his</td></tr>
      <tr><td>she</td><td>her</td><td>her</td><td>hers</td></tr>
      <tr><td>it</td><td>it</td><td>its</td><td>-</td></tr>
      <tr><td>we</td><td>us</td><td>our</td><td>ours</td></tr>
      <tr><td>they</td><td>them</td><td>their</td><td>theirs</td></tr>
    </tbody></table></div>
    <ul>
      <li>A dialogue has an opening, an exchange, and a closing.</li>
      <li>Simple present questions use do or does: “Do you have a sister?”</li>
      <li>With he, she, and it, the verb takes -s: works, has.</li>
      <li>A polite request: “May I have your name, please?”</li>
    </ul>
  </div>
</div>
<script>
var Q=[
{t:"Social function",q:"What is the main purpose of a transactional conversation about identity and family?",o:["To tell a long story about a holiday","To compare two school subjects","To ask for and give basic information about a person and the family","To describe a beautiful place"],a:2,why:"A transactional conversation is used to ask for and give basic information for a practical purpose. It also helps us get to know other people."},
{t:"Reading a dialogue",p:["Rina: Do you have any brothers or sisters?","Arman: Yes, I have a younger sister. Her name is Laila, and she is fourteen."],q:"Who is Laila?",o:["Arman’s younger sister","Rina’s younger sister","Arman’s classmate","Rina’s mother"],a:0,why:"Arman says, “I have a younger sister. Her name is Laila.” The word “Her” refers back to his sister."},
{t:"Possessive adjectives",q:"Choose the correct word: “This is my sister. ___ name is Laila.”",o:["She","He","Hers","Her"],a:3,why:"A possessive adjective comes before a noun. “Her” + name shows that the name belongs to a girl. We do not say “She name”."},
{t:"Object pronouns",q:"Which sentence is correct?",o:["I love she.","I love her.","I love hers.","I love he."],a:1,why:"An object pronoun comes after a verb. “Love” is the verb, so we use “her”, not “she”."},
{t:"Question forms",q:"Which question is correct?",o:["Are you have a sister?","Does you have a sister?","Do you have a sister?","Is you have a sister?"],a:2,why:"Most simple present questions use do or does. With “you” we use “do”. We do not combine be (are) with the main verb “have”."},
{t:"Giving answers",p:["Rina: Where does your father work?"],q:"Which answer is correct?",o:["He work in Medan.","He works in Medan.","She works in Medan.","He are work in Medan."],a:1,why:"We talk about a father, so we use “he”. In the simple present, the verb takes -s with he, she, and it: “works”."},
{t:"Text structure",q:"A says, “Thank you, Rina. Nice to meet you.” Which part of the dialogue is this?",o:["Opening","Exchange: asking about identity","Exchange: giving information","Closing"],a:3,why:"A dialogue has an opening, an exchange, and a closing. Thanking the other person and ending politely belongs to the closing."},
{t:"Vocabulary and question words",p:["Ms. Sari: And what do your parents do?","Dewi: My father is a bus driver, and my mother is a tailor."],q:"What does Ms. Sari ask about?",o:["Dewi’s parents’ jobs","Dewi’s parents’ ages","Dewi’s parents’ address","Dewi’s parents’ names"],a:0,why:"“What do your parents do?” asks for a job. Dewi answers with the jobs bus driver and tailor."},
{t:"Choosing polite language",q:"You are at the English Club registration desk. You are the club advisor. What is the best polite way to ask for a name?",o:["Hey, who are you?","May I have your name, please?","Tell me your name.","Hi! What’s your name?"],a:1,why:"At a registration, we use a formal and polite form: “May I have your name, please?”. “Hi! What’s your name?” is informal."},
{t:"Protecting privacy",q:"A new online friend asks for your home address and phone number. What is the best answer?",o:["Sure! My address is Jalan Mawar 5.","Here is my phone number.","I will send you my identity card.","Sorry, I’d prefer not to answer that."],a:3,why:"Online, we should not share an address or a phone number with strangers. A polite refusal like “I’d rather not say” protects private information."}
];
var L=["A","B","C","D"],ans=[],cur=0,fresh=0,me={};
var CFG={endpoint:"",pin:"guru123",teacher:""};
var $=function(i){return document.getElementById(i)};
function show(id){["welcome","quiz","result","dash"].forEach(function(s){$(s).classList.toggle("hide",s!==id)});
  var n={welcome:0,quiz:1,result:2}[id],st=$("steps");st.classList.toggle("hide",n===undefined);
  if(n!==undefined)[].forEach.call(st.children,function(el,i){el.className=i===n?"on":(i<n?"dn":"")});
  window.scrollTo({top:0})}
function reset(){ans=Q.map(function(){return null});cur=0;$("warn").textContent=""}
function render(){
  var q=Q[cur],a=ans[cur],done=ans.filter(function(x){return x!==null}).length;
  $("stamps").innerHTML=Q.map(function(x,i){
    var c="st"+(i===cur?" cur":"")+(ans[i]===null?"":(ans[i]===x.a?" ok":" bad"));
    return '<button type="button" class="'+c+'" data-i="'+i+'" aria-label="Question '+(i+1)+'">'+(i+1)+'</button>'}).join("");
  $("fill").style.width=(done/Q.length*100)+"%";
  $("cnt").textContent="Question "+(cur+1)+" of "+Q.length;
  $("tag").textContent=q.t;$("tag").className="chip";
  var p=$("passage");
  if(q.p){p.innerHTML=q.p.map(function(l){return "<div>"+l+"</div>"}).join("");p.classList.remove("hide")}else p.classList.add("hide");
  $("qtext").textContent=q.q;
  $("opts").innerHTML=q.o.map(function(o,i){
    var c="opt";
    if(a!==null){if(i===q.a)c+=" right";else if(i===a)c+=" wrong"}
    return '<button type="button" class="'+c+'" data-o="'+i+'"'+(a!==null?" disabled":"")+'><span class="l">'+L[i]+'</span><span>'+o+'</span></button>'}).join("");
  if(a===null)$("fb").innerHTML="";
  else{var ok=a===q.a;
    $("fb").innerHTML='<div class="fb'+(fresh?" pop":"")+'"><div class="av" aria-hidden="true">'+(ok?"🌟":"💡")+'</div><div class="bub '+(ok?"ok":"no")+'"><strong>'+(ok?"Great job! +10 points":"Not quite. The answer is "+L[q.a]+".")+'</strong><p>'+q.why+'</p></div></div>'}
  $("prev").disabled=cur===0;
  $("next").textContent=cur===Q.length-1?"See my score":"Next";
  $("next").disabled=a===null&&cur!==Q.length-1;
}
function finish(){
  var miss=ans.map(function(x,i){return x===null?i+1:0}).filter(Boolean);
  if(miss.length){$("warn").textContent="Please answer question"+(miss.length>1?"s ":" ")+miss.join(", ")+" first. Tap the numbers above to go there.";return}
  var ok=ans.filter(function(x,i){return x===Q[i].a}).length,sc=ok*10;
  $("score").textContent=0;count(sc);$("nok").textContent=ok;$("nbad").textContent=Q.length-ok;
  var m=sc>=90?["Excellent work! 🎉","You understand this chapter very well. You are ready for Activity 1."]
   :sc>=70?["Good job! 👏","You understand most of the material. Check the questions you missed below, then go to Activity 1."]
   :sc>=50?["Nice try! 💪","You are on the right track. Read the explanations below and review the pronoun tables and the model dialogues."]
   :["Keep going! 🌱","Do not worry. Learning takes time. Read Chapter 1 again and study the explanations below. You will do better in the next activity."];
  $("mh").textContent=m[0];$("mp").textContent=m[1];
  $("review").innerHTML=Q.map(function(q,i){var g=ans[i]===q.a;
    return '<div class="ri '+(g?"ok":"no")+'"><h3>'+(i+1)+". "+q.q+'</h3><p class="a">'+(g?"✅ Your answer: ":"❌ Your answer: ")+L[ans[i]]+". "+q.o[ans[i]]+'</p>'+(g?"":'<p class="a">✔ Correct answer: '+L[q.a]+". "+q.o[q.a]+'</p>')+'<p>'+q.why+'</p></div>'}).join("");
  show("result");
  $("arc").style.strokeDashoffset=465;
  setTimeout(function(){$("arc").style.strokeDashoffset=465*(1-sc/100)},60);me.sc=sc;me.ok=ok;send();if(sc>=70)for(var k=0;k<4;k++)setTimeout(function(){burst($("score"),14)},k*400);
}
function restart(){reset();show("quiz");render()}
function mailOk(){return !!CFG.teacher||/^[^\s@]+@[^\s@]+\.[^\s@]{2,}$/.test($("te").value.trim())}
function chk(){var n=$("nm").value.trim(),c=$("cl").value.trim();$("start").disabled=!(n&&c&&$("dt").value&&mailOk());$("idn").textContent=n||"Your name";$("idc").textContent=c||"Class";$("ph").textContent=n?n[0].toUpperCase():"?";$("ph").classList.remove("bump");void $("ph").offsetWidth;$("ph").classList.add("bump")}
$("nm").oninput=chk;$("cl").oninput=chk;$("dt").oninput=chk;$("te").oninput=chk;
$("start").onclick=function(){
  var n=$("nm").value.trim(),c=$("cl").value.trim().toUpperCase(),k=(n+"|"+c).toLowerCase(),ws=$("ws");ws.textContent="";
  var go=function(){try{var a=JSON.parse(localStorage.getItem("fa1s")||"[]");a.push(k);localStorage.setItem("fa1s",JSON.stringify(a))}catch(e){}me={name:n,cls:c,date:$("dt").value,to:CFG.teacher||$("te").value.trim()};restart()};
  var stop=function(){ws.textContent="This quiz can be taken only once. "+n+" ("+c+") has already started or finished it. Please ask your teacher."};
  var seen=false;try{seen=JSON.parse(localStorage.getItem("fa1s")||"[]").indexOf(k)>-1}catch(e){}
  if(seen){stop();return}
  if(!CFG.endpoint){go();return}
  $("start").disabled=true;
  fetch(CFG.endpoint+"?action=check&name="+encodeURIComponent(n)+"&cls="+encodeURIComponent(c)).then(function(r){return r.json()})
   .then(function(d){$("start").disabled=false;if(d.exists)stop();else go()})
   .catch(function(){$("start").disabled=false;go()})};
$("prev").onclick=function(){if(cur>0){cur--;$("warn").textContent="";render()}};
$("next").onclick=function(){if(cur<Q.length-1){cur++;$("warn").textContent="";render()}else finish()};
$("opts").onclick=function(e){var b=e.target.closest("[data-o]");if(!b||ans[cur]!==null)return;pick(+b.dataset.o)};
$("stamps").onclick=function(e){var b=e.target.closest("[data-i]");if(!b)return;cur=+b.dataset.i;$("warn").textContent="";render()};
document.addEventListener("keydown",function(e){
  if($("quiz").classList.contains("hide")||!$("mo").classList.contains("hide")||e.ctrlKey||e.metaKey||e.altKey)return;
  var k=e.key.toUpperCase(),i=L.indexOf(k);
  if(i>-1&&ans[cur]===null)pick(i)
});
function pick(i){ans[cur]=i;$("warn").textContent="";fresh=1;render();fresh=0;
  var s=document.querySelector(".st.cur");if(s)s.classList.add("pop");
  if(i===Q[cur].a)burst(document.querySelector('[data-o="'+i+'"]'),12)}
function burst(el,n){
  if(!el||matchMedia("(prefers-reduced-motion:reduce)").matches)return;
  var r=el.getBoundingClientRect(),E=["⭐","✨","🎉","💛","🌟"];
  for(var k=0;k<n;k++){var d=document.createElement("span");d.className="cf";d.textContent=E[k%E.length];
    d.style.left=(r.left+r.width/2)+"px";d.style.top=(r.top+r.height/2)+"px";document.body.appendChild(d);
    var a=Math.random()*6.28,v=60+Math.random()*90;
    d.animate([{transform:"translate(0,0) scale(.4)",opacity:1},{transform:"translate("+Math.cos(a)*v+"px,"+(Math.sin(a)*v-50)+"px) scale(1.2) rotate("+(Math.random()*360)+"deg)",opacity:0}],{duration:900,easing:"cubic-bezier(.2,.8,.4,1)"}).onfinish=(function(x){return function(){x.remove()}})(d)}}
function count(to){var t0=performance.now();(function f(t){var p=Math.min((t-t0)/1000,1);$("score").textContent=Math.round(to*p);if(p<1)requestAnimationFrame(f)})(t0)}
function loc(){try{return JSON.parse(localStorage.getItem("fa1")||"[]")}catch(e){return[]}}
function answersText(){return Q.map(function(q,i){return (i+1)+". "+L[ans[i]]+(ans[i]===q.a?" (correct)":" (wrong, correct answer: "+L[q.a]+")")}).join("\n")}
function reportText(){return "Formative Assessment: Identity and Family\nName: "+me.name+"\nClass: "+me.cls+"\nDate: "+me.date+"\nScore: "+me.sc+" / 100 ("+me.ok+" of "+Q.length+" correct)\n\n"+answersText()}
function post(){
  var s=$("sent"),jobs=[],rec=me.rec;$("resend").classList.add("hide");
  if(CFG.endpoint)jobs.push(fetch(CFG.endpoint,{method:"POST",mode:"no-cors",headers:{"Content-Type":"text/plain"},body:JSON.stringify(rec)}));
  if(me.to)jobs.push(fetch("https://formsubmit.co/ajax/"+encodeURIComponent(me.to),{method:"POST",headers:{"Content-Type":"application/json","Accept":"application/json"},
    body:JSON.stringify({_subject:"Quiz result: "+me.name+" ("+me.cls+") "+me.sc+"/100",_template:"table",_captcha:"false",Name:me.name,Class:me.cls,Date:me.date,Score:me.sc+" / 100",Correct:me.ok+" of "+Q.length,Answers:answersText()})})
    .then(function(r){return r.json()}).then(function(d){if(!d||d.success==="false"||d.success===false)throw 0}));
  if(!jobs.length){s.textContent="Result saved on this device.";return}
  s.textContent="Sending your result to the teacher...";
  Promise.all(jobs).then(function(){s.textContent="Result sent to your teacher ✓"})
   .catch(function(){s.textContent="Could not send yet. Tell your teacher, or tap Copy my result.";$("resend").classList.remove("hide")})}
function send(){
  var rec={t:Date.now(),name:me.name,cls:me.cls,date:me.date,score:me.sc,ok:me.ok};me.rec=rec;
  try{var a=loc();a.push(rec);localStorage.setItem("fa1",JSON.stringify(a))}catch(e){}
  post()}
$("resend").onclick=post;
$("copy").onclick=function(){
  var t=reportText(),b=$("copy");
  var done=function(){b.textContent="Copied ✓";setTimeout(function(){b.textContent="Copy my result"},2000)};
  var fall=function(){var x=document.createElement("textarea");x.value=t;x.style.cssText="position:fixed;opacity:0";document.body.appendChild(x);x.select();try{document.execCommand("copy");done()}catch(e){}x.remove()};
  if(navigator.clipboard&&navigator.clipboard.writeText)navigator.clipboard.writeText(t).then(done,fall);else fall()};
$("refbtn").onclick=function(){$("mo").classList.remove("hide");$("mx").focus()};
$("mx").onclick=function(){$("mo").classList.add("hide");$("refbtn").focus()};
$("mo").onclick=function(e){if(e.target===$("mo"))$("mx").click()};
document.addEventListener("keydown",function(e){if(e.key==="Escape"&&!$("mo").classList.contains("hide"))$("mx").click()});
var DR=[];
function dview(){
  var g={};DR.forEach(function(r){var k=(r.name+"|"+r.cls).toLowerCase(),o=g[k];
    if(!o)g[k]={name:r.name,cls:r.cls,best:+r.score,n:1,t:+r.t};else{o.n++;if(+r.score>o.best){o.best=+r.score;o.t=+r.t}}});
  var f=$("cf").value,a=Object.keys(g).map(function(k){return g[k]}).filter(function(o){return !f||o.cls===f});
  a.sort(function(x,y){return y.best-x.best||x.t-y.t});
  $("rows").innerHTML=a.length?a.map(function(o,i){var m=["🥇","🥈","🥉"][i]||(i+1);
    return "<tr><td>"+m+"</td><td>"+esc(o.name)+"</td><td>"+esc(o.cls)+"</td><td><b>"+o.best+"</b></td><td>"+o.n+"</td></tr>"}).join(""):'<tr><td colspan="5">No results yet.</td></tr>';
  var av=a.length?Math.round(a.reduce(function(s,o){return s+o.best},0)/a.length):0;
  $("dsum").textContent=a.length+" students · class average (best scores): "+av+(CFG.endpoint?"":" · Local mode: only results from this device")}
function esc(x){return String(x).replace(/[&<>"]/g,function(c){return{"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;"}[c]})}
function dload(){
  $("dw").textContent="";
  var done=function(rows){DR=rows;var cs=[];rows.forEach(function(r){if(cs.indexOf(r.cls)<0)cs.push(r.cls)});cs.sort();
    var v=$("cf").value;$("cf").innerHTML='<option value="">All classes</option>'+cs.map(function(c){return'<option>'+esc(c)+'</option>'}).join("");$("cf").value=v;
    $("lock").classList.add("hide");$("dbody").classList.remove("hide");dview()};
  if(!CFG.endpoint){if($("pin").value!==CFG.pin){$("dw").textContent="Wrong PIN.";return}done(loc());return}
  $("dw").textContent="Loading...";
  fetch(CFG.endpoint+"?action=list&pin="+encodeURIComponent($("pin").value)).then(function(r){return r.json()})
   .then(function(d){if(d.error){$("dw").textContent="Wrong PIN.";return}$("dw").textContent="";done(d.rows||[])})
   .catch(function(){$("dw").textContent="Could not load the data. Check the endpoint link."})}
$("tlink").onclick=function(){$("lock").classList.remove("hide");$("dbody").classList.add("hide");$("pin").value="";$("dw").textContent="";show("dash")};
$("unlock").onclick=dload;$("rf").onclick=dload;$("cf").onchange=dview;
$("pin").onkeydown=function(e){if(e.key==="Enter")dload()};
$("back").onclick=function(){show("welcome")};
$("csv").onclick=function(){var c="Name,Class,Score,Correct,Time\n"+DR.map(function(r){return[r.name,r.cls,r.score,r.ok,new Date(+r.t).toLocaleString()].map(function(x){return'"'+String(x).replace(/"/g,'""')+'"'}).join(",")}).join("\n");
  var a=document.createElement("a");a.href=URL.createObjectURL(new Blob([c],{type:"text/csv"}));a.download="quiz-results.csv";a.click()};
(function(){
  var d=new Date(),p=function(x){return String(x).padStart(2,"0")},to="";
  $("dt").value=d.getFullYear()+"-"+p(d.getMonth()+1)+"-"+p(d.getDate());
  try{to=new URLSearchParams(location.search).get("to")||""}catch(e){}
  if(CFG.teacher)$("tew").classList.add("hide");
  else if(/^[^\s@]+@[^\s@]+\.[^\s@]{2,}$/.test(to)){$("te").value=to;$("te").readOnly=true}
  show("welcome");chk()})();
reset();
</script>
</body>
</html>
