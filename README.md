<!doctype html>
<html lang="pt-BR">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>CasaRes Play - Aluguel de Máquina de Pelúcia</title>

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
  transition: transform 0.2s;
}
.pkg:hover { transform: translateY(-4px); }

.pkg .swiper { width: 100%; height: 230px; }
.pkg .swiper-slide img { width: 100%; height: 230px; object-fit: cover; }

.pkg-content { padding: 12px; flex-grow: 1; }
.pkg-content h3 { font-size: 18px; margin-bottom: 4px; }
.pkg-content .price { color: var(--accent); font-weight: bold; margin-bottom: 8px; }

.etiquetas { display: flex; flex-wrap: wrap; gap: 6px; margin-bottom: 10px; }
.etiqueta { background: #e5e7eb; color: #111; font-size: 12px; border-radius: 6px; padding: 4px 8px; font-weight: 500; }

.pkg-content ul { list-style: none; margin-bottom: 10px; }
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
</style>
</head>
<body>

<header>
  <h1>CasaRes Play</h1>
  <p>Aluguel de máquinas de pelúcia — diversão garantida nas festas!</p>
</header>

<main>
  <!-- AVISO DE INDISPONIBILIDADE -->
  <div class="aviso-indisponivel">
    ⚠️ No momento, a locação das máquinas está <strong>indisponível por tempo indeterminado</strong>.<br>
    Continue conferindo nossos pacotes e aproveite para comprar suas pelúcias!
  </div>

  <h2 class="fundo-branco">Pacotes com máquina (4 horas)</h2>
  <div class="pricing">
    <!-- PACOTE 1 -->
    <div class="pkg">
      <div class="swiper pacoteSwiper">
        <div class="swiper-wrapper">
          <div class="swiper-slide"><img src="maquina1.jpg" alt="Máquina 1"></div>
          <div class="swiper-slide"><img src="maquina2.jpg" alt="Máquina 2"></div>
        </div>
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
    <!-- PACOTE 2 -->
    <div class="pkg">
      <div class="swiper pacoteSwiper">
        <div class="swiper-wrapper">
          <div class="swiper-slide"><img src="maquina3.jpg" alt="Máquina 3"></div>
          <div class="swiper-slide"><img src="maquina4.jpg" alt="Máquina 4"></div>
        </div>
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
  <!-- VENDA DE PELÚCIAS -->
  <h2 class="fundo-branco" style="margin-top:40px;">Venda de Pelúcias 🧸</h2>
  <div class="pricing">
    <div class="pkg">
      <div class="swiper pacoteSwiper">
        <div class="swiper-wrapper">
          <div class="swiper-slide"><img src="peluci10a.jpg" alt="Pelúcia 1"></div>
          <div class="swiper-slide"><img src="peluci10b.jpg" alt="Pelúcia 2"></div>
        </div>
      </div>
      <div class="pkg-content">
        <h3>Pelucia Coelho Feisty Mal Humurado - Muda Face Marrom-claros</h3>
        <div class="price">R$ 150</div>
        <div class="etiquetas">
          <span class="etiqueta">Entrega Fácil</span>
          <span class="etiqueta">Frete Grátis</span>
        </div>
        <ul>
          <li>Pelúcia de alta qualidade</li>
          <li>Qualidade premium</li>
          <li>Envio combinado pelo WhatsApp</li>
        </ul>
        <a class="cta ativo" href="https://wa.me/5521968884003?text=Olá! Tenho interesse na *Pelúcia Coelho Feisty Mal Humorado - Muda Face Marrom-claro* do kit com 10 pelúcias por R$150." target="_blank">Comprar pelo WhatsApp</a>
      </div>
    </div>
    <div class="pkg">
      <div class="swiper pacoteSwiper">
        <div class="swiper-wrapper">
          <div class="swiper-slide"><img src="pelucia3.jpg" alt="Pelúcia 3"></div>
          <div class="swiper-slide"><img src="pelucia4.jpg" alt="Pelúcia 4"></div>
        </div>
      </div>
      <div class="pkg-content">
        <h3>Pelucia Coelho Feisty Mal Humurado - Muda Face Marrom-claros</h3>
        <div class="price">R$ 280</div>
        <div class="etiquetas">
          <span class="etiqueta">Entrega Fácil</span>
          <span class="etiqueta">Frete Grátis</span>
        </div>
        <ul>
          <li>Pelúcia de alta qualidade</li>
          <li>Alta qualidade e acabamento</li>
          <li>Envio combinado pelo WhatsApp</li>
        </ul>
        <a class="cta ativo" href="https://wa.me/5521968884003?text=Olá! Tenho interesse na *Pelúcia Coelho Feisty Mal Humorado - Muda Face Marrom-claro* do kit com 20 pelúcias por R$280." target="_blank">Comprar pelo WhatsApp</a>
      </div>
    </div>

  </div>
</main>

<footer>
  © CasaRes Play — Aluguel de máquinas de pelúcia.<br>
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
  });
});
</script>

</body>
</html>
