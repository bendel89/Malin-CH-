<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="utf-8">
<title>Malin CH</title>
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<style>
:root{--bg:#f2f6fc;--card:#fff;--tx:#1b2430;--mu:#6b7785;--ac:#2563eb;--ok:#16a34a;--er:#dc2626;--bd:#e3e9f1;--sh:0 6px 20px rgba(37,99,235,.10);box-sizing:border-box;padding-top:env(safe-area-inset-top,0px)}
@media(prefers-color-scheme:dark){:root{--bg:#0f141c;--card:#19212c;--tx:#e8eef6;--mu:#98a5b5;--bd:#2a3442;--sh:0 6px 20px rgba(0,0,0,.4)}}
*{box-sizing:border-box}
html,body{margin:0;background:linear-gradient(160deg,#dbe8ff,var(--bg) 40%,#e2f6ea) fixed;color:var(--tx);font:17px/1.45 -apple-system,system-ui,Helvetica,sans-serif}
@media(prefers-color-scheme:dark){html,body{background:linear-gradient(160deg,#14233f,var(--bg) 40%,#12261c) fixed}}
main{max-width:640px;margin:0 auto;padding:12px 14px 100px}
h1{font-size:26px;margin:6px 0 4px}h2{font-size:17px;margin:0 0 8px}
.card{background:var(--card);border-radius:20px;padding:14px;margin-bottom:12px;box-shadow:var(--sh)}
input,select,button{font:inherit;color:var(--tx);background:var(--bg);border:1px solid var(--bd);border-radius:12px;padding:12px;width:100%;margin:4px 0}
button{background:linear-gradient(135deg,var(--ac),#0ea5a4);color:#fff;border:0;font-weight:600;cursor:pointer}
button.s{background:var(--bg);color:var(--tx);border:1px solid var(--bd)}
button.x{width:auto;padding:4px 10px;background:none;color:var(--mu)}
.row{display:flex;gap:8px}.row>*{flex:1}
.mu{color:var(--mu);font-size:14px}
.big{font-size:32px;font-weight:700;color:var(--ok)}
.item{display:flex;align-items:center;gap:10px;padding:10px 0;border-bottom:1px solid var(--bd)}.item:last-child{border:0}
.item input[type=checkbox]{width:26px;height:26px;margin:0;flex:none}
.item.d span{text-decoration:line-through;color:var(--mu)}
.best{background:rgba(22,163,74,.14);border-radius:10px;padding:8px}
.warn{background:rgba(220,38,38,.1);border:1px solid var(--er);border-radius:12px;padding:10px;margin-bottom:12px}
.chip{display:inline-block;background:var(--bg);border-radius:20px;padding:3px 10px;font-size:13px;margin:2px}
.bar{height:10px;background:var(--bd);border-radius:6px;overflow:hidden;margin:6px 0}.bar i{display:block;height:100%;background:var(--ok)}
nav{position:fixed;bottom:0;left:0;right:0;display:flex;overflow-x:auto;background:var(--card);box-shadow:0 -4px 20px rgba(0,0,0,.08);padding-bottom:env(safe-area-inset-bottom,0px)}
nav button{background:none;color:var(--mu);border-radius:0;font-size:11px;padding:8px 6px;margin:0;flex:1 0 auto;min-width:68px;width:auto}
nav button.on{color:var(--ac)}nav span{display:block;font-size:22px}
</style>
</head>
<body>
<main id="app"></main>
<nav id="nav"></nav>
<script>
const CATS=["Assurance maladie","Mobile","Internet / TV","Assurance ménage / RC","Assurance auto","Électricité / gaz","Banque / carte","Autre"];
const KEY="malin_v1";
const XD={exp:[],crit:[],opt:[],px:[],lt:{}};
let S={off:{},con:[],goal:{t:1000,s:0},tips:[],x:XD},tab="home",cat=CATS[0],M=12;
try{const r=localStorage.getItem(KEY);if(r){const o=JSON.parse(r);S=Object.assign(S,o);S.x=Object.assign({},XD,o.x||{})}}catch(e){}
const save=()=>{try{localStorage.setItem(KEY,JSON.stringify(S))}catch(e){}};
const $=id=>document.getElementById(id);
const esc=s=>String(s??"").replace(/[&<>"]/g,c=>({"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;"}[c]));
const chf=n=>(Math.round(n*100)/100).toLocaleString("fr-CH",{minimumFractionDigits:2,maximumFractionDigits:2})+" CHF";
const X=()=>S.x,td=()=>new Date().toISOString().slice(0,10);
const cp=t=>{try{navigator.clipboard.writeText(t);alert("Copié")}catch(e){alert(t)}};
const TABS=[["home","🏠","Accueil"],["cmp","🔍","Comparer"],["con","📑","Contrats"],["lamal","🏥","Franchise"],["bud","💰","Budget"],["uni","⚖️","Universel"],["prix","📈","Prix"],["ag","📅","Agenda"],["lett","✉️","Lettres"],["out","🧮","Outils"],["tips","💡","Astuces"],["bk","💾","Données"]];
function go(t){tab=t;render();scrollTo(0,0)}
function render(){$("nav").innerHTML=TABS.map(t=>`<button class="${tab==t[0]?"on":""}" onclick="go('${t[0]}')"><span>${t[1]}</span>${t[2]}</button>`).join("");$("app").innerHTML=({home,cmp,con,lamal,bud,uni,prix,ag,lett,out,tips,bk})[tab]()}

/* COMPARER */
function addO(){const n=$("on").value.trim(),p=+$("op").value;if(!n||!p)return;(S.off[cat]=S.off[cat]||[]).push({n,p,f:+$("of").value||0,cur:$("oc").checked});save();render()}
function delO(i){S.off[cat].splice(i,1);save();render()}
function setCat(v){cat=v;render()}
function setM(v){M=+v;render()}
function sav(){let s=0;CATS.forEach(c=>{const L=S.off[c]||[],cu=L.find(o=>o.cur);if(!cu)return;const b=L.reduce((m,o)=>o.p<m.p?o:m,L[0]);if(b.p<cu.p)s+=(cu.p-b.p)*12});return s}
function cmp(){
  const L=(S.off[cat]||[]).map((o,i)=>({...o,i,t:o.p*M+o.f})).sort((a,b)=>a.t-b.t);
  const cu=L.find(o=>o.cur),best=L[0],base=cu||L[L.length-1],sv=L.length>1?base.t-best.t:0;
  return `<h1>🔍 Comparer</h1><div class="mu">Entre les prix trouvés sur comparis.ch, priminfo.admin.ch ou chez les fournisseurs.</div><br>
  <div class="card"><select onchange="setCat(this.value)">${CATS.map(c=>`<option ${c==cat?"selected":""}>${c}</option>`).join("")}</select>
  <select onchange="setM(this.value)">${[12,24,36].map(m=>`<option value="${m}" ${m==M?"selected":""}>Comparer sur ${m} mois</option>`).join("")}</select></div>
  <div class="card"><input id="on" placeholder="Nom de l'offre"><div class="row"><input id="op" type="number" inputmode="decimal" placeholder="Prix / mois"><input id="of" type="number" inputmode="decimal" placeholder="Frais uniques"></div>
  <label class="item" style="border:0"><input id="oc" type="checkbox"><span>C'est mon offre actuelle</span></label><button onclick="addO()">Ajouter l'offre</button></div>
  ${sv>0?`<div class="card best"><div class="mu">Économie possible sur ${M} mois</div><div class="big">${chf(sv)}</div><div class="mu">avec « ${esc(best.n)} » · environ ${chf(sv/M*12)} par an</div></div>`:""}
  <div class="card">${L.map((o,k)=>`<div class="item ${k==0?"best":""}"><div style="flex:1"><b>${k==0?"🏆 ":""}${esc(o.n)}</b>${o.cur?' <span class="chip">actuelle</span>':""}<div class="mu">${chf(o.p)}/mois · frais ${chf(o.f)}</div></div><div style="text-align:right"><b>${chf(o.t)}</b><div class="mu">sur ${M} mois</div></div><button class="x" onclick="delO(${o.i})">✕</button></div>`).join("")||'<div class="mu">Aucune offre pour cette catégorie</div>'}</div>`;
}
/* CONTRATS */
function addC(){const n=$("cn").value.trim();if(!n)return;S.con.push({n,c:$("cc").value,p:+$("cp").value||0,e:$("ce").value,nt:+$("cnt").value||30});save();render()}
function delC(i){S.con.splice(i,1);save();render()}
const dleft=e=>e?Math.ceil((new Date(e)-new Date().setHours(0,0,0,0))/864e5):null;
function con(){
  const L=S.con.map((c,i)=>({...c,i,d:dleft(c.e)})).sort((a,b)=>(a.d??9e9)-(b.d??9e9)),tot=S.con.reduce((s,c)=>s+c.p,0);
  return `<h1>📑 Mes contrats</h1><div class="card"><div class="mu">Total par mois</div><div class="big" style="color:var(--tx)">${chf(tot)}</div><div class="mu">${chf(tot*12)} par an</div></div>
  <div class="card"><input id="cn" placeholder="Nom (ex. Mobile Swisscom)"><select id="cc">${CATS.map(c=>`<option>${c}</option>`).join("")}</select><div class="row"><input id="cp" type="number" inputmode="decimal" placeholder="Prix / mois"><input id="cnt" type="number" placeholder="Préavis (jours)" value="30"></div><label class="mu">Fin du contrat</label><input id="ce" type="date"><button onclick="addC()">Ajouter</button></div>
  <div class="card">${L.map(c=>{const lim=c.d===null?null:c.d-c.nt;const m=lim===null?"":lim<0?'<span style="color:var(--er)">⚠️ Délai de résiliation dépassé</span>':lim<=30?`<span style="color:var(--er)">⏰ Résilier dans ${lim} j</span>`:`Résilier avant le ${new Date(new Date(c.e)-c.nt*864e5).toLocaleDateString("fr-CH")}`;return `<div class="item"><div style="flex:1"><b>${esc(c.n)}</b> <span class="chip">${esc(c.c)}</span><div class="mu">${chf(c.p)}/mois</div><div class="mu">${m}</div></div><button class="x" onclick="delC(${c.i})">✕</button></div>`}).join("")||'<div class="mu">Aucun contrat</div>'}</div>`;
}

/* ACCUEIL */
function home(){
  const tot=S.con.reduce((s,c)=>s+c.p,0)*12,urg=S.con.map(c=>({...c,l:dleft(c.e)-c.nt})).filter(c=>!isNaN(c.l)&&c.l<=30).sort((a,b)=>a.l-b.l),g=S.goal;
  return `<h1>Malin CH 💸</h1><div class="mu">Chaque franc économisé compte.</div><br>
  <div class="card best"><div class="mu">Économie annuelle possible</div><div class="big">${chf(sav())}</div><div class="mu">calculée d'après tes offres comparées</div></div>
  <div class="card"><div class="mu">Mes contrats coûtent</div><div class="big" style="color:var(--tx)">${chf(tot)}</div><div class="mu">par an</div></div>
  ${urg.length?`<div class="warn"><b>À résilier bientôt :</b>${urg.map(c=>`<div>${esc(c.n)} : ${c.l<0?"délai dépassé":"dans "+c.l+" j"}</div>`).join("")}</div>`:""}
  <div class="card"><h2>🎯 Mon objectif d'épargne</h2><div class="mu">${chf(g.s)} sur ${chf(g.t)}</div><div class="bar"><i style="width:${Math.min(100,g.s/(g.t||1)*100)}%"></i></div></div>
  <div class="card"><h2>💡 Astuces</h2><div class="mu">${S.tips.length}/${TIPS.length} faites. Va dans l'onglet Astuces.</div></div>`;
}

/* OUTILS */
function unit(){const f=(p,q)=>p>0&&q>0?p/q:Infinity,a=f(+$("u1p").value,+$("u1q").value),b=f(+$("u2p").value,+$("u2q").value);$("uo").innerHTML=a==Infinity||b==Infinity?"Remplis les 4 champs":a<b?`<b style="color:var(--ok)">A est moins cher</b> (${chf(a)} contre ${chf(b)} l'unité)`:`<b style="color:var(--ok)">B est moins cher</b> (${chf(b)} contre ${chf(a)} l'unité)`}
function use(){const p=+$("sp").value,u=+$("su").value;$("so").innerHTML=p&&u?`Chaque usage te coûte <b>${chf(p/u)}</b>`:""}
function fx(){const a=+$("fa").value,r=+$("fr").value;$("fo").innerHTML=a&&r?`${a} EUR = <b>${chf(a*r)}</b>`:""}
function addG(){S.goal.s+=+$("ga").value||0;save();render()}
function setG(){S.goal.t=+$("gt").value||0;save();render()}
function c1(){const P=+$("kp").value,r=+$("kr").value/1200,n=+$("kn").value*12;$("ko").innerHTML=P&&n?(m=>`Mensualité <b>${chf(m)}</b> · coût total ${chf(m*n)} · intérêts ${chf(m*n-P)}`)(r?P*r/(1-Math.pow(1+r,-n)):P/n):""}
function c2(){const v=Math.min(+$("tv").value,+$("tm").value),t=+$("tt").value;$("to").innerHTML=v?`Économie d'impôt estimée : <b>${chf(v*t/100)}</b> par an`:""}
function out(){const g=S.goal;setTimeout(()=>{c1();c2()},0);return `<h1>🧮 Outils</h1>
  <div class="card"><h2>⚖️ Meilleur prix à l'unité</h2><div class="row"><input id="u1p" type="number" placeholder="Prix A" oninput="unit()"><input id="u1q" type="number" placeholder="Quantité A" oninput="unit()"></div><div class="row"><input id="u2p" type="number" placeholder="Prix B" oninput="unit()"><input id="u2q" type="number" placeholder="Quantité B" oninput="unit()"></div><div id="uo"></div></div>
  <div class="card"><h2>📊 Prix par usage</h2><div class="row"><input id="sp" type="number" placeholder="Prix / mois" oninput="use()"><input id="su" type="number" placeholder="Usages / mois" oninput="use()"></div><div id="so"></div></div>
  <div class="card"><h2>💶 EUR → CHF</h2><div class="row"><input id="fa" type="number" placeholder="Montant EUR" oninput="fx()"><input id="fr" type="number" step="0.01" placeholder="Taux (ex. 0.93)" oninput="fx()"></div><div id="fo"></div></div>
  <div class="card"><h2>🏦 Crédit ou leasing</h2><div class="row"><input id="kp" type="number" placeholder="Montant" value="20000" oninput="c1()"><input id="kr" type="number" placeholder="Taux %" value="5" oninput="c1()"><input id="kn" type="number" placeholder="Années" value="4" oninput="c1()"></div><div id="ko"></div></div>
  <div class="card"><h2>🧓 3e pilier (3a)</h2><div class="row"><input id="tv" type="number" placeholder="Versement" value="3000" oninput="c2()"><input id="tt" type="number" placeholder="Taux marginal %" value="20" oninput="c2()"></div><label class="mu">Plafond annuel (à vérifier sur admin.ch)</label><input id="tm" type="number" value="7258" oninput="c2()"><div id="to"></div></div>
  <div class="card"><h2>🎯 Objectif d'épargne</h2><div class="row"><input id="gt" type="number" value="${g.t}" placeholder="Objectif"><button class="s" onclick="setG()">Définir</button></div><div class="row"><input id="ga" type="number" placeholder="Montant mis de côté"><button onclick="addG()">Ajouter</button></div><div class="bar"><i style="width:${Math.min(100,g.s/(g.t||1)*100)}%"></i></div><div class="mu">${chf(g.s)} sur ${chf(g.t)}</div></div>`}

/* ASTUCES */
const TIPS=["Comparer ma caisse maladie sur priminfo.admin.ch (changement possible jusqu'au 30 novembre)","Demander la réduction de primes (subside) auprès de mon canton","Me renseigner sur mes droits aux prestations complémentaires (caisse de compensation ou commune)","Choisir la franchise qui correspond à mes frais de santé réels","Demander les génériques en pharmacie (souvent moins chers)","Passer à un abonnement mobile low-cost ou prépayé si je consomme peu","Comparer mon internet et demander une meilleure offre à l'échéance","Résilier les abonnements que je n'utilise plus","Comparer mon assurance ménage / RC","Me renseigner sur les cartes de réduction locales (ex. Carte Culture Caritas)","Ne jamais signer au téléphone : demander l'offre par écrit","Noter mes dates de résiliation dans l'onglet Contrats"];
function togT(i){const k=S.tips.indexOf(i);k<0?S.tips.push(i):S.tips.splice(k,1);save();render()}
function tips(){return `<h1>💡 Astuces pour économiser</h1><div class="mu">Vérifie toujours les conditions auprès de l'organisme concerné.</div><br><div class="card">${TIPS.map((t,i)=>`<div class="item ${S.tips.includes(i)?"d":""}"><input type="checkbox" ${S.tips.includes(i)?"checked":""} onchange="togT(${i})"><span>${t}</span></div>`).join("")}</div>`}
/* FRANCHISE LAMAL */
const FR=[[300,0],[500,70],[1000,310],[1500,550],[2000,790],[2500,1030]];
function lm(){const L=X().lt;L.p=+$("lp").value||0;L.c=+$("lc").value||0;save();
 const r=FR.map(([f,d])=>{const pr=L.p*12-d,q=Math.min(700,Math.max(0,L.c-f)*.1);return{f,t:pr+Math.min(L.c,f)+q,w:pr+f+700}}),b=Math.min(...r.map(x=>x.t));
 $("lr").innerHTML=`<table style="width:100%;font-size:14px;text-align:right"><tr><th style="text-align:left">Franchise</th><th>Total prévu</th><th>Pire année</th></tr>${r.map(x=>`<tr class="${x.t==b?"best":""}"><td style="text-align:left">${x.f}</td><td>${Math.round(x.t)}</td><td>${Math.round(x.w)}</td></tr>`).join("")}</table><div class="mu">Rabais de prime estimés (adultes). Vérifie ton tarif sur priminfo.admin.ch.</div>`}
function lamal(){const L=X().lt;setTimeout(lm,0);return `<h1>🏥 Franchise LAMal</h1><div class="card"><label class="mu">Prime mensuelle avec franchise 300</label><input id="lp" type="number" value="${L.p??400}" oninput="lm()"><label class="mu">Frais de santé annuels prévus</label><input id="lc" type="number" value="${L.c??800}" oninput="lm()"><div id="lr"></div></div><div class="card mu">« Pire année » = prime + franchise + quote-part maximale (700). Choisis selon ce que tu peux supporter.</div>`}

/* BUDGET */
function addB(){const a=+$("ba").value;if(!a)return;X().exp.unshift({d:td(),t:$("bt").value,a,c:$("bc").value,n:$("bn").value});save();render()}
function delB(i){X().exp.splice(i,1);save();render()}
function bud(){const m=td().slice(0,7),A=X().exp.map((e,i)=>({...e,i})).filter(e=>e.d.slice(0,7)==m),sum=t=>A.filter(e=>(e.t=="Revenu")==t).reduce((s,e)=>s+e.a,0),inc=sum(true),ex=sum(false),by={};
 A.filter(e=>e.t!="Revenu").forEach(e=>by[e.c]=(by[e.c]||0)+e.a);const rate=inc?Math.round((inc-ex)/inc*100):0;
 return `<h1>💰 Budget du mois</h1><div class="card"><div class="row"><div><div class="mu">Revenus</div><b>${chf(inc)}</b></div><div><div class="mu">Dépenses</div><b>${chf(ex)}</b></div></div><div class="mu">Reste : <b style="color:${inc-ex<0?"var(--er)":"var(--ok)"}">${chf(inc-ex)}</b> · épargne ${rate}%</div><div class="bar"><i style="width:${Math.max(0,Math.min(100,rate))}%"></i></div></div>
 <div class="card"><div class="row"><select id="bt"><option>Dépense</option><option>Revenu</option></select><input id="ba" type="number" inputmode="decimal" placeholder="Montant"></div><select id="bc">${["Logement","Santé","Courses","Transport","Loisirs","Abonnements","Autre"].map(c=>`<option>${c}</option>`).join("")}</select><input id="bn" placeholder="Note"><button onclick="addB()">Ajouter</button></div>
 <div class="card"><h2>Par catégorie</h2>${Object.entries(by).sort((a,b)=>b[1]-a[1]).map(([c,v])=>`<div class="item" style="display:block"><div style="display:flex;justify-content:space-between"><span>${c}</span><b>${chf(v)}</b></div><div class="bar"><i style="width:${v/ex*100}%"></i></div></div>`).join("")||'<div class="mu">Aucune dépense</div>'}</div>
 <div class="card">${A.slice(0,20).map(e=>`<div class="item"><div style="flex:1">${e.t=="Revenu"?"➕":"➖"} ${esc(e.c)}<div class="mu">${e.d} ${esc(e.n)}</div></div><b>${chf(e.a)}</b><button class="x" onclick="delB(${e.i})">✕</button></div>`).join("")}</div>`}

/* COMPARATEUR UNIVERSEL */
function addCr(){const n=$("cn2").value.trim();if(!n)return;X().crit.push({n,w:+$("cw").value});X().opt.forEach(o=>o.s.push(5));save();render()}
function addOp(){const n=$("on2").value.trim();if(!n||!X().crit.length)return;const s=X().crit.map(c=>Math.max(1,Math.min(10,+prompt(n+" : "+c.n+" (1 à 10) ?","5")||5)));X().opt.push({n,s});save();render()}
function delU(k,i){X()[k].splice(i,1);if(k=="crit")X().opt.forEach(o=>o.s.splice(i,1));save();render()}
function uni(){const C=X().crit,W=C.reduce((s,c)=>s+c.w,0)||1,R=X().opt.map((o,i)=>({n:o.n,i,p:Math.round(o.s.reduce((s,v,j)=>s+v*C[j].w,0)/(W*10)*100)})).sort((a,b)=>b.p-a.p);
 return `<h1>⚖️ Comparateur universel</h1><div class="mu">Compare n'importe quoi (téléphone, voiture, job, appartement…) avec tes propres critères.</div><br>
 <div class="card"><h2>1. Mes critères</h2><div class="row"><input id="cn2" placeholder="Ex. prix, qualité"><select id="cw"><option value="1">Peu important</option><option value="3" selected>Important</option><option value="5">Essentiel</option></select></div><button class="s" onclick="addCr()">Ajouter le critère</button>${C.map((c,i)=>`<span class="chip">${esc(c.n)} ×${c.w} <a onclick="delU('crit',${i})">✕</a></span>`).join("")}</div>
 <div class="card"><h2>2. Mes options</h2><input id="on2" placeholder="Nom de l'option"><button onclick="addOp()">Ajouter et noter</button></div>
 <div class="card">${R.map((r,k)=>`<div class="item ${k==0?"best":""}" style="display:block"><div style="display:flex;justify-content:space-between"><b>${k==0?"🏆 ":""}${esc(r.n)}</b><b>${r.p}%</b><button class="x" onclick="delU('opt',${r.i})">✕</button></div><div class="bar"><i style="width:${r.p}%"></i></div></div>`).join("")||'<div class="mu">Ajoute des critères puis des options</div>'}</div>`}
/* SUIVI DES PRIX */
function addP(){const n=$("pn").value.trim().toLowerCase(),p=+$("pp").value;if(!n||!p)return;X().px.push({n,d:td(),p,s:$("ps").value});save();render()}
function delP(n){X().px=X().px.filter(e=>e.n!=n);save();render()}
function prix(){const g={};X().px.forEach(e=>(g[e.n]=g[e.n]||[]).push(e));
 return `<h1>📈 Suivi des prix</h1><div class="mu">Note le prix d'un produit à chaque achat : l'appli te dit si c'est le bon moment.</div><br>
 <div class="card"><input id="pn" placeholder="Produit (ex. café 500 g)"><div class="row"><input id="pp" type="number" inputmode="decimal" placeholder="Prix"><input id="ps" placeholder="Magasin"></div><button onclick="addP()">Enregistrer le prix</button></div>
 ${Object.entries(g).map(([n,L])=>{const l=L[L.length-1],mn=L.reduce((m,e)=>e.p<m.p?e:m,L[0]),av=L.reduce((s,e)=>s+e.p,0)/L.length,v=l.p<=mn.p*1.03?"✅ Bon prix":l.p>av?"⏳ Plutôt cher, attends":"👌 Correct";return `<div class="card"><b>${esc(n)}</b> <button class="x" onclick="delP(decodeURIComponent('${encodeURIComponent(n).replace(/'/g,"%27")}'))">✕</button><div>${v}</div><div class="mu">Dernier ${chf(l.p)} · Min ${chf(mn.p)} (${esc(mn.s)}) · Moy. ${chf(av)} · ${L.length} relevé(s)</div></div>`}).join("")}`}

/* AGENDA */
function nx(m,d){const t=new Date().setHours(0,0,0,0),y=new Date(new Date().getFullYear(),m-1,d);if(y<t)y.setFullYear(y.getFullYear()+1);return y}
function ag(){const t=new Date().setHours(0,0,0,0),E=[["Changement de caisse maladie",nx(11,30)],["Dernier jour pour verser au 3e pilier",nx(12,31)],["Déclaration d'impôts (varie selon le canton)",nx(3,31)]];
 S.con.forEach(c=>{if(c.e)E.push(["Résilier : "+c.n,new Date(new Date(c.e)-c.nt*864e5)])});
 return `<h1>📅 Agenda des échéances</h1><div class="mu">Dates indicatives : vérifie celles de ton canton et de tes contrats.</div><br><div class="card">${E.sort((a,b)=>a[1]-b[1]).map(e=>{const d=Math.ceil((e[1]-t)/864e5);return `<div class="item"><div style="flex:1">${esc(e[0])}<div class="mu">${e[1].toLocaleDateString("fr-CH")}</div></div><b style="color:${d<=30?"var(--er)":"var(--ok)"}">${d<0?"dépassé":d+" j"}</b></div>`}).join("")}</div>`}

/* LETTRES TYPES */
const LT=[["Résiliation de contrat","Madame, Monsieur,\n\nPar la présente, je résilie mon contrat n° [NUMÉRO] pour la prochaine échéance possible, soit le [DATE]. Merci de me confirmer la résiliation par écrit.\n\nSalutations distinguées,\n[NOM ET ADRESSE]"],
["Négocier avec une offre concurrente","Madame, Monsieur,\n\nJe suis client depuis [DURÉE]. J'ai reçu une offre à [PRIX] CHF par mois pour un service équivalent. Pouvez-vous m'indiquer si vous pouvez adapter mon tarif ? Sinon, je résilierai pour la prochaine échéance.\n\nSalutations distinguées,\n[NOM]"],
["Contester une facture","Madame, Monsieur,\n\nJe conteste la facture n° [NUMÉRO] du [DATE] d'un montant de [MONTANT] CHF, pour la raison suivante : [MOTIF]. Je vous prie de la vérifier et de m'envoyer une réponse écrite.\n\nSalutations distinguées,\n[NOM]"],
["Demander un renseignement sur mes droits","Madame, Monsieur,\n\nJe souhaite savoir si j'ai droit à [AIDE / SUBSIDE / PRESTATION]. Ma situation : [SITUATION BRÈVE]. Pouvez-vous m'indiquer les conditions et les documents à fournir ?\n\nSalutations distinguées,\n[NOM]"]];
function lett(){return `<h1>✉️ Lettres types</h1><div class="mu">Complète les [CROCHETS], puis copie.</div><br>${LT.map((l,i)=>`<div class="card"><b>${l[0]}</b><div class="mu" style="white-space:pre-wrap;margin:6px 0">${esc(l[1])}</div><button class="s" onclick="cp(LT[${i}][1])">Copier</button></div>`).join("")}`}

/* DONNÉES */
function ex(){$("bkx").value=JSON.stringify(S)}
function im(){try{Object.assign(S,JSON.parse($("bkx").value));save();render()}catch(e){alert("Données invalides")}}
function rz(){if(confirm("Tout effacer ?")){try{localStorage.removeItem(KEY)}catch(e){}location.reload()}}
function bk(){return `<h1>💾 Mes données</h1><div class="card"><div class="mu">Tout reste sur ton téléphone. Exporte pour faire une copie.</div><div class="row"><button class="s" onclick="ex()">Exporter</button><button class="s" onclick="im()">Importer</button></div><input id="bkx" placeholder="Données"><button class="s" onclick="rz()">Tout effacer</button></div>`}

render();
</script>
</body>
</html>
