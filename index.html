<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CRIMSON FACTIONS</title>
<meta name="description" content="Facções Americanas - Crimson City RP">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Bebas+Neue&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#0a0a0b; --bg-soft:#121214; --card:#161618; --border:#2a2a2e;
    --accent:#dc143c; --accent-glow:color-mix(in srgb, var(--accent) 45%, transparent);
    --text:#f2f2f3; --text-dim:#9a9aa0; --success:#2bd97a; --warn:#e0b020; --danger:#d92b2b;
  }
  *{box-sizing:border-box;margin:0;padding:0}
  html,body{height:100%; margin:0}
  body{background:var(--bg);color:var(--text);font-family:'Inter',sans-serif;overflow-x:hidden}
  canvas#particles{position:fixed;inset:0;z-index:0;pointer-events:none}
  /* (CSS completo mantido igual ao original - não repeti aqui por tamanho) */
</style>
</head>
<body>
<canvas id="particles"></canvas>

<!-- PUBLIC VIEW -->
<div id="publicView">
  <div class="wrap">
    <header class="hero">
      <span class="badge" id="statusBadge">Inscrições Abertas</span>
      <h1 id="siteTitle">CRIMSON FACTIONS</h1>
      <p class="subtitle" id="siteSubtitle">Inscreva-se para as Facções Americanas</p>
    </header>
    <div class="card" id="formCard"></div>
    <p class="footer-note" id="footerNote">Crimson City RP &copy; <span id="year"></span></p>
  </div>
  <a href="#/admin" class="admin-link">admin</a>
</div>

<!-- ADMIN LOGIN + PANEL (mantido) -->
<!-- ... (o resto do HTML do login e admin é igual) ... -->

<script type="module">
import { initializeApp } from "https://www.gstatic.com/firebasejs/10.12.2/firebase-app.js";
import { getAuth, signInWithEmailAndPassword, onAuthStateChanged, signOut } from "https://www.gstatic.com/firebasejs/10.12.2/firebase-auth.js";
import { getFirestore, doc, getDoc, setDoc, collection, addDoc, getDocs, deleteDoc, updateDoc, query, orderBy, serverTimestamp } from "https://www.gstatic.com/firebasejs/10.12.2/firebase-firestore.js";
import { getStorage, ref as storageRef, uploadBytes, getDownloadURL } from "https://www.gstatic.com/firebasejs/10.12.2/firebase-storage.js";

// ==================== NOVO FIREBASE ====================
const firebaseConfig = {
  apiKey: "AIzaSyDpFNHdS5qyvzisflT0sik-XOf5vkiHFX0",
  authDomain: "cidade-avancada-4aa20.firebaseapp.com",
  projectId: "cidade-avancada-4aa20",
  storageBucket: "cidade-avancada-4aa20.firebasestorage.app",
  messagingSenderId: "703999683431",
  appId: "1:703999683431:web:df2f9aae59f61e198b9dc2",
  measurementId: "G-25VS45NJPT"
};
// ======================================================

const fbApp = initializeApp(firebaseConfig);
const auth = getAuth(fbApp);
const db = getFirestore(fbApp);
let storage = getStorage(fbApp);

document.getElementById('year').textContent = new Date().getFullYear();

// ... (todo o código de router, login, public form, particles, etc. continua igual) ...

// Perguntas padrão para Facções
const DEFAULT_QUESTIONS = [
  { id:'q_nome', label:'Nome IC / Personagem', type:'text', required:true },
  { id:'q_discord', label:'Discord', type:'text', required:true },
  { id:'q_idade', label:'Idade Real', type:'number', required:true },
  { id:'q_id_cidade', label:'ID na Cidade', type:'text', required:true },
  { id:'q_facao', label:'Facção Desejada', type:'select', required:true, options:['The Families','Ballas','Vagos','Lost MC','Mara Salvatrucha','Mafia','Cartel Mexicano','Outra'] },
  { id:'q_tempo_rp', label:'Tempo de RP (meses)', type:'number', required:true },
  { id:'q_por_que', label:'Por que quer entrar nessa facção?', type:'textarea', required:true },
  { id:'q_contribuicao', label:'Como pretende contribuir?', type:'textarea', required:true },
  { id:'q_horario', label:'Horário disponível', type:'text', required:true },
  { id:'q_experiencia', label:'Experiência em facções', type:'textarea', required:true }
];

// Expansão do Admin (mais configs)
async function loadSiteConfig() {
  const snap = await getDoc(doc(db,'config','site'));
  const site = snap.exists() ? snap.data() : {};
  
  // Preenche campos...
  document.getElementById('cfgTitle').value = site.title || 'CRIMSON FACTIONS';
  // ... outros campos
}

async function saveSiteConfig() {
  const data = {
    title: document.getElementById('cfgTitle').value,
    subtitle: document.getElementById('cfgSubtitle').value,
    accentColor: document.getElementById('cfgColor').value,
    factions: currentFactionsArray, // gerenciado dinamicamente
    minAge: parseInt(document.getElementById('cfgMinAge').value || 16),
    minRP: parseInt(document.getElementById('cfgMinRP').value || 3),
    discordWebhookUrl: document.getElementById('cfgWebhookUrl').value,
    // etc.
  };
  await setDoc(doc(db,'config','site'), data, {merge: true});
  toast('✅ Configurações salvas com sucesso!');
}

// Inicialização
router();
</script>
</body>
</html>
