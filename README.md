<!doctype html>
<html lang="pt-BR">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>CasaRes Play - Aluguel e Venda de Pelúcias</title>

<!-- Swiper.js -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css"/>
<script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>

<style>
:root { --accent:#ff6b6b; --dark:#0f1724; --muted:#6b7280; }
*{box-sizing:border-box;margin:0;padding:0;}
body{font-family:Inter,sans-serif;background:#f8fafc;color:#0b1220;line-height:1.5;}
header{background:linear-gradient(90deg,var(--accent),#ff9a76);color:white;text-align:center;padding:20px;position:fixed;top:0;left:0;right:0;z-index:1000;}
header h1{font-size:24px;margin-bottom:4px;}
main{padding:140px 16px 40px;max-width:1100px;margin:0 auto;}
h2.fundo-branco{background:#fff;display:inline-block;padding:6px 12px;border-radius:8px;margin-bottom:16px;color:#111;}
.aviso-indisponivel{
  background:#fff3cd;
  border:1px solid #ffeeba;
  color:#856404;
  padding:16px;
  border-radius:12px;
  text-align:center;
  margin-bottom:30px;
  font-weight:600;
  box-shadow:0 4px 10px rgba(0,0,0,0.1);
}
.pricing{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:16px;}

.pkg {
  background: #fff;
  border-radius: 12px;
  box-shadow: 0 4px 15px rgba(0,0,0,0.15);
  overflow: hidden;
  display: flex;
  flex-direction: column;
  text-align:center;
  transition: transform 0.2s;
}
.pkg:hover { transform: translateY(-4px); }

.pkg .swiper { width: 100%; height: 230px; }
.pkg .swiper-slide img { width: 100%; height: 230px; object-fit: cover; }

.pkg-content { padding: 12px; flex-grow: 1; display:flex; flex-direction:column; justify-content:space-between;}
.pkg-content h3 { font-size: 18px; margin-bottom: 4px; }
.pkg-content .price { color: var(--accent); font-weight: bold; margin-bottom: 8px; }

.etiquetas { display: flex; flex-wrap: wrap; justify-content:center; gap: 6px; margin-bottom: 10px; }
.etiqueta { background: #e5e7eb; color:#111; font-size: 12px; border-radius: 6px; padding: 4px 8px; font-weight: 500; }

.pkg-content ul { list-style: none; margin-bottom: 10px; text-align:left; display:inline-block;}
.pkg-content ul li { font-size: 14px; margin-bottom: 4px; }

.cta {
  display: inline-block;
  margin-top: 8px;
  background: var(--accent);
  color: #fff;
  padding: 8px 12px;
  border-radius: 8px;
  text-decoration: none;
  font-weight: 600;
  text-align: center;
  cursor: not-allowed;
  opacity: 0.6;
}
.cta.ativo { cursor: pointer; opacity: 1; }
.cta:hover.ativo { opacity: 0.9; }

footer{margin-top:30px;text-align:center;color:#555;font-size:12px;}

.avisos{margin-top:40px;background:#fff;border-radius:12px;padding:16px;box-shadow:0 4px 15px rgba(0,0,0,0.1);}
.avisos h3{margin-bottom:8px;color:var(--accent);}
.avisos p, .avisos li{font-size:14px;margin-bottom:6px;}

.floating-buttons{position:fixed;bottom:20px;right:20px;display:flex;gap:12px;z-index:10000;}
.floating-buttons a{width:55px;height:55px;border-radius:50%;display:flex;align-items:center;justify-content:center;box-shadow:0 4px 15px rgba(0,0,0,0.25);transition:transform 0.2s, box-shadow 0.2s;}
.floating-buttons a img{width:28px;height:28px;}
.floating-buttons a:hover{transform:scale(1.1);box-shadow:0 0 25px rgba(0,0,0,0.5);}
.floating-buttons a.whatsapp{background:#25D366;}
.floating-buttons a.instagram{background: radial-gradient(circle at 30% 107%, #fdf497 0%, #fd5949 45%, #d6249f 60%, #285AEB 90%);}
</style>
</head>
<body>

<header>
  <h1>CasaRes Play</h1>
  <p>Aluguel e venda de pelúcias — diversão garantida nas festas!</p>
</header>

<main>

  <div class="aviso-indisponivel">
    🚫 <strong>AVISO IMPORTANTE:</strong> A locação de máquinas está temporariamente <strong>indisponível por tempo indeterminado</strong>.<br>
    Os pacotes abaixo estão apenas para visualização.<br>
    Mas você ainda pode comprar pelúcias conosco! 🧸
  </div>

  <h2 class="fundo-branco">Pacotes com máquina (4 horas)</h2>
  <div class="pricing">

    <div class="pkg">
      <div class="swiper pacoteSwiper">
        <div class="swiper-wrapper">
          <div class="swiper-slide"><img src="pelucia30a.jpg" alt="30 pelúcias - imagem 1"></div>
          <div class="swiper-slide"><img src="pelucia30b.jpg" alt="30 pelúcias - imagem 2"></div>
        </div>
        <div class="swiper-pagination"></div>
      </div>
      <div class="pkg-content">
        <h3>30 pelúcias + máquina</h3>
        <div class="price">R$ 1000</div>
        <div class="etiquetas">
          <span class="etiqueta">Frete Grátis</span>
          <span class="etiqueta">4 horas de uso</span>
        </div>
        <ul>
          <li>30 pelúcias inclusas</li>
          <li>Uso da máquina por 4 horas</li>
          <li>Frete grátis</li>
        </ul>
        <a class="cta">Indisponível no momento</a>
      </div>
    </div>

    <div class="pkg">
      <div class="swiper pacoteSwiper">
        <div class="swiper-wrapper">
          <div class="swiper-slide"><img src="pelucia50a.jpg" alt="50 pelúcias - imagem 1"></div>
          <div class="swiper-slide"><img src="pelucia50b.jpg" alt="50 pelúcias - imagem 2"></div>
        </div>
        <div class="swiper-pagination"></div>
      </div>
      <div class="pkg-content">
        <h3>50 pelúcias + máquina</h3>
        <div class="price">R$ 1300</div>
        <div class="etiquetas">
          <span class="etiqueta">Frete Grátis</span>
          <span class="etiqueta">4 horas de uso</span>
        </div>
        <ul>
          <li>50 pelúcias inclusas</li>
          <li>Uso da máquina por 4 horas</li>
          <li>Frete grátis</li>
        </ul>
        <a class="cta">Indisponível no momento</a>
      </div>
    </div>

  </div>

  <!-- NOVA SEÇÃO: PACOTE PERSONALIZADO -->
  <h2 class="fundo-branco" style="margin-top:40px;">Pacote Personalizado com Máquina 🧸</h2>
  <div class="pricing" id="personalizado-container"></div>

  <h2 class="fundo-branco" style="margin-top:40px;">Venda de Pelúcias 🧸</h2>
  <div class="pricing">

    <div class="pkg">
      <div class="swiper pacoteSwiper">
        <div class="swiper-wrapper">
          <div class="swiper-slide"><img src="pelucia10a.jpg" alt="Kit 10 pelúcias - 1"></div>
          <div class="swiper-slide"><img src="pelucia10b.jpg" alt="Kit 10 pelúcias - 2"></div>
        </div>
        <div class="swiper-pagination"></div>
      </div>
      <div class="pkg-content">
        <h3>Kit com 10 Pelúcias</h3>
        <div class="price">R$ 150</div>
        <div class="etiquetas">
          <span class="etiqueta">Entrega Fácil</span>
          <span class="etiqueta">Frete Grátis</span>
        </div>
        <ul>
          <li>10 pelúcias sortidas</li>
          <li>Qualidade premium</li>
          <li>Envio combinado pelo WhatsApp</li>
        </ul>
        <a class="cta ativo" href="https://wa.me/5521968884003?text=Olá! Quero comprar o *Kit com 10 Pelúcias* por R$150." target="_blank">Comprar pelo WhatsApp</a>
      </div>
    </div>

    <div class="pkg">
      <div class="swiper pacoteSwiper">
        <div class="swiper-wrapper">
          <div class="swiper-slide"><img src="pelucia20a.jpg" alt="Kit 20 pelúcias - 1"></div>
          <div class="swiper-slide"><img src="pelucia20b.jpg" alt="Kit 20 pelúcias - 2"></div>
        </div>
        <div class="swiper-pagination"></div>
      </div>
      <div class="pkg-content">
        <h3>Kit com 20 Pelúcias</h3>
        <div class="price">R$ 280</div>
        <div class="etiquetas">
          <span class="etiqueta">Entrega Fácil</span>
          <span class="etiqueta">Frete Grátis</span>
        </div>
        <ul>
          <li>20 pelúcias variadas</li>
          <li>Alta qualidade e acabamento</li>
          <li>Envio combinado pelo WhatsApp</li>
        </ul>
        <a class="cta ativo" href="https://wa.me/5521968884003?text=Olá! Quero comprar o *Kit com 20 Pelúcias* por R$280." target="_blank">Comprar pelo WhatsApp</a>
      </div>
    </div>

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
  © CasaRes Play — Aluguel e venda de pelúcias.<br>
  Contato: (21) 96888-4003 — casaresplayfesta@gmail.com
</footer>

<script>
document.querySelectorAll('.pacoteSwiper').forEach((swiperEl)=>{
  new Swiper(swiperEl, {
    loop: true,
    autoplay: {
      delay: 5000,
      disableOnInteraction: false,
    },
    slidesPerView: 1,
    spaceBetween: 0,
    pagination: {
      el: swiperEl.querySelector('.swiper-pagination'),
      clickable: true,
    },
  });
});

// ===== PACOTE PERSONALIZADO =====
const container = document.getElementById("personalizado-container");

const pkgDiv = document.createElement('div');
pkgDiv.classList.add('pkg');

// preços base
const precoMaquina = 550;  
const precoPorPelucia = 15; 

pkgDiv.innerHTML = `
  <div class="pkg-content">
    <h3>Monte seu pacote personalizado</h3>
    <p>Escolha quantas pelúcias deseja com a máquina.</p>
    <div style="margin:10px 0;">
      <button id="menos" style="padding:4px 8px;">-</button>
      <input type="number" id="inputQtd" value="20" min="20" style="width:50px;text-align:center;">
      <button id="mais" style="padding:4px 8px;">+</button>
      <span style="margin-left:10px;">pelúcias</span>
    </div>
    <div class="price" id="precoPersonalizado">R$ 0</div>
    <a class="cta ativo" id="btnPersonalizado">Reservar pelo WhatsApp</a>
  </div>
`;

container.appendChild(pkgDiv);

const inputQtd = pkgDiv.querySelector("#inputQtd");
const precoPersonalizado = pkgDiv.querySelector("#precoPersonalizado");
const btnPersonalizado = pkgDiv.querySelector("#btnPersonalizado");
const btnMais = pkgDiv.querySelector("#mais");
const btnMenos = pkgDiv.querySelector("#menos");

function atualizarPreco() {
  let qtd = parseInt(inputQtd.value);
  if (isNaN(qtd) || qtd < 20) qtd = 20;
  inputQtd.value = qtd;
  const total = precoMaquina + qtd * precoPorPelucia;
  precoPersonalizado.textContent = `R$ ${total}`;
}

inputQtd.addEventListener("input", atualizarPreco);
btnMais.addEventListener("click", () => {
  inputQtd.value = parseInt(inputQtd.value) + 1;
  atualizarPreco();
});
btnMenos.addEventListener("click", () => {
  inputQtd.value = parseInt(inputQtd.value) - 1;
  atualizarPreco();
});
btnPersonalizado.addEventListener("click", () => {
  let qtd = parseInt(inputQtd.value);
  if (isNaN(qtd) || qtd < 20) qtd = 20;
  const total = precoMaquina + qtd * precoPorPelucia;
  const msg = `Olá! Quero reservar a máquina com ${qtd} pelúcias (total R$ ${total}).`;
  window.open(`https://wa.me/5521968884003?text=${encodeURIComponent(msg)}`, "_blank");
});

atualizarPreco();
</script>

</body>
</html>
