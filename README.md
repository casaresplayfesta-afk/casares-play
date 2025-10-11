<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>CasaRes Play - Aluguel de Máquina de Pelúcia</title>
  <style>
    /* Logo e nome */
    .logo-container {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
    }
    .logo {
      width: 50px;
      height: 50px;
      border-radius: 50%;
      object-fit: cover;
      border: 2px solid white;
      box-shadow: 0 0 8px rgba(0,0,0,0.2);
    }

    /* Fundo */
    .fundo {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      object-fit: cover;
      z-index: -1;
      opacity: 0.9;
      filter: brightness(0.7) blur(5px);
    }

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

    /* Cabeçalho */
    header {
      background: linear-gradient(90deg, var(--accent), #ff9a76);
      color: white;
      text-align: center;
      padding: 20px;
      position: fixed;
      top: 0; left: 0; right: 0;
      z-index: 1000;
      transition: top 0.4s ease;
    }
    header h1 { font-size: 24px; margin-bottom: 4px; }
    header .lead { font-size: 14px; opacity: .9; }

    main { padding: 140px 16px 40px; max-width: 1100px; margin: 0 auto; }

    /* Pacotes */
    .pricing {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px,1fr));
      gap: 16px;
    }

    .pkg {
      background: rgba(255,255,255,0.95);
      border-radius: 12px;
      padding: 16px;
      border: 1px solid #ddd;
      box-shadow: 0 5px 20px rgba(0,0,0,0.15);
      text-align: center;
    }

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

    /* Galeria */
    .galeria {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 16px;
      margin-top: 16px;
    }
    .galeria img {
      width: 100%;
      height: 230px;
      object-fit: cover;
      border-radius: 12px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.15);
      cursor: pointer;
      transition: transform 0.3s;
    }
    .galeria img:hover { transform: scale(1.05); }

    /* Modal da galeria */
    .modal { display: none; position: fixed; z-index: 2000; inset: 0; background: rgba(0,0,0,0.9); }
    .modal-content { margin: auto; display: block; width: 80%; max-width: 700px; border-radius: 10px; }
    .close { position: absolute; top: 20px; right: 35px; color: #fff; font-size: 40px; cursor: pointer; }

    /* Botões flutuantes */
    .floating-buttons {
      position: fixed;
      bottom: 20px; right: 20px;
      display: flex; gap: 12px;
      z-index: 10000;
    }
    .floating-buttons a {
      background-color: #25D366;
      width: 55px; height: 55px;
      border-radius: 50%;
      display: flex; align-items: center; justify-content: center;
      box-shadow: 0 0 15px rgba(0,0,0,0.3);
      transition: 0.2s;
    }
    .floating-buttons a:hover { transform: scale(1.1); }

    .instagram {
      background: radial-gradient(circle at 30% 107%, #fdf497 0%, #fd5949 45%, #d6249f 60%, #285AEB 90%);
    }

    footer { margin-top: 30px; text-align: center; color: white; font-size: 12px; }

    /* ======= Gaveta Shopee ======= */
    .overlay {
      display: none;
      position: fixed;
      inset: 0;
      background: rgba(0,0,0,0.6);
      z-index: 9998;
      transition: opacity 0.3s;
    }
    .drawer {
      position: fixed;
      bottom: -100%;
      left: 0; right: 0;
      background: #fff;
      border-radius: 20px 20px 0 0;
      padding: 20px;
      box-shadow: 0 -2px 15px rgba(0,0,0,0.3);
      transition: bottom 0.4s ease;
      z-index: 9999;
      max-height: 70%;
      overflow-y: auto;
    }
    .drawer.active { bottom: 0; }
    .overlay.active { display: block; }
    .drawer h3 { text-align: center; margin-bottom: 16px; color: #333; }
    .options {
      display: flex; justify-content: center; flex-wrap: wrap;
      gap: 10px; margin-bottom: 20px;
    }
    .option {
      padding: 10px 18px; border-radius: 30px; border: 2px solid #ff6b6b;
      color: #ff6b6b; background: #fff; font-weight: 600; cursor: pointer;
      transition: all 0.2s;
    }
    .option:hover, .option.selected { background: #ff6b6b; color: #fff; }
    .confirmar {
      display: block; width: 100%;
      background: linear-gradient(90deg,#ff6b6b,#ff9a76);
      color: #fff; border: none; border-radius: 10px;
      padding: 14px; font-size: 16px; font-weight: bold;
      cursor: pointer;
    }
    .confirmar:hover { opacity: .9; }
  </style>
</head>
<body>
  <img src="maquina.jpg" alt="máquina de pelúcia" class="fundo">

  <header id="header">
    <div class="logo-container">
      <img src="logo.jpg" class="logo">
      <h1>CasaRes Play</h1>
    </div>
    <p class="lead">Aluguel de máquinas de pelúcia — diversão garantida nas festas!</p>
  </header>

  <main>
    <h2>Pacotes com máquina (4 horas)</h2>
    <div class="pricing" id="pricing-container"></div>

    <h2 style="margin-top:40px;">Fotos da Máquina</h2>
    <div class="galeria">
      <img src="maquina1.jpg">
      <img src="maquina2.jpg">
      <img src="maquina3.jpg">
    </div>

    <div id="imagemModal" class="modal">
      <span class="close">&times;</span>
      <img class="modal-content" id="imgAmpliada">
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

  <!-- Fundo escuro e gaveta -->
  <div class="overlay"></div>
  <div class="drawer" id="drawer">
    <h3>Escolha a quantidade de pelúcias</h3>
    <div class="options">
      <div class="option" data-qtd="30">30 pelúcias</div>
      <div class="option" data-qtd="50">50 pelúcias</div>
      <div class="option" data-qtd="80">80 pelúcias</div>
      <div class="option" data-qtd="100">100 pelúcias</div>
    </div>
    <button class="confirmar">Confirmar reserva</button>
  </div>

  <script>
    // Pacotes
    const pacotes = [
      { nome: "Somente máquina", preco: "R$ 500", itens: ["Uso da máquina por 4 horas", "Sem pelúcias inclusas"], tipo: "somente" },
      { nome: "Máquina + pelúcias", preco: "Personalizado", itens: ["Escolha a quantidade na reserva"], tipo: "com" }
    ];
    const container = document.getElementById("pricing-container");
    pacotes.forEach(p => {
      const pkgDiv = document.createElement("div");
      pkgDiv.classList.add("pkg");
      pkgDiv.innerHTML = `
        <h3>${p.nome}</h3>
        <div class="price">${p.preco}</div>
        <ul>${p.itens.map(i => `<li>${i}</li>`).join('')}</ul>
        <a href="#" class="cta reservar" data-tipo="${p.tipo}">Reservar pelo WhatsApp</a>
      `;
      container.appendChild(pkgDiv);
    });

    // Gaveta moderna
    const overlay = document.querySelector(".overlay");
    const drawer = document.getElementById("drawer");
    const options = document.querySelectorAll(".option");
    const confirmar = document.querySelector(".confirmar");
    let selecionado = null;
    let tipoPacote = null;

    document.querySelectorAll(".reservar").forEach(btn => {
      btn.addEventListener("click", e => {
        e.preventDefault();
        tipoPacote = btn.dataset.tipo;
        if (tipoPacote === "somente") {
          const msg = "Olá, quero reservar somente a máquina de pelúcia (sem pelúcias inclusas).";
          window.open(`https://wa.me/5521968884003?text=${encodeURIComponent(msg)}`, "_blank");
          return;
        }
        overlay.classList.add("active");
        drawer.classList.add("active");
      });
    });

    overlay.addEventListener("click", () => {
      overlay.classList.remove("active");
      drawer.classList.remove("active");
      selecionado = null;
      options.forEach(o => o.classList.remove("selected"));
    });

    options.forEach(opt => {
      opt.addEventListener("click", () => {
        options.forEach(o => o.classList.remove("selected"));
        opt.classList.add("selected");
        selecionado = opt.dataset.qtd;
      });
    });

    confirmar.addEventListener("click", () => {
      if (!selecionado) {
        alert("Selecione uma quantidade de pelúcias.");
        return;
      }
      const msg = `Olá! Quero reservar a máquina com ${selecionado} pelúcias.`;
      window.open(`https://wa.me/5521968884003?text=${encodeURIComponent(msg)}`, "_blank");
      overlay.classList.remove("active");
      drawer.classList.remove("active");
    });

    // Modal imagens
    const modal = document.getElementById("imagemModal");
    const modalImg = document.getElementById("imgAmpliada");
    const closeBtn = document.querySelector(".close");
    document.querySelectorAll(".galeria img").forEach(img => {
      img.addEventListener("click", () => {
        modal.style.display = "block";
        modalImg.src = img.src;
      });
    });
    closeBtn.onclick = () => modal.style.display = "none";
    window.onclick = e => { if (e.target === modal) modal.style.display = "none"; };
  </script>
</body>
</html>
