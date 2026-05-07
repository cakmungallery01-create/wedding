<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
-webkit-tap-highlight-color:transparent;
}

html,body{
margin:0;
padding:0;
width:100%;
height:100%;
overflow:hidden;
background:#000;
font-family:'Poppins',sans-serif;
}

body{
position:fixed;
inset:0;
}

/* OPENING */

#opening{
position:fixed;
inset:0;
z-index:999999;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
padding:30px;
color:white;

background:
linear-gradient(rgba(0,0,0,.55),rgba(0,0,0,.55)),
url('https://images.unsplash.com/photo-1519741497674-611481863552?q=80&w=1200&auto=format&fit=crop');

background-size:cover;
background-position:center;

transition:1s;
}

#opening.hide{
opacity:0;
pointer-events:none;
}

#opening h1{
font-size:42px;
font-weight:700;
margin-bottom:10px;
}

#opening p{
font-size:15px;
opacity:.9;
}

#openBtn{
margin-top:28px;
padding:15px 34px;
border:none;
border-radius:999px;
background:white;
color:black;
font-size:15px;
font-weight:600;
cursor:pointer;
transition:.2s;
}

#openBtn:active{
transform:scale(.95);
}

/* PHONE */

.phone{
position:fixed;
inset:0;

width:100vw;
height:100dvh;

background:#000;

overflow:hidden;

display:none;

z-index:99999;
}

/* DYNAMIC ISLAND */

.phone::before{
content:'';
position:absolute;
top:12px;
left:50%;
transform:translateX(-50%);
width:126px;
height:34px;
border-radius:40px;
background:#000;
z-index:999;
}

/* HEADER */

.header{
position:absolute;
top:0;
left:0;
right:0;

z-index:5;

height:95px;
padding:14px 16px 10px;

background:rgba(20,20,20,.88);
backdrop-filter:blur(25px);

border-bottom:1px solid rgba(255,255,255,.06);

color:white;
}

.topbar{
display:flex;
justify-content:space-between;
align-items:center;
font-size:13px;
font-weight:600;
padding:0 4px;
margin-bottom:14px;
}

.icons{
font-size:12px;
opacity:.9;
}

.header-content{
display:flex;
align-items:center;
}

.profile{
width:42px;
height:42px;
border-radius:50%;
background:#2c2c2e;

display:flex;
justify-content:center;
align-items:center;

font-size:20px;
margin-right:12px;
}

.name{
font-size:16px;
font-weight:600;
}

.status{
font-size:12px;
color:#aaa;
}

/* CHAT AREA */

.chat-area{
position:absolute;
top:95px;
left:0;
right:0;
bottom:0;

overflow-y:auto;

padding:18px 12px 120px;

scroll-behavior:smooth;

background:
linear-gradient(rgba(0,0,0,.45),rgba(0,0,0,.45)),
url('https://images.unsplash.com/photo-1516589091380-5d8e87df6999?q=80&w=1200&auto=format&fit=crop');

background-size:cover;
background-position:center;
}

.chat-area::-webkit-scrollbar{
display:none;
}

/* MESSAGE */

.message{
display:none;
max-width:78%;

padding:10px 14px 6px;

margin-bottom:8px;

font-size:15px;
line-height:1.45;

animation:show .35s ease;
}

.sent{
margin-left:auto;

background:#0A84FF;
color:white;

border-radius:22px 22px 6px 22px;

box-shadow:0 3px 12px rgba(10,132,255,.25);
}

.received{
background:#2c2c2e;
color:white;

border-radius:22px 22px 22px 6px;
}

.message-time{
font-size:10px;
opacity:.72;
margin-top:4px;
text-align:right;
}

/* TYPING */

.typing{
display:none;

background:#2c2c2e;

width:74px;

padding:10px 14px;

border-radius:20px;

margin-bottom:10px;

animation:show .3s ease;
}

.dot{
width:7px;
height:7px;

background:#aaa;

border-radius:50%;

display:inline-block;

margin-right:3px;

animation:blink 1.2s infinite;
}

.dot:nth-child(2){
animation-delay:.2s;
}

.dot:nth-child(3){
animation-delay:.4s;
}

@keyframes blink{

0%{
opacity:.25;
transform:translateY(0);
}

50%{
opacity:1;
transform:translateY(-2px);
}

100%{
opacity:.25;
transform:translateY(0);
}

}

@keyframes show{

from{
opacity:0;
transform:translateY(10px);
}

to{
opacity:1;
transform:translateY(0);
}

}

/* INVITATION */

.invitation{
display:none;

background:rgba(255,255,255,.97);

backdrop-filter:blur(30px);

padding:32px 28px;

border-radius:34px;

text-align:center;

margin-top:26px;

animation:show .8s ease;

box-shadow:0 15px 40px rgba(0,0,0,.35);
}

.invitation h1{
font-size:32px;
margin-bottom:12px;
color:#111;
}

.invitation p{
font-size:15px;
line-height:1.8;
color:#333;
}

.button{
display:inline-block;

margin-top:20px;

padding:14px 24px;

border-radius:999px;

background:#111;
color:white;

text-decoration:none;

font-size:14px;
font-weight:600;
}

.fade{
margin-top:16px;
font-size:13px;
opacity:.7;
font-style:italic;
}

</style>
