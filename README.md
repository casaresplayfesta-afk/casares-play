<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>CasaRes Play - Aluguel de Máquina de Pelúcia</title>
  <style>
    :root {
      --accent: #ff6b6b;
      --dark: #0f1724;
      --muted: #6b7280;
    }
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body {
      font-family: Inter, system-ui, sans-serif;
      background: #f8fafc;
      color: #0b1220;
      line-height: 1.5;
    }

    .fundo {
      position: fixed; top: 0; left: 0;
      width: 100%; height: 100%;
      object-fit: cover; z-index: -1;
      opacity: 0.9; filter: brightness(0.7) blur(5px);
    }

    header {
      background: linear-gradient(90deg,var(--accent),#ff9a76);
      color: white; text-align: center;
      padding: 20px; position: fixed;
      top: 0; left: 0; right: 0;
      z-index: 1000; transition: top 0.4s ease;
    }
    header h1 { font-size: 24px; margin-bottom: 4px; }
    header .lead { font-size: 14px; opacity: .9; }

    .logo-container {
      display: flex; align-items: center; justify-content: center; gap: 10px;
    }
    .logo {
      width: 50px; height: 50px; border-radius: 50%;
      object-fit: cover; border: 2px solid white;
      box-shadow: 0 0 8px rgba(0,0,0,0.2);
    }

    main { padding: 140px 16px 40px; max-width: 1100px; margin: 0 auto; }

    h2.fundo-branco {
      background: #fff; display: inline-block;
      padding: 6px 12px; border-radius: 8px;
      margin-bottom: 16px; color: #111;
    }

    .pricing {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px,1fr));
      gap: 16px; margin-top: 16px;
    }
    .pkg {
      background: rgba(255,255,255,0.95);
      border-radius: 12px; padding: 16px;
      border: 1px solid #ddd;
      box-shadow: 0 5px 20px rgba(0,0,0,0.15);
      text-align: center; cursor: pointer;
      transition: transform 0.2s, box-shadow 0.2s;
    }
    .pkg:hover { transform: translateY(-3px); box-shadow:0 8px 25px rgba(0,0,0,0.25);}
    .pkg h3 { margin-bottom: 8px; }
    .price { font-size: 20px; color: var(--accent); font-weight: 700; margin: 8px 0; }
    .cta {
      display: inline-block;
      margin-top: 10px;
      padding: 10px 14px;
      border-radius: 10px;
      background: var(--accent);
      color: white;
      text-decoration: none;
      font-weight: 600;
      font-size: 14px;
      transition: 0.2s;
      box-shadow: 0 3px 10px rgba(0,0,0,0.2);
    }
    .cta:hover { opacity: 0.9; }

    /* Gaveta moderna */
    .gaveta-container {
      overflow: hidden;
      max-height: 0;
      transition: max-height 0.5s ease, box-shadow 0.5s ease;
      margin-top: 12px;
      border-radius: 12px;
      background: #fff;
      box-shadow: 0 0 0 rgba(0,0,0,0);
    }
    .gaveta-container.open { max-height: 120px; box-shadow: 0 8px 20px rgba(0,0,0,0.2); }

    .gaveta {
      display: flex; justify-content: center; align-items: center; gap: 8px;
      padding: 12px;
    }
    .gaveta button {
      width: 32px; height: 32px;
      border: 1px solid #ddd; background: #fff;
      font-size: 20px; line-height: 1; cursor: pointer;
      border-radius: 6px; transition: 0.2s;
    }
    .gaveta button:hover { background: var(--accent); color:#fff;}
    .gaveta input {
      width: 60px; text-align: center;
      border: 1px solid #ddd; border-radius: 6px; padding:4px;
      font-size: 14px;
    }

    .galeria {
      display: grid; grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
      gap:16px; margin-top:16px;
    }
    .galeria img {
      width:100%; height:230px; object-fit:cover;
      border-radius:12px; box-shadow:0 4px 15px rgba(0,0,0,0.15);
      cursor:pointer; transition: transform 0.3s;
    }
    .galeria img:hover { transform: scale(1.05); }

    .modal { display:none; position:fixed; z-index:2000; inset:0; background: rgba(0,0,0,0.9);}
    .modal-content { margin:auto; display:block; width:80%; max-width:700px; border-radius:10px;}
    .close { position:absolute; top:20px; right:35px; color:#fff; font-size:40px; cursor:pointer; }

    .floating-buttons { position:fixed; bottom:20px; right:20px; display:flex; gap:12px; z-index:10000;}
    .floating-buttons a { width:55px; height:55px; border-radius:50%; display:flex; align-items:center; justify-content:center; box-shadow:0 0 15px rgba(0,0,0,0.3); transition:0.2s;}
    .floating-buttons a:hover { transform: scale(1.1);}
    .instagram { background: radial-gradient(circle at 30% 107%, #fdf497 0%, #fd5949 45%, #d6249f 60%, #285AEB 90%); }

    footer { margin-top:30px; text-align:center; color:white; font-size:12px; }

    .avisos { margin-top:24px; background:#fff; border-radius:12px; padding:16px; box-shadow:0 4px 15px rgba(0,0,0,0.1);}
    .avisos h3 { margin-bottom:8px; color:var(--accent); }
    .avisos p, .avisos li { font-size:14px; margin-bottom:6px; }

  </style>
</head>
<body>
<img src="maquina.jpg" alt="máquina de pelúcia" class="fundo">

<header id="header">
  <div class="logo-container">
    <img src="logo.jpg" class="logo" alt="Logo CasaRes Play">
    <h1>CasaRes Play</h1>
  </div>
  <p class="lead">Aluguel de máquinas de pelúcia — diversão garantida nas festas!</p>
</header>

<main>
  <h2 class="fundo-branco">Pacotes com máquina (4 horas)</h2>
  <div class="pricing" id="pricing-container"></div>

  <h2 class="fundo-branco" style="margin-top:40px;">Fotos da Máquina</h2>
  <div class="galeria">
    <img src="maquina1.jpg" alt="Máquina 1">
    <img src="maquina2.jpg" alt="Máquina 2">
    <img src="maquina3.jpg" alt="Máquina 3">
  </div>

  <div class="avisos">
    <h3>Informações importantes</h3>
    <p>Tempo de locação: 4 horas. Caso precise de horário estendido ou transporte fora das regiões atendidas, entre em contato.</p>
    <h3>Onde entregamos</h3>
    <p>Paracambi, Seropédica, Japeri e Conrado — frete grátis nessas localidades.</p>
    <h3>Como reservar</h3>
    <ol>
      <li>Entre em contato por WhatsApp: <a href="https://wa.me/5521968884003" target="_blank">(21) 96888-4003</a>.</li>
      <li>Combine data, horário e endereço de entrega.</li>
      <li>Pagamento: na hora de receber a máquina.</li>
    </ol>
  </div>
</main>

<div class="floating-buttons">
  <a href="https://wa.me/5521968884003" target="_blank">
    <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" width="28">
  </a>
  <a href="https://www.instagram.com/diversao_em_festas_" target="_blank" class="instagram">
    <img src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Instagram_icon.png" width="28">
  </a>
</div>

<footer>
  <p>© CasaRes Play — Aluguel de máquinas de pelúcia.<br>Contato: (21) 96888-4003 — casaresplayfesta@gmail.com</p>
</footer>

<script>
const precoMaquina = 550;
const precoPorPelucia = 15;

const pacotes = [
  { nome:"Somente máquina", preco:550, itens:["Uso da máquina por 4 horas","Sem pelúcias inclusas","Frete grátis (Paracambi, Seropédica, Japeri, Conrado)"], whatsappMsg:"Olá, quero reservar apenas a máquina" },
  { nome:"30 pelúcias + máquina", preco:1000, itens:["30 pelúcias inclusas","Uso da máquina por 4 horas","Frete grátis"], whatsappMsg:"Olá, quero reservar o pacote de 30 pelúcias com máquina" },
  { nome:"50 pelúcias + máquina", preco:1300, itens:["50 pelúcias inclusas","Uso da máquina por 4 horas","Frete grátis"], whatsappMsg:"Olá, quero reservar o pacote de 50 pelúcias com máquina" },
  { nome:"80 pelúcias + máquina", preco:1750, itens:["80 pelúcias inclusas","Uso da máquina por 4 horas","Frete grátis"], whatsappMsg:"Olá, quero reservar o pacote de 80 pelúcias com máquina" },
  { nome:"Pacote Personalizado", preco:precoMaquina, itens:["Uso da máquina por 4 horas","Sem pelúcias inclusas","Frete grátis (Paracambi, Seropédica, Japeri, Conrado)"], personalizado:true }
];

const container = document.getElementById("pricing-container");

pacotes.forEach(p=>{
  const pkgDiv = document.createElement("div");
  pkgDiv.classList.add("pkg");

  if(p.personalizado){
    pkgDiv.innerHTML = `
      <h3>${p.nome}</h3>
      <div class="price" id="precoPersonalizado">R$ ${p.preco}</div>
      <ul>${p.itens.map(i=>`<li>${i}</li>`).join('')}</ul>
      <div class="gaveta-container">
        <div class="gaveta">
          <button id="menos">-</button>
          <input type="number" id="inputQtd" min="20" value="20">
          <button id="mais">+</button>
          <button id="addPelucias" style="padding:4px 8px; background:var(--accent); color:#fff; border:none; border-radius:6px;">+ Adicionar pelúcias</button>
        </div>
      </div>
      <a class="cta" id="btnPersonalizado">Reservar pelo WhatsApp</a>
    `;
    container.appendChild(pkgDiv);

    const gavetaContainer = pkgDiv.querySelector(".gaveta-container");
    pkgDiv.addEventListener("click", ()=>{ gavetaContainer.classList.toggle("open"); });

    const inputQtd = pkgDiv.querySelector("#inputQtd");
    const precoPersonalizado = pkgDiv.querySelector("#precoPersonalizado");
    const btnPersonalizado = pkgDiv.querySelector("#btnPersonalizado");
    const btnMais = pkgDiv.querySelector("#mais");
    const btnMenos = pkgDiv.querySelector("#menos");

    function atualizarPreco(){ 
      let qtd = parseInt(inputQtd.value);
      if(isNaN(qtd) || qtd<20) qtd=20; inputQtd.value=qtd;
      const total = precoMaquina + qtd*precoPorPelucia;
      precoPersonalizado.textContent = `R$ ${total}`;
    }

    inputQtd.addEventListener("input", atualizarPreco);
    btnMais.addEventListener("click", e=>{e.stopPropagation(); inputQtd.value=parseInt(inputQtd.value)+1; atualizarPreco();});
    btnMenos.addEventListener("click", e=>{e.stopPropagation(); inputQtd.value=parseInt(inputQtd.value)-1; atualizarPreco();});
    btnPersonalizado.addEventListener("click", e=>{
      e.stopPropagation();
      let qtd = parseInt(inputQtd.value); if(isNaN(qtd)||qtd<20) qtd=20;
      const total = precoMaquina + qtd*precoPorPelucia;
      const msg = `Olá! Quero reservar a máquina com ${qtd} pelúcias (total R$ ${total}).`;
      window.open(`https://wa.me/5521968884003?text=${encodeURIComponent(msg)}`,"_blank");
    });
    atualizarPreco();
  } else {
    pkgDiv.innerHTML = `
      <h3>${p.nome}</h3>
      <div class="price">R$ ${p.preco}</div>
      <ul>${p.itens.map(i=>`<li>${i}</li>`).join('')}</ul>
      <a class="cta" href="https://wa.me/5521968884003?text=${encodeURIComponent(p.whatsappMsg)}" target="_blank">Reservar pelo WhatsApp</a>
    `;
    container.appendChild(pkgDiv);
  }
});

// esconder header ao rolar
let lastScroll=0;
const header=document.getElementById("header");
window.addEventListener("scroll",()=>{const s=window.pageYOffset; header.style.top=(s>lastScroll && s>100)?"-100px":"0"; lastScroll=s;});

// Modal da galeria
const modal=do
