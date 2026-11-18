<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>SIM Gacha — телефоны, симки и авто-кейсы</title>
<style>
:root{--bg:#f4f5f8;--card:#fff;--tx:#161a24;--mut:#6b7385;--bd:#dfe3ec;--ac:#4f46e5}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#0f1117;--card:#1a1d27;--tx:#eef0f6;--mut:#8b93a7;--bd:#2c3140;--ac:#818cf8}}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--tx);font-family:system-ui,-apple-system,"Segoe UI",Roboto,sans-serif;max-width:720px;margin:0 auto;padding:14px;padding-top:calc(14px + env(safe-area-inset-top,0px));padding-bottom:calc(14px + env(safe-area-inset-bottom,0px))}
h1{font-size:20px;margin:4px 0 12px}
.bal{display:flex;justify-content:space-between;align-items:center;background:var(--card);border:1px solid var(--bd);border-radius:14px;padding:12px 14px;margin-bottom:12px}
.bal b{font-size:22px}.bal small{color:var(--mut);display:block}
button{font:inherit;cursor:pointer;border:0;border-radius:12px;padding:12px 14px;background:var(--ac);color:#fff;font-weight:600}
button.sec{background:transparent;color:var(--tx);border:1px solid var(--bd)}
button:disabled{opacity:.45;cursor:not-allowed}
.tabs{display:flex;gap:8px;margin-bottom:10px}
.tabs button{flex:1;background:var(--card);color:var(--tx);border:1px solid var(--bd)}
.tabs .on{background:var(--ac);color:#fff;border-color:var(--ac)}
.cases{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:12px}
.case{background:var(--card);border:1px solid var(--bd);border-radius:14px;padding:12px;display:flex;flex-direction:column;gap:8px}
.case h2{margin:0;font-size:16px}.case p{margin:0;color:var(--mut);font-size:12px;line-height:1.4;flex:1}
.btns{display:flex;flex-direction:column;gap:6px}.btns button{padding:10px 6px;font-size:13px}
.stage{background:var(--card);border:1px solid var(--bd);border-radius:14px;padding:14px;min-height:150px;display:flex;flex-direction:column;align-items:center;justify-content:center;margin-bottom:12px}
.sim{width:100%;max-width:340px;border-radius:14px;padding:14px;color:#fff;position:relative;border:2px solid rgba(255,255,255,.35);text-shadow:0 1px 2px rgba(0,0,0,.35)}
.sim .op{font-weight:700;font-size:14px;opacity:.95}
.sim .num{font-size:21px;font-weight:700;margin:10px 0 8px;letter-spacing:.5px;font-variant-numeric:tabular-nums}
.sim .row{display:flex;justify-content:space-between;font-size:13px}
.sim .chip{position:absolute;right:12px;top:12px;width:30px;height:22px;border-radius:5px;background:linear-gradient(135deg,#f5d77a,#c9a227)}
.plate{background:#fff;color:#111;border:2px solid #111;border-radius:6px;display:flex;align-items:center;justify-content:space-between;padding:4px 10px;margin:10px 0 8px;font-size:26px;font-weight:700;text-shadow:none}
.plate em{font-style:normal;font-size:20px;border-left:2px solid #111;padding-left:8px}
.slotbox{display:flex;align-items:center;justify-content:center;font-size:22px;font-weight:700;color:#fff;padding:14px 12px;border-radius:14px;background:linear-gradient(135deg,#222,#4a4f60);max-width:100%}
.slotbox.pl{background:#fff;color:#111;border:3px solid #111;font-size:28px}
.sl{display:inline-block;height:34px;overflow:hidden;width:17px}.sl.lt{width:22px}
.col{display:flex;flex-direction:column;will-change:transform}
.col i{font-style:normal;height:34px;line-height:34px;text-align:center;flex:0 0 34px}
.st{height:34px;line-height:34px;padding:0 1px}
.pop{animation:pop .55s cubic-bezier(.2,1.6,.4,1)}
@keyframes pop{0%{transform:scale(.3) rotate(-8deg);opacity:0}100%{transform:scale(1) rotate(0);opacity:1}}
.glow{box-shadow:0 0 30px var(--g)}
.car{width:100%;max-width:340px;border-radius:14px}.car svg{width:100%;height:auto;display:block;border-radius:14px}
.car .cap{display:flex;justify-content:space-between;padding:8px 2px 0;font-weight:700;font-size:14px}
.reel{position:relative;width:100%;overflow:hidden;border-radius:12px;height:110px;background:rgba(0,0,0,.08)}
.reel::after{content:"";position:absolute;left:50%;top:0;bottom:0;width:3px;background:#fff;box-shadow:0 0 8px #000;transform:translateX(-50%);z-index:2}
.track{display:flex;gap:8px;position:absolute;left:0;top:0;will-change:transform}
.rc{flex:0 0 120px;height:110px;border-radius:10px;color:#fff;text-shadow:0 1px 2px rgba(0,0,0,.4);padding:8px;font-size:12px;font-weight:700;display:flex;flex-direction:column;justify-content:flex-end}
.multi{display:grid;grid-template-columns:repeat(auto-fill,minmax(140px,1fr));gap:8px;width:100%;margin-top:10px}
.hint{color:var(--mut)}
.tools{display:flex;gap:8px;flex-wrap:wrap;margin-bottom:10px;align-items:center}.tools h2{margin:0;font-size:16px;flex:1}
.inv{display:grid;grid-template-columns:repeat(auto-fill,minmax(150px,1fr));gap:8px}
.mini{border-radius:12px;padding:10px;color:#fff;text-shadow:0 1px 2px rgba(0,0,0,.35);font-size:12px;display:flex;flex-direction:column;gap:3px}
.mini b{font-size:13px;font-variant-numeric:tabular-nums}
.mini button{margin-top:6px;padding:6px;font-size:12px;background:rgba(0,0,0,.35)}
.table{background:var(--card);border:1px solid var(--bd);border-radius:14px;padding:6px 12px;margin-top:12px;font-size:12px;overflow-x:auto}
.table div{display:flex;justify-content:space-between;gap:10px;padding:5px 0;border-bottom:1px solid var(--bd);white-space:nowrap}.table div:last-child{border:0}
.dot{display:inline-block;width:9px;height:9px;border-radius:50%;margin-right:6px}
.stats{color:var(--mut);font-size:12px;margin:8px 0}
.tabs button{padding:10px 4px;font-size:13px}
.ov{position:fixed;inset:0;background:rgba(0,0,0,.65);z-index:50;display:none;overflow:auto;padding:calc(10px + env(safe-area-inset-top,0px)) 10px calc(10px + env(safe-area-inset-bottom,0px))}
.ov.show{display:block}
.pbox{max-width:420px;margin:0 auto;background:var(--card);border:1px solid var(--bd);border-radius:16px;padding:12px}
.phead{display:flex;justify-content:space-between;align-items:center;gap:8px;margin-bottom:10px}
.phwrap{position:relative;width:226px;margin:6px auto 12px}
.ph{width:226px;height:420px;border-radius:32px;border:7px solid #222;background:#000;position:relative;overflow:hidden;box-shadow:0 8px 30px rgba(0,0,0,.4)}
.scr{position:absolute;inset:0;color:#fff;display:flex;flex-direction:column;overflow:hidden;font-size:12px}
.notch{position:absolute;top:6px;left:50%;width:60px;height:12px;background:#000;border-radius:8px;transform:translateX(-50%);z-index:3}
.sbar{display:flex;justify-content:space-between;font-size:10px;padding:8px 16px 2px;z-index:2}
.home{flex:1;display:flex;flex-direction:column;padding:6px 12px;background:linear-gradient(160deg,var(--w1),#111);animation:fade .6s}
.clock{font-size:42px;font-weight:300;text-align:center;margin:18px 0 24px}
.apps{display:grid;grid-template-columns:repeat(4,1fr);gap:8px}
.app{display:flex;flex-direction:column;align-items:center;font-size:9px;gap:3px;background:none;padding:0;color:#fff;border-radius:0}
.app b{display:block;width:40px;height:40px;border-radius:11px;background:rgba(255,255,255,.2);font-size:22px;line-height:40px;text-align:center}
.boot{flex:1;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:18px;animation:wake .6s}
.boot .lg{font-size:18px;font-weight:700;animation:pulse 1.6s infinite;text-align:center;padding:0 10px}
.bar{width:110px;height:4px;border-radius:2px;background:#333;overflow:hidden}.bar i{display:block;height:100%;width:0;background:#fff;animation:fill 2.4s linear forwards}
@keyframes fill{to{width:100%}}@keyframes pulse{50%{opacity:.35}}@keyframes wake{from{filter:brightness(5)}to{filter:none}}@keyframes fade{from{opacity:0;transform:scale(1.06)}}
.off{flex:1;display:flex;align-items:center;justify-content:center;color:#333}
.tray{position:absolute;right:-2px;top:96px;width:9px;height:42px;border-radius:3px;background:#555;z-index:4}.tray.full{background:#2fbf71}
.simfly{position:absolute;right:-80px;top:97px;width:62px;height:40px;border-radius:6px;z-index:5;border:2px solid rgba(255,255,255,.5);animation:simin 1.5s ease-in-out forwards}
.simfly::before{content:"";position:absolute;left:6px;top:8px;width:16px;height:12px;border-radius:2px;background:#e8c64a}
@keyframes simin{0%{transform:translateX(0) rotate(-8deg)}70%{transform:translateX(-72px) rotate(0)}100%{transform:translateX(-80px);opacity:0}}
.capp{flex:1;overflow:auto;padding:6px 8px;background:#0f1117;animation:fade .4s}
.capp button{font-size:12px;padding:8px;width:100%;margin-top:6px}
.cr{display:flex;justify-content:space-between;gap:6px;align-items:center;padding:7px 8px;border-radius:9px;background:#1b1f2c;margin-top:5px;cursor:pointer}
.cr small{color:#9aa3b8}
.drop{display:flex;justify-content:space-between;gap:6px;font-size:10px;padding:3px 0;border-bottom:1px solid #2a2f40}
.capp .reel,.capp .rc{height:80px}.capp .rc{font-size:10px;padding:5px}
.sims{display:flex;flex-direction:column;gap:6px;max-height:170px;overflow:auto;margin-top:6px}.sims button{padding:8px;font-size:12px;text-align:left}
.simline{font-size:12px;margin:6px 0}
</style>
</head>
<body>
<h1>📱 SIM Gacha</h1>
<div class="bal"><div><small>Баланс</small><b id="bal"></b></div><button class="sec" id="reset" style="display:none">Начать заново</button></div>
<div class="tabs"><button class="tab" data-m="sim">📱 Симки</button><button class="tab" data-m="plate">🚗 Номера</button><button class="tab" data-m="phone">📞 Телефоны</button></div>
<div class="cases" id="cases"></div>
<div class="stage" id="stage"><span class="hint">Выбери крутку или кейс</span></div>
<div class="stats" id="stats"></div>
<div class="tools"><h2>Коллекция (<span id="cnt">0</span>)</h2><button class="sec" id="sellLow">Продать дешёвые</button><button class="sec" id="sellAll">Продать всё</button></div>
<div class="inv" id="inv"></div>
<div class="table" id="tbl"></div>
<div class="ov" id="ov"><div class="pbox" id="pbox"></div></div>

<script>
const OPS={
 'МТС':{c:'#e30611',p:[910,911,912,913,914,915,916,917,918,919,980,981,982,983,984,985,986,987,988,989]},
 'МегаФон':{c:'#00a651',p:[920,921,922,923,924,925,926,927,928,929,930,931,932,933,934,936,937,938,939]},
 'Билайн':{c:'#d99a00',p:[903,905,906,909,960,961,962,963,964,965,966,967,968,969]},
 'Т-Мобайл':{c:'#e6007e',p:[933,994,995]},
 'Йота':{c:'#1a7cf0',p:[999,958,991,992,995,996]},
 'Ростелеком':{c:'#7b2fd0',p:[901,902,912,930,931,939,958,970,971,991,992,993]}
};
const R=[
 {n:'Обычный',ch:50,a:500,b:1500,c:'#8a8f98'},
 {n:'Необычный',ch:25,a:3000,b:8000,c:'#3fae5a'},
 {n:'Редкий',ch:12,a:15000,b:40000,c:'#2f86e0'},
 {n:'Эпический',ch:7,a:7000,b:20000,c:'#9b45e0'},
 {n:'Легендарный',ch:3.5,a:35000,b:100000,c:'#f08a00'},
 {n:'Мифический',ch:1.8,a:150000,b:500000,c:'#e0334f'},
 {n:'Секретный',ch:.5,a:6e5,b:2e6,c:'#16a3a3'},
 {n:'Бесконечный',ch:.15,a:3e6,b:10e6,c:'#4a4fe0'},
 {n:'Божественный',ch:.04,a:12e6,b:45e6,c:'#c9a227'},
 {n:'Невозможный',ch:.01,a:60e6,b:200e6,c:'#111'},
 {n:'Автомобиль',ch:0,a:5e8,b:5e8,c:'#0b3d91'}
];
const LET='АВЕКМНОРСТУХ',DIG='0123456789';
const PH={
3:['iPhone 11','iPhone 12','Samsung Galaxy A12','Samsung Galaxy A32','Samsung Galaxy A51','Samsung Galaxy A52','Xiaomi Redmi 9A','Xiaomi Redmi Note 10S','Xiaomi Redmi Note 11','Xiaomi Redmi Note 12','POCO M3','POCO M4 Pro','POCO M5','Honor 7A','Honor 8X','Honor 9 Lite','Honor 10i','Huawei P20 Lite','Realme C11','Realme C21','Realme 6 Pro','Realme 8','Tecno Spark 6 Go','Tecno Pova 2','Tecno Pova 4','Infinix Hot 10 Play','Infinix Note 8','Infinix Hot 12','Vivo Y11','Vivo Y31','Oppo A52','Oppo Reno 4 Lite'],
4:['iPhone 13','iPhone 14','Samsung Galaxy A54','Samsung Galaxy S22','Xiaomi Redmi Note 13','POCO X3 Pro','POCO X4 Pro','POCO X5 Pro','Honor 20','Honor 50','Honor 70','Honor 90','Huawei P30 Pro','Huawei Nova 10','Huawei Nova 11','Realme 9 Pro','Realme 10','Realme 11 Pro','Tecno Spark 10 Pro','Tecno Camon 20','Infinix Note 30','Infinix GT 10 Pro','Vivo V25','Vivo V27','Oppo Reno 7','Oppo Reno 8'],
5:['iPhone 15','iPhone 15 Pro','iPhone 16','Samsung Galaxy S23','Samsung Galaxy S24','POCO X6 Pro']};
const CN=['Lada Granta','Lada Vesta','Kia Rio','Hyundai Solaris','Toyota Camry','Mazda 6','BMW 3 Series','Audi A6','Mercedes E-Class','BMW M5','Porsche Macan','Range Rover Sport','Mercedes G63 AMG','Porsche 911 Turbo S','Lamborghini Urus','Ferrari 488','McLaren 720S','Rolls-Royce Cullinan','Lamborghini Aventador','Ferrari LaFerrari','Koenigsegg Jesko','Pagani Huayra','Bugatti W16 Mistral','Bugatti La Voiture Noire'];
const CARS=CN.map((n,i)=>({n,h:(i*37)%360,p:i==22?5e8:+(40000*Math.pow(20000,i/23)).toPrecision(2)}));CARS[22].h=220;
const CASEN=['Первая машина','Городской','Семейный','Таксист','Автолюбитель','Тюнинг','Бизнес','Гараж','Премиум','Люкс','Внедорожник','Спорткар','Дрифт','Гоночный','Суперкар','Гиперкар','Коллекционный','Миллиардер','Королевский','Легенда'];
const CC=CASEN.map((t,k)=>({t,cost:+(100000*Math.pow(2000,k/19)).toPrecision(2),ids:[k,k+1,k+2,k+3,k+4],w:[40,32,18,8,2]}));
const W1=Object.fromEntries(R.map((r,i)=>[i,r.ch]).filter(x=>x[1]>0));
const M={
 sim:{cases:[
  {t:'Крутка симок',d:'Шансы от Обычного (50%) до Невозможного (0.01%)',cost:3000,w:W1,reel:false},
  {t:'Кейс «Рулетка»',d:'Обычный 50% · Редкий 49.9% · Невозможный 0.09%',cost:100000,w:{0:50,2:49.9,9:.09},reel:true}]},
 plate:{cases:[
  {t:'Крутка номеров',d:'Российские номера. Шансы от Обычного (50%) до Невозможного (0.01%)',cost:3000,w:W1,reel:false},
  {t:'Кейс «Номера»',d:'Редкий 50% · Эпический 49.7% · Невозможный 0.2% · 🏎️ Bugatti 0.1%',cost:100000,w:{2:50,3:49.7,9:.2,10:.1},reel:true}]},
 phone:{cases:[
  {t:'Кейс «Телефоны»',d:'Эпический 7% · Легендарный 3.5% · Мифический 1.8%. Вставь SIM — продаётся дороже на стоимость симки. Включи телефон — открой приложение с авто-кейсами',cost:75000,w:{3:7,4:3.5,5:1.8},reel:true}]}
};
let S={bal:20000,inv:[],spins:0,best:0,id:1};
try{const d=JSON.parse(localStorage.getItem('simgacha')||'null');if(d&&typeof d.bal==='number')S=d}catch(e){}
S.inv.forEach(s=>{s.kind=s.car?'car':(s.kind||'sim');if(s.kind==='car'&&!s.name){s.name='Bugatti W16 Mistral';s.h=220}});
let mode='sim',busy=false,sellArm=0;
function save(){try{localStorage.setItem('simgacha',JSON.stringify(S))}catch(e){}}
const $=id=>document.getElementById(id);
const rub=n=>Math.round(n).toLocaleString('ru-RU')+' ₽';
const rnd=(a,b)=>Math.floor(a+Math.random()*(b-a+1));
function pick(w){const e=Object.entries(w),t=e.reduce((s,x)=>s+x[1],0);let r=Math.random()*t;for(const [i,v] of e){if((r-=v)<0)return +i}return +e[e.length-1][0]}
function genSim(ri){
 const names=Object.keys(OPS),op=names[rnd(0,names.length-1)],pf=OPS[op].p[rnd(0,OPS[op].p.length-1)];
 const t=String(rnd(0,9999999)).padStart(7,'0');
 return {id:S.id++,kind:'sim',op,num:`+7 (${pf}) ${t.slice(0,3)}-${t.slice(3,5)}-${t.slice(5)}`,r:ri,price:rnd(R[ri].a,R[ri].b)};
}
function genPlate(ri){
 const x=rnd(1,9),y=rnd(0,9),l=LET[rnd(0,11)],L3=()=>LET[rnd(0,11)];
 let d;
 if(ri<=1)d=String(rnd(1,999)).padStart(3,'0');
 else if(ri==2)d=`${x}${y}${x}`;
 else if(ri==3)d=`${x}${x}${y}`;
 else if(ri==4||ri==5||ri==7)d=`${x}${x}${x}`;
 else if(ri==6)d='00'+rnd(1,9);
 else d=ri==8?'777':'001';
 const ls=ri>=5?[l,l,l]:[L3(),L3(),L3()];
 const lo=['02','16','23','34','50','52','54','59','61','63','66','72','74','76','116','136','150','161','163','174'];
 const hi=['77','78','99','97','98','177','178','197','199','777','799'];
 const reg=(ri<=4?lo:hi)[rnd(0,(ri<=4?lo:hi).length-1)];
 return {id:S.id++,kind:'plate',num:ls[0]+d+ls[1]+ls[2],reg,r:ri,price:rnd(R[ri].a,R[ri].b)};
}
function genCar(i){const q=CARS[i];return {id:S.id++,kind:'car',car:1,op:'Авто',name:q.n,num:q.n,r:10,h:q.h,price:q.p}}
function genPhone(ri){const l=PH[ri];return {id:S.id++,kind:'phone',name:l[rnd(0,l.length-1)],r:ri,price:rnd(R[ri].a,R[ri].b),sim:null}}
function genItem(ri){
 if(ri===10)return genCar(22);
 if(mode==='phone')return genPhone(ri);
 return (mode==='plate'?genPlate:genSim)(ri);
}
const col=s=>s.kind==='sim'?OPS[s.op].c:s.kind==='car'?'#0b3d91':s.kind==='phone'?'#2a3350':'#3a3f4d';
const lab=s=>s.kind==='sim'?s.op:s.kind==='car'?'Авто':s.kind==='phone'?'Телефон':'Номер';
const txt=s=>s.kind==='plate'?s.num+' '+s.reg:s.kind==='car'?'🏎️ '+s.name:s.kind==='phone'?s.name:s.num;
const val=s=>s.price+(s.sim?s.sim.price:0);

function playReel(el,rt,win,tw,cb){
 const N=40,WIN=34;let h='';
 for(let k=0;k<N;k++){const x=k===WIN?win:rt();h+=`<div class="rc" style="width:${tw}px;flex:0 0 ${tw}px;background:linear-gradient(160deg,${x.c},#000a)">${x.t}</div>`}
 el.innerHTML=`<div class="reel"><div class="track">${h}</div></div>`;
 const trk=el.querySelector('.track'),w=el.querySelector('.reel').clientWidth;
 trk.getBoundingClientRect();
 trk.style.transition='transform 4.5s cubic-bezier(.12,.6,.1,1)';
 trk.style.transform=`translateX(${-(WIN*(tw+8)+tw/2-w/2+rnd(-tw/3,tw/3))}px)`;
 setTimeout(cb,4700);
}

function carHTML(s){
 const h=s.h==null?220:s.h,nm=s.name||'Bugatti W16 Mistral';
 return `<div class="car pop glow" style="--g:hsl(${h},80%,55%)"><svg viewBox="0 0 300 150" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="cbg" x1="0" y1="0" x2="0" y2="1"><stop offset="0" stop-color="#0d1b3d"/><stop offset="1" stop-color="#1d3a7a"/></linearGradient><linearGradient id="cb" x1="0" y1="0" x2="0" y2="1"><stop offset="0" stop-color="hsl(${h},75%,55%)"/><stop offset="1" stop-color="hsl(${h},80%,22%)"/></linearGradient></defs><rect width="300" height="150" fill="url(#cbg)"/><ellipse cx="155" cy="128" rx="125" ry="9" fill="#000" opacity=".45"/><path d="M28 104 C26 94 38 88 62 85 L100 72 C118 62 150 59 176 62 C200 65 214 72 230 82 L262 88 C276 91 282 97 282 104 L282 110 L28 110 Z" fill="url(#cb)"/><rect x="28" y="102" width="254" height="8" fill="#0a0f1c"/><path d="M104 72 L128 62 L146 64 L136 77 Z" fill="#bcd9ff" opacity=".85"/><path d="M136 77 L146 64 C170 62 190 66 205 76 Z" fill="#05070d"/><path d="M150 66 C165 54 195 56 208 70 L192 72 Z" fill="#0a2a66"/><path d="M92 100 C130 80 180 80 222 98" fill="none" stroke="#dfe8f5" stroke-width="3"/><path d="M28 98 C26 92 32 90 36 94 L38 104 L28 104 Z" fill="#1a1a1a"/><rect x="40" y="90" width="14" height="4" rx="2" fill="#fff"/><circle cx="82" cy="108" r="20" fill="#0a0a0a"/><circle cx="82" cy="108" r="12" fill="#c9ced6"/><circle cx="82" cy="108" r="4" fill="#333"/><circle cx="236" cy="108" r="20" fill="#0a0a0a"/><circle cx="236" cy="108" r="12" fill="#c9ced6"/><circle cx="236" cy="108" r="4" fill="#333"/><text x="150" y="145" text-anchor="middle" font-size="11" font-weight="700" fill="#cfe0ff" font-family="sans-serif">${nm.toUpperCase()}</text></svg><div class="cap"><span>🏎️ ${nm}</span><span>${rub(s.price)}</span></div></div>`;
}
function itemHTML(s){
 if(s.kind==='car')return carHTML(s);
 if(s.kind==='phone')return `<div class="sim pop glow" style="--g:${R[s.r].c};background:linear-gradient(135deg,#2a3350,${R[s.r].c})"><div class="op">📱 Телефон · ${R[s.r].n}</div><div class="num">${s.name}</div><div class="row"><span>Цена</span><b>${rub(val(s))}</b></div></div>`;
 const r=R[s.r];
 const mid=s.kind==='plate'?`<div class="plate"><span>${s.num}</span><em>${s.reg}</em></div>`:`<div class="num">${s.num}</div>`;
 return `<div class="sim pop glow" style="--g:${r.c};background:linear-gradient(135deg,${col(s)},${r.c})">${s.kind==='sim'?'<div class="chip"></div>':''}<div class="op">${s.kind==='plate'?'Номер на авто':s.op}</div>${mid}<div class="row"><span>${r.n}</span><b>${rub(s.price)}</b></div></div>`;
}
const mini=(s,b)=>`<div class="mini" style="background:linear-gradient(135deg,${col(s)},${R[s.r].c})"><span>${lab(s)} · ${R[s.r].n}</span><b>${txt(s)}</b><span>${rub(val(s))}${s.sim?' · 📶 с SIM':''}</span>${b?`${s.kind==='phone'?`<button data-open="${s.id}">📱 Открыть</button>`:''}<button data-id="${s.id}">Продать</button>`:''}</div>`;

function runSlots(st,s,done){
 const toks=[];
 if(s.kind==='plate'){
  [...s.num].forEach(ch=>toks.push({c:ch,sp:1,p:/\d/.test(ch)?DIG:LET}));
  toks.push({c:' ',sp:0});
  [...s.reg].forEach(ch=>toks.push({c:ch,sp:1,p:DIG}));
 }else{
  [...s.num].forEach((ch,i)=>toks.push({c:ch,sp:i>1&&/\d/.test(ch),p:DIG}));
 }
 let maxT=0;
 const html=toks.map((t,i)=>{
  if(!t.sp)return `<span class="st">${t.c===' '?'&nbsp;':t.c}</span>`;
  const n=14+i;let cells='';
  for(let k=0;k<n-1;k++)cells+=`<i>${t.p[rnd(0,t.p.length-1)]}</i>`;
  cells+=`<i>${t.c}</i>`;
  const d=(0.9+i*0.14).toFixed(2);maxT=Math.max(maxT,+d);
  return `<span class="sl ${t.p===LET?'lt':''}"><b class="col" data-n="${n}" data-d="${d}">${cells}</b></span>`;
 }).join('');
 st.innerHTML=`<div class="slotbox ${s.kind==='plate'?'pl':''}">${html}</div><div class="hint" style="margin-top:10px">Крутим…</div>`;
 requestAnimationFrame(()=>requestAnimationFrame(()=>{
  st.querySelectorAll('.col').forEach(c=>{c.style.transition=`transform ${c.dataset.d}s cubic-bezier(.15,.7,.2,1)`;c.style.transform=`translateY(${-(c.dataset.n-1)*34}px)`});
 }));
 setTimeout(done,maxT*1000+300);
}
function showResult(items){
 const st=$('stage');
 if(items.length===1){st.innerHTML=itemHTML(items[0]);return}
 const tot=items.reduce((a,s)=>a+s.price,0);
 st.innerHTML=`<div class="hint">Выпало ${items.length} шт. на ${rub(tot)}</div><div class="multi">`+items.slice().sort((a,b)=>b.price-a.price).map(s=>mini(s,false)).join('')+'</div>';
}
function finish(items){
 for(const s of items){S.inv.unshift(s);if(s.price>S.best)S.best=s.price}
 busy=false;save();render();
}
function roll(i,n){
 const c=M[mode].cases[i];
 if(busy||S.bal<c.cost*n)return;
 busy=true;S.bal-=c.cost*n;S.spins+=n;render();
 const items=Array.from({length:n},()=>genItem(pick(c.w)));
 const win=items.reduce((a,s)=>s.price>a.price?s:a),st=$('stage');
 const end=()=>{showResult(items);finish(items)};
 if(c.reel){
  const tl=ri=>({t:(ri===10?'🏎️ ':'')+R[ri].n,c:R[ri].c});
  st.innerHTML='<div id="rl0" style="width:100%"></div><div class="hint" style="margin-top:10px">Открываем кейс…</div>';
  playReel($('rl0'),()=>tl(pick(c.w)),tl(win.r),120,end);
 }else runSlots(st,win,end);
}
function sell(id){const i=S.inv.findIndex(x=>x.id===id);if(i<0)return;S.bal+=val(S.inv[i]);S.inv.splice(i,1);save();render()}
function render(){
 $('bal').textContent=rub(S.bal);
 document.querySelectorAll('.tab').forEach(t=>t.classList.toggle('on',t.dataset.m===mode));
 $('cases').innerHTML=M[mode].cases.map((c,i)=>`<div class="case"><h2>${c.t}</h2><p>${c.d}</p><div class="btns">${[1,10].map(n=>`<button data-i="${i}" data-n="${n}" ${busy||S.bal<c.cost*n?'disabled':''}>×${n} · ${rub(c.cost*n)}</button>`).join('')}</div></div>`).join('');
 $('cnt').textContent=S.inv.length;
 $('stats').textContent=`Круток: ${S.spins} · Лучшая находка: ${S.best?rub(S.best):'—'}`;
 $('inv').innerHTML=S.inv.slice(0,60).map(s=>mini(s,true)).join('')+(S.inv.length>60?`<div class="hint" style="grid-column:1/-1">…и ещё ${S.inv.length-60} (продай, чтобы увидеть)</div>`:'');
 $('reset').style.display=(!busy&&S.bal<3000&&!S.inv.length)?'':'none';
}
$('cases').onclick=e=>{const b=e.target.closest('button[data-i]');if(b)roll(+b.dataset.i,+b.dataset.n)};
document.querySelector('.tabs').onclick=e=>{const b=e.target.closest('.tab');if(b&&!busy){mode=b.dataset.m;render()}};
// ===== телефон =====
let pv=null;
const getPh=()=>S.inv.find(x=>x.id===pv.id);
function openPhone(id){pv={id,on:false,boot:false,view:'home',k:0,lock:false,fly:null,last:null};$('ov').classList.add('show');draw()}
function closePhone(f){if(pv&&pv.lock&&!f)return;pv=null;$('ov').classList.remove('show')}

function screenHTML(ph){
 const sim=ph.sim;
 if(pv.boot)return `<div class="boot"><div class="lg">${ph.name}</div><div class="bar"><i></i></div></div>`;
 if(!pv.on)return '<div class="off">Выключен</div>';
 const sb=`<div class="sbar"><span>${sim?sim.op:'Нет SIM'}</span><span>${sim?'▂▄▆█ ':''}🔋</span></div>`,c=CC[pv.k];
 if(pv.view==='home')return sb+`<div class="home"><div class="clock">${new Date().toLocaleTimeString('ru-RU',{hour:'2-digit',minute:'2-digit'})}</div><div class="apps"><button class="app" data-a="app"><b>🚗</b>Кейсы</button><button class="app" disabled><b>📞</b>Звонки</button><button class="app" disabled><b>💬</b>SMS</button><button class="app" disabled><b>📷</b>Камера</button></div></div>`;
 if(pv.view==='list')return sb+`<div class="capp"><b>🚗 Авто-кейсы</b>${CC.map((c,k)=>`<div class="cr" data-k="${k}"><span><b>${c.t}</b><br><small>${rub(c.cost)}</small></span><span>▶</span></div>`).join('')}<button class="sec" data-a="home" style="color:#fff">⌂ Домой</button></div>`;
 if(pv.view==='case')return sb+`<div class="capp"><b>${c.t}</b> · ${rub(c.cost)}<div style="margin:6px 0">${c.ids.map((id,j)=>`<div class="drop"><span>${CARS[id].n}</span><span>${c.w[j]}% · ${rub(CARS[id].p)}</span></div>`).join('')}</div><button data-a="openc" ${S.bal<c.cost?'disabled':''}>Открыть · ${rub(c.cost)}</button><button class="sec" data-a="app" style="color:#fff">← Назад</button></div>`;
 if(pv.view==='open')return sb+`<div class="capp"><b>${c.t}</b><div id="rl" style="margin-top:10px"></div></div>`;
 return sb+`<div class="capp">${carHTML(pv.last)}<button data-a="openc" ${S.bal<c.cost?'disabled':''}>Ещё раз · ${rub(c.cost)}</button><button class="sec" data-a="app" style="color:#fff">← К кейсам</button></div>`;
}
function draw(){
 const ph=getPh();if(!ph){closePhone(true);return}
 const r=R[ph.r],sim=ph.sim,L=pv.lock?'disabled':'';
 const sims=S.inv.filter(s=>s.kind==='sim').sort((a,b)=>b.price-a.price).slice(0,12);
 $('pbox').innerHTML=`<div class="phead"><div><b>${ph.name}</b><br><small style="color:var(--mut)">${r.n}</small></div><div style="text-align:right"><small style="color:var(--mut)">Баланс</small><br><b>${rub(S.bal)}</b></div><button class="sec" data-a="close" ${L}>✕</button></div>
<div class="phwrap"><div class="ph" style="border-color:${r.c};--w1:${r.c}"><div class="notch"></div><div class="scr">${screenHTML(ph)}</div></div><div class="tray ${sim?'full':''}"></div>${pv.fly?`<div class="simfly" style="background:${col(pv.fly)}"></div>`:''}</div>
<div class="tools" style="justify-content:center"><button data-a="pow" ${L}>${pv.on?'⏻ Выключить':'⏻ Включить'}</button></div>
${sim?`<div class="simline">📶 ${sim.op} ${sim.num} · <b>+${rub(sim.price)}</b></div><button class="sec" data-a="eject" ${L}>Достать SIM</button>`:sims.length?`<div class="hint" style="margin-top:6px">Вставить SIM:</div><div class="sims">${sims.map(s=>`<button class="sec" data-sid="${s.id}" ${L}>${s.op} · ${s.num} · ${rub(s.price)}</button>`).join('')}</div>`:'<div class="hint">В коллекции нет симок — выбей их на вкладке «Симки»</div>'}
<button data-a="sell" ${L} style="width:100%;margin-top:10px">Продать за ${rub(val(ph))}${sim?` (телефон + SIM)`:''}</button>`;
}
$('pbox').onclick=e=>{
 if(!pv)return;
 const k=e.target.closest('.cr'),b=e.target.closest('button');
 if(k&&!pv.lock){pv.k=+k.dataset.k;pv.view='case';draw();return}
 if(!b||b.disabled)return;
 const a=b.dataset.a,ph=getPh();
 if(a==='close'){closePhone();return}
 if(pv.lock)return;
 if(b.dataset.sid){
  const s=S.inv.find(x=>x.id==b.dataset.sid);if(!s||ph.sim)return;
  pv.lock=true;pv.fly=s;draw();
  setTimeout(()=>{if(!pv)return;S.inv=S.inv.filter(x=>x.id!==s.id);ph.sim=s;pv.fly=null;pv.lock=false;save();draw();render()},1600);
 }else if(a==='pow'){
  if(pv.on){pv.on=false;pv.view='home';draw()}
  else{pv.boot=true;pv.lock=true;draw();setTimeout(()=>{if(!pv)return;pv.boot=false;pv.lock=false;pv.on=true;pv.view='home';draw()},2800)}
 }else if(a==='eject'){S.inv.unshift(ph.sim);ph.sim=null;save();draw();render()}
 else if(a==='sell'){S.bal+=val(ph);S.inv=S.inv.filter(x=>x.id!==ph.id);save();closePhone(true);render()}
 else if(a==='app'){pv.view='list';draw()}
 else if(a==='home'){pv.view='home';draw()}
 else if(a==='openc'){
  const c=CC[pv.k];if(S.bal<c.cost||busy)return;
  S.bal-=c.cost;S.spins++;busy=true;pv.lock=true;pv.view='open';render();draw();
  const wo=Object.fromEntries(c.w.map((w,i)=>[i,w])),car=genCar(c.ids[pick(wo)]);
  const tl=q=>({t:q.n,c:`hsl(${q.h},55%,38%)`});
  playReel($('rl'),()=>tl(CARS[c.ids[pick(wo)]]),{t:car.name,c:`hsl(${car.h},55%,38%)`},96,()=>{
   S.inv.unshift(car);if(car.price>S.best)S.best=car.price;
   if(pv){pv.last=car;pv.view='result';pv.lock=false}
   busy=false;save();render();if(pv)draw();
  });
 }
};
$('inv').onclick=e=>{const o=e.target.closest('button[data-open]');if(o){openPhone(+o.dataset.open);return}const b=e.target.closest('button[data-id]');if(b)sell(+b.dataset.id)};
$('reset').onclick=()=>{S={bal:20000,inv:[],spins:0,best:0,id:1};save();render()};
$('sellAll').onclick=()=>{
 if(!S.inv.length)return;
 if(!sellArm){sellArm=1;$('sellAll').textContent='Точно? Нажми ещё раз';setTimeout(()=>{sellArm=0;$('sellAll').textContent='Продать всё'},3000);return}
 S.bal+=S.inv.reduce((a,s)=>a+val(s),0);S.inv=[];sellArm=0;$('sellAll').textContent='Продать всё';save();render();
};
$('sellLow').onclick=()=>{const k=S.inv.filter(s=>s.r<=2);S.bal+=k.reduce((a,s)=>a+val(s),0);S.inv=S.inv.filter(s=>s.r>2);save();render()};
$('tbl').innerHTML=R.filter(r=>r.ch>0).map(r=>`<div><span><i class="dot" style="background:${r.c}"></i>${r.n}</span><span>${r.ch}% · ${rub(r.a)} – ${rub(r.b)}</span></div>`).join('')+'<div><span><i class="dot" style="background:#0b3d91"></i>🏎️ Bugatti W16 Mistral (кейс номеров)</span><span>0.1% · 500 000 000 ₽</span></div>';
render();
</script>
</body>
</html>
