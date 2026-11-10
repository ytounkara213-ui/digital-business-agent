<!doctype html>
<html lang="fr">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="theme-color" content="#101827">
<title>TOUNKARA CYBER GUARDIAN AI</title>
<style>
:root{--bg:#0b1220;--panel:#121d30;--panel2:#17243a;--line:#263650;--text:#edf3ff;--muted:#9eacc2;--gold:#e8bd65;--green:#55c99a;--yellow:#f1c66d;--red:#f07b7b;--blue:#83b7ff}
*{box-sizing:border-box}body{margin:0;background:radial-gradient(circle at 80% 0%,#1b2b46 0,transparent 35%),var(--bg);color:var(--text);font:15px/1.5 system-ui,-apple-system,Segoe UI,Roboto,sans-serif}
.wrap{max-width:1180px;margin:auto;padding:26px 18px 50px}.top{display:flex;justify-content:space-between;align-items:center;gap:16px;flex-wrap:wrap;margin-bottom:22px}
.brand{display:flex;gap:13px;align-items:center}.shield{width:48px;height:48px;border-radius:15px;display:grid;place-items:center;background:linear-gradient(135deg,#e8bd65,#946b2e);color:#101827;font-size:25px;font-weight:900}
h1{font-size:clamp(20px,4vw,30px);margin:0;letter-spacing:.3px}.sub{color:var(--muted);font-size:13px}.pill{border:1px solid #3b5b50;color:#a5e5c8;background:#16352f;padding:7px 12px;border-radius:99px;font-size:12px}
.notice{padding:13px 15px;border:1px solid #705b32;background:#302819;border-radius:13px;color:#f4dca9;margin-bottom:18px;font-size:13px}
.grid{display:grid;grid-template-columns:repeat(4,minmax(0,1fr));gap:13px;margin:14px 0 20px}.card,.panel{background:linear-gradient(160deg,var(--panel),#101a2b);border:1px solid var(--line);border-radius:16px;padding:17px;min-width:0}
.metric small,.muted{color:var(--muted)}.metric strong{display:block;font-size:27px;margin-top:6px}.metric .hint{font-size:12px;color:var(--muted)}
.layout{display:grid;grid-template-columns:1.15fr .85fr;gap:14px}.panel h2{font-size:17px;margin:0 0 13px}.accounts{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:10px}
.account{background:var(--panel2);border:1px solid var(--line);border-radius:12px;padding:12px;display:flex;justify-content:space-between;gap:10px;align-items:center}
.account b{display:block}.account small{color:var(--muted)}.state{font-size:11px;border-radius:99px;padding:4px 8px;white-space:nowrap;background:#33303a;color:#f1d59a}
.state.off{background:#302a1e;color:#f1d59a}.state.ok{background:#17352e;color:#9de0c0}
.tools{display:flex;gap:8px;flex-wrap:wrap;margin-top:14px}.btn{border:1px solid #405574;background:#1b2a42;color:var(--text);padding:9px 12px;border-radius:10px;cursor:pointer;font-weight:600}.btn.primary{background:var(--gold);color:#172033;border-color:var(--gold)}.btn:hover{filter:brightness(1.1)}
textarea,input{width:100%;background:#0c1627;color:var(--text);border:1px solid #344761;border-radius:10px;padding:11px;font:inherit}textarea{min-height:115px;resize:vertical}.field{margin:10px 0}.field label{display:block;color:var(--muted);font-size:12px;margin-bottom:6px}
.result{margin-top:12px;padding:12px;border-radius:11px;background:#0c1627;border:1px solid var(--line);display:none}.result.show{display:block}.tag{font-size:11px;padding:3px 8px;border-radius:99px;font-weight:700}.high{background:#4a252b;color:#ffaaaa}.med{background:#47391e;color:#ffdc91}.low{background:#17382e;color:#a6e4c5}
ul.clean{padding-left:18px;margin:8px 0;color:var(--muted)}.activity{display:grid;gap:9px}.event{border-left:3px solid #526b8b;padding:3px 0 3px 11px;color:var(--muted);font-size:13px}.event b{color:var(--text)}
footer{margin-top:20px;color:var(--muted);font-size:12px;text-align:center}
@media(max-width:800px){.grid{grid-template-columns:repeat(2,minmax(0,1fr))}.layout{grid-template-columns:1fr}}
@media(max-width:480px){.accounts{grid-template-columns:1fr}.wrap{padding:18px 12px 36px}.card,.panel{padding:14px}}
</style>
</head>
<body>
<div class="wrap">
<header class="top">
  <div class="brand"><div class="shield">✦</div><div><h1>TOUNKARA CYBER GUARDIAN AI</h1><div class="sub">Centre de contrôle de sécurité numérique</div></div></div>
  <span class="pill">● Tableau de bord local</span>
</header>
<div class="notice"><b>Mode démonstration :</b> ce tableau de bord ne surveille pas automatiquement tes comptes. Les statuts sont « à vérifier » tant qu'une connexion officielle et autorisée n'est pas configurée. N'inscris jamais de mot de passe, code de vérification ou clé secrète ici.</div>

<section class="grid">
  <div class="card metric"><small>Comptes listés</small><strong>5</strong><div class="hint">Réseaux et messagerie</div></div>
  <div class="card metric"><small>Contrôles confirmés</small><strong id="checkedCount">0</strong><div class="hint">Dans cette session</div></div>
  <div class="card metric"><small>Risques détectés</small><strong id="riskCount">—</strong><div class="hint">Aucun audit connecté</div></div>
  <div class="card metric"><small>Prochain bilan</small><strong>Dimanche</strong><div class="hint">Rapport hebdomadaire programmé séparément</div></div>
</section>

<div class="layout">
<section class="panel">
  <h2>Comptes à protéger</h2>
  <div class="accounts" id="accounts">
    <div class="account"><div><b>TikTok</b><small>Compte social</small></div><span class="state off">À vérifier</span></div>
    <div class="account"><div><b>Instagram</b><small>Compte social</small></div><span class="state off">À vérifier</span></div>
    <div class="account"><div><b>Facebook</b><small>Compte social</small></div><span class="state off">À vérifier</span></div>
    <div class="account"><div><b>YouTube</b><small>Chaîne vidéo</small></div><span class="state off">À vérifier</span></div>
    <div class="account"><div><b>Gmail</b><small>Messagerie</small></div><span class="state off">À vérifier</span></div>
    <div class="account"><div><b>GitHub</b><small>Dépôts et code</small></div><span class="state off">Non connecté</span></div>
  </div>
  <div class="tools"><button class="btn" id="markReview">Marquer un contrôle manuel</button><button class="btn" id="reset">Réinitialiser la session</button></div>
</section>

<section class="panel">
  <h2>État des protections</h2>
  <div class="activity">
    <div class="event"><b>Authentification à deux facteurs</b><br>À confirmer dans chaque compte.</div>
    <div class="event"><b>Sessions et appareils</b><br>Non vérifiés — consulter les paramètres officiels.</div>
    <div class="event"><b>Applications connectées</b><br>Non vérifiées — examiner les autorisations.</div>
    <div class="event"><b>Dépôts GitHub</b><br>En attente de connexion et d'autorisation.</div>
    <div class="event"><b>Sauvegardes et récupération</b><br>À vérifier dans les paramètres officiels.</div>
  </div>
</section>

<section class="panel">
  <h2>Détecteur de message ou lien suspect</h2>
  <p class="muted">Colle un message ou un lien reçu. L'analyse locale recherche quelques signes d'alerte ; elle ne prouve pas qu'un contenu est sûr ou frauduleux.</p>
  <div class="field"><label for="sample">Message ou lien à examiner</label><textarea id="sample" placeholder="Colle ici le texte suspect. Retire d'abord tes informations personnelles et tout code confidentiel."></textarea></div>
  <button class="btn primary" id="analyze">Analyser les signes d'alerte</button>
  <div class="result" id="result" aria-live="polite"></div>
</section>

<section class="panel">
  <h2>Plan d'action prioritaire</h2>
  <ul class="clean">
    <li>Activer la double authentification sur les comptes importants.</li>
    <li>Utiliser un mot de passe unique pour chaque service.</li>
    <li>Vérifier les appareils et sessions connectés depuis les applications officielles.</li>
    <li>Ne jamais ouvrir une page de connexion depuis un lien inattendu.</li>
    <li>Sur GitHub, activer les alertes de sécurité et examiner les permissions des dépôts.</li>
    <li>Conserver les moyens de récupération en lieu sûr, hors de ce tableau de bord.</li>
  </ul>
</section>
</div>
<footer>TOUNKARA CYBER GUARDIAN AI · Prototype local · Aucune connexion à un compte externe</footer>
</div>
<script>
const checked = document.getElementById('checkedCount');
let checks = 0;
document.getElementById('markReview').addEventListener('click',()=>{
  checks += 1; checked.textContent = String(checks);
  alert('Contrôle manuel noté dans cette session. Cela ne signifie pas qu’un compte a été audité automatiquement.');
});
document.getElementById('reset').addEventListener('click',()=>{
  checks = 0; checked.textContent = '0';
  document.getElementById('riskCount').textContent = '—';
  document.getElementById('result').className = 'result';
  document.getElementById('sample').value = '';
});
document.getElementById('analyze').addEventListener('click',()=>{
  const value = document.getElementById('sample').value.trim();
  const result = document.getElementById('result');
  if(!value){result.className='result show';result.textContent='Ajoute un message ou un lien à examiner.';return;}
  const patterns = [
    ['Demande de mot de passe, code ou données bancaires',/mot de passe|password|code de vérification|code sms|coordonnées bancaires|carte bancaire|pin\b/i],
    ['Urgence ou menace pour pousser à agir vite',/urgent|immédiatement|dans les \d+ minutes|dernier avertissement|compte sera suspendu|bloqué aujourd'hui/i],
    ['Promesse de gain ou cadeau inattendu',/vous avez gagné|gain garanti|cadeau gratuit|réclamez votre prix|lotterie|million/i],
    ['Demande de paiement ou frais préalables',/frais de dossier|payer.*débloquer|frais.*livraison|envoyez.*argent|transfert d'argent/i],
    ['Lien ou adresse web à vérifier avec prudence',/https?:\/\/|www\./i]
  ];
  const found = patterns.filter(p=>p[1].test(value)).map(p=>p[0]);
  let level = found.length>=3?'Élevé':found.length>=1?'À examiner':'Aucun signe repéré par les règles simples';
  let cls = found.length>=3?'high':found.length>=1?'med':'low';
  result.className='result show';
  result.innerHTML='<span class="tag '+cls+'">'+level+'</span><p><b>Signes repérés :</b></p>';
  if(found.length){const ul=document.createElement('ul');found.forEach(item=>{const li=document.createElement('li');li.textContent=item;ul.appendChild(li)});result.appendChild(ul);}
  else {const p=document.createElement('p');p.textContent='Les règles locales n’ont repéré aucun des signes recherchés. Cela ne garantit pas que le message ou le lien soit fiable.';result.appendChild(p);}
  const advice=document.createElement('p');advice.textContent='Conseil : ne partage aucun code ni mot de passe. Vérifie toute demande en ouvrant toi-même l’application ou le site officiel, sans utiliser le lien reçu.';result.appendChild(advice);
});
</script>
</body>
</html>