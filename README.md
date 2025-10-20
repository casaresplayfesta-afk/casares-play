<!doctype html>
<html lang="pt-BR">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>CasaRes Play - Aluguel e Venda de Pelúcias</title>

<!-- Swiper CSS -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css"/>

<style>
:root { --accent:#ff6b6b; --dark:#0f1724; --muted:#6b7280; }
*{box-sizing:border-box;margin:0;padding:0;}
body{font-family:Inter,sans-serif;background:#f8fafc;color:#0b1220;line-height:1.5;}
.fundo{position:fixed;top:0;left:0;width:100%;height:100%;object-fit:cover;z-index:-1;opacity:0.9;filter:brightness(0.7) blur(5px);}
header{background:linear-gradient(90deg,var(--accent),#ff9a76);color:white;text-align:center;padding:20px;position:fixed;top:0;left:0;right:0;z-index:1000;transition:top 0.4s ease;}
header h1{font-size:24px;margin-bottom:4px;}
header .lead{font-size:14px;opacity:.9;}
.logo-container{display:flex;align-items:center;justify-content:center;gap:10px;}
.logo{width:50px;height:50px;border-radius:50%;object-fit:cover;border:2px solid white;box-shadow:0 0 8px rgba(0,0,0,0.2);}
main{padding:180px 16px 40px;max-width:1100px;margin:0 auto;}
.aviso-indisponivel{background:#fff3cd;color:#856404;border:1px solid #ffeeba;padding:12px 16px;border-radius:10px;text-align:center;margin:20px auto;max-width:800px;box-shadow:0 3px 10px rgba(0,0,0,0.1);}
h2.fundo-branco{background:#fff;display:inline-block;padding:6px 12px;border-radius:8px;margin-bottom:16px;color:#111;}
.pricing{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:16px;margin-top:16px;}
.pkg{background:rgba(255,255,255,0.95);border-radius:12px;padding:16px;border:1px solid #ddd;
box-shadow:0 5px 20px rgba(0,0,0,0.15);text-align:center;display:flex;flex-direction:column;
justify-content:space-between;min-height:480px;}
.pkg:hover{transform:translateY(-3px);box-shadow:0 8px 25px rgba(0,0,0,0.25);}
.pkg h3{margin-bottom:8px;}
.price{font-size:20px;color:var(--accent);font-weight:700;margin:8px 0;}
.cta{display:inline-block;margin-top:auto;padding:10px 14px;border-radius:10px;background:var(--accent);
color:white;text-decoration:none;font-weight:600;font-size:14px;transition:0.2s;box-shadow:0 3px 10px rgba(0,0,0,0.2);}
.cta.disabled{background:#ccc;cursor:not-allowed;box-shadow:none;}
.cta:hover:not(.disabled){opacity:0.9;}
.swiper{width:100%;height:200px;margin:10px 0;}
.swiper-slide img{width:100%;height:200px;object-fit:cover;border-radius:10px;}
.swiper-pagination{bottom:5px !important;}
.modal{display:none;position:fixed;z-index:2000;inset:0;background:rgba(0,0,0,0.9);}
.modal-content{margin:auto;display:block;width:80%;max-width:700px;border-radius:10px;}
.close{position:absolute;top:20px;right:35px;color:#fff;font-size:40px;cursor:pointer;}
.floating-buttons{position:fixed;bottom:20px;right:20px;display:flex;gap:12px;z-index:10000;}
.floating-buttons a{width:55px;height:55px;border-radius:50%;display:flex;align-items:center;justify-content:center;
box-shadow:0 4px 15px rgba(0,0,0,0.25);transition:transform 0.2s, box-shadow 0.2s;}
.floating-buttons a img{width:28px;height:28px;}
.floating-buttons a:hover{transform:scale(1.1);box-shadow:0 0 25px rgba(0,0,0,0.5);}
.floating-buttons a.whatsapp{background:#25D366;}
.floating-buttons a.instagram{background:radial-gradient(circle at 30% 107%,#fdf497 0%,#fd5949 45%,#d6249f 60%,#285AEB 90%);}
footer{margin-top:30px;text-align:center;color:white;font-size:12px;}
.avisos{margin-top:24px;background:#fff;border-radius:12px;padding:16px;box-shadow:0 4px 15px rgba(0,0,0,0.1);}
.avisos h3{margin-bottom:8px;color:var(--accent);}
.avisos p, .avisos li{font-size:14px;margin-bottom:6px;}
</style>
</head>
<body>
<img src="maquina.jpg" alt="máquina de pelúcia" class="fundo">

<header id="header">
<div class="logo-container">
<img src="logo.jpg" class="logo" alt="Logo CasaRes Play">
<h1>CasaRes Play</h1>
</div>
<p class="lead">Aluguel e venda de pelúcias — diversão garantida nas festas!</p>
</header>

<main>
<div class="aviso-indisponivel">
🚫 <strong>AVISO IMPORTANTE:</strong> A locação de máquinas está temporariamente <strong>indisponível por tempo indeterminado</strong>.<br>
Os pacotes abaixo estão apenas para visualização.<br>
Mas você ainda pode comprar pelúcias conosco! 🧸
</div>

<h2 class="fundo-branco">Pacotes com máquina (4 horas)</h2>
<div class="pricing" id="pricing-container"></div>

<h2 class="fundo-branco" style="margin-top:40px;">Venda de Pelúcias 🧸</h2>
<div class="pricing">
  <div class="pkg">
    <h3>Pelucia Coelho Feisty Mal Humurado - Muda Face Marrom-claro</h3>
    <div class="price">R$ 150</div>
    <ul>
      <li>Pelúcia de alta qualidade</li>
      <li>Entrega combinada via WhatsApp</li>
      <li>Frete grátis para Paracambi, Seropédica, Japeri e Conrado</li>
    </ul>
    <div class="swiper">
      <div class="swiper-wrapper">
        <div class="swiper-slide"><img src="pelucia10a.jpg" alt=""></div>
        <div class="swiper-slide"><img src="pelucia10b.jpg" alt=""></div>
      </div>
      <div class="swiper-pagination"></div>
    </div>
    <a class="cta" href="https://wa.me/5521968884003?text=Olá! Quero comprar a Pelucia Coelho Feisty Mal Humurado - Muda Face Marrom-claro por R$150." target="_blank">Comprar pelo WhatsApp</a>
  </div>

  <div class="pkg">
    <h3>Pelucia Coelho Feisty Mal Humurado - Muda Face Marrom-claros</h3>
    <div class="price">R$ 280</div>
    <ul>
      <li>Pelúcia de alta qualidade</li>
      <li>Entrega combinada via WhatsApp</li>
      <li>Frete grátis nas cidades atendidas</li>
    </ul>
    <div class="swiper">
      <div class="swiper-wrapper">
        <div class="swiper-slide"><img src="pelucia20a.jpg" alt=""></div>
        <div class="swiper-slide"><img src="pelucia20b.jpg" alt=""></div>
      </div>
      <div class="swiper-pagination"></div>
    </div>
    <a class="cta" href="https://wa.me/5521968884003?text=Olá! Quero comprar o kit com 20 pelúcias por R$280." target="_blank">Comprar pelo WhatsApp</a>
  </div>
</div>

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
<h3>Como comprar</h3>
<ol>
<li>Entre em contato por WhatsApp: <a href="https://wa.me/5521968884003" target="_blank">(21) 96888-4003</a>.</li>
<li>Combine o kit e o endereço de entrega.</li>
<li>Pagamento: na hora da entrega.</li>
</ol>
</div>
</main>

<div class="floating-buttons">
<a href="https://wa.me/5521968884003" target="_blank" class="whatsapp">
<img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" alt="WhatsApp">
</a>
<a href="https://www.instagram.com/diversao_em_festas_" target="_blank" class="instagram">
<img src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Instagram_icon.png" alt="Instagram">
</a>
</div>

<footer>
<p>© CasaRes Play — Aluguel e venda de pelúcias.<br>Contato: (21) 96888-4003 — casaresplayfesta@gmail.com</p>
</footer>

<!-- Swiper JS -->
<script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>

<script>
// Pacotes de máquina (somente visualização)
const pacotes=[
  { nome:"Somente máquina", preco:550,itens:["Uso da máquina por 4 horas","Sem pelúcias inclusas","Frete grátis"], fotos:["pelucia-base1.jpg","pelucia-base2.jpg"] },
  { nome:"30 pelúcias + máquina", preco:1000,itens:["30 pelúcias inclusas","Uso da máquina por 4 horas","Frete grátis"], fotos:["pelucia30a.jpg","pelucia30b.jpg"] },
  { nome:"50 pelúcias + máquina", preco:1300,itens:["50 pelúcias inclusas","Uso da máquina por 4 horas","Frete grátis"], fotos:["pelucia50a.jpg","pelucia50b.jpg"] },
  { nome:"80 pelúcias + máquina", preco:1750,itens:["80 pelúcias inclusas","Uso da máquina por 4 horas","Frete grátis"], fotos:["pelucia80a.jpg","pelucia80b.jpg"] }
];
const container=document.getElementById("pricing-container");
pacotes.forEach((p,i)=>{
  const pkg=document.createElement("div");
  pkg.className="pkg";
  pkg.innerHTML=`
    <h3>${p.nome}</h3>
    <div class="price">R$ ${p.preco}</div>
    <ul>${p.itens.map(i=>`<li>${i}</li>`).join('')}</ul>
    <div class="swiper pacote-swiper-${i}">
      <div class="swiper-wrapper">
        ${p.fotos.map(f=>`<div class='swiper-slide'><img src='${f}'></div>`).join('')}
      </div>
      <div class="swiper-pagination"></div>
    </div>
    <a class="cta disabled">Indisponível</a>`;
  container.appendChild(pkg);
  new Swiper(`.pacote-swiper-${i}`,{
    loop:true,
    autoplay:{delay:5000},
    pagination:{el:".pacote-swiper-"+i+" .swiper-pagination",clickable:true},
  });
});

new Swiper(".swiper",{
  loop:true,
  autoplay:{delay:5000},
  pagination:{el:".swiper-pagination",clickable:true},
});

// Header oculto ao rolar
let lastScroll=0; const header=document.getElementById("header");
window.addEventListener("scroll",()=>{const s=window.pageYOffset;header.style.top=(s>lastScroll&&s>100)?"-100px":"0";lastScroll=s;});
</script>
</body>
</html>
