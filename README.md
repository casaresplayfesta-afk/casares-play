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

    /* Imagem de fundo com blur */
    .fundo {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
      z-index: -1;
      opacity: 0.9;
      filter: brightness(0.7) blur(5px);
    }

    :root {
      --accent: #ff6b6b;
      --dark: #0f1724;
      --muted: #6b7280;
      --card: #ffffff;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }
    body {
      font-family: Inter, system-ui, Segoe UI, Roboto, Helvetica, Arial, sans-serif;
      background: #f8fafc;
      color: #0b1220;
      line-height: 1.5;
      letter-spacing: 0.5px;
      -webkit-font-smoothing: antialiased;
    }

    /* Cabeçalho fixo com efeito de esconder */
    header {
      background: linear-gradient(90deg, var(--accent), #ff9a76);
      color: white;
      text-align: center;
      padding: 20px 12px;
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      z-index: 1000;
      box-shadow: 0 2px 8px rgba(0,0,0,0.15);
      transition: transform 0.4s ease;
    }

    header.hide {
      transform: translateY(-100%);
    }

    header h1 { font-size: 24px; margin-bottom: 4px; }
    header .lead { font-size: 14px; color: #fff; opacity: .9; }

    main { padding: 140px 16px 40px; max-width: 1100px; margin: 0 auto; }

    h2.pacotes {
      background: rgba(255, 255, 255, 0.9);
      padding: 8px 16px;
      border-radius: 8px;
      display: inline-block;
      color: #111;
      text-shadow: 0 1px 2px rgba(255,255,255,0.6);
      margin-bottom: 16px;
    }

    h2, h3 { text-shadow: 0 1px 2px rgba(255,255,255,0.6); }
    h3 { color: var(--dark); }

    .pricing {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px,1fr));
      gap: 16px;
      margin-top: 16px;
    }

    .pkg {
      background: rgba(255,255,255,0.95);
      border-radius: 12px;
      padding: 16px;
      border: 1px solid #ddd;
      box-shadow: 0 5px 20px rgba(0,0,0,0.15);
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      align-items: center;
      text-align: center;
      min-height: 360px;
    }

    .pkg:hover { transform: translateY(-4px); box-shadow: 0 6px 16px rgba(0,0,0,0.2); }
    .pkg h3 { margin: 0 0 6px; font-size: 16px; }
    .price { font-size: 20px; color: var(--accent); font-weight: 700; margin-bottom: 8px; }

    .pkg ul {
      padding-left: 18px;
      margin: 8px 0;
      font-size: 14px;
      color: #111;
      text-align: left;
    }

    .cta {
      display: inline-block; margin-top: 10px; padding: 10px 14px; border-radius: 10px;
      background: var(--accent); color: white; text-decoration: none; font-weight: 600; font-size: 14px; transition: 0.2s;
      text-align: center;
      box-shadow: 0 3px 10px rgba(0,0,0,0.2);
    }
    .cta:hover { opacity: 0.9; }

    .details {
      display: grid; grid-template-columns: 2fr 1fr; gap: 18px; margin-top: 24px;
    }
    .details > div, .contact-card {
      background: rgba(255,255,255,0.95);
      border-radius: 12px;
      padding: 16px;
      border: 1px solid #ddd;
      box-shadow: 0 4px 15px rgba(0,0,0,0.1);
    }

    .contact-card h3 { margin-bottom: 6px; color: var(--accent); }
    .contact-line { margin: 6px 0; font-size: 14px; color: #111; }
    .contact-line a { text-decoration: none; color: var(--dark); }
    .contact-line a:hover { color: var(--accent); text-decoration: underline; }

    footer { margin-top: 30px; padding: 14px; text-align: center; color: var(--muted); font-size: 12px; }

    @media (max-width:700px){
      .details{ grid-template-columns: 1fr; }
      .pricing { gap: 20px; }
    }

    /* Botões flutuantes */
    .floating-buttons {
      position: fixed;
      bottom: 20px;
      right: 20px;
      display: flex;
      gap: 12px;
      z-index: 10000;
    }

    .floating-buttons a {
      background-color: #25D366;
      width: 55px;
      height: 55px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 0 15px rgba(0,0,0,0.3);
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .floating-buttons a img {
      width: 28px;
      height: 28px;
    }

    .floating-buttons a:hover {
      transform: scale(1.1);
      box-shadow: 0 0 25px rgba(0,0,0,0.5);
    }

    .floating-buttons .instagram {
      background: radial-gradient(circle at 30% 107%, #fdf497 0%, #fdf497 5%, #fd5949 45%, #d6249f 60%, #285AEB 90%);
    }
  </style>
</head>
<body>
  <!-- Imagem de fundo -->
  <img src="maquina.jpg" alt="máquina de pelúcia" class="fundo">

  <!-- Cabeçalho -->
  <header id="header">
    <div class="logo-container">
      <img src="logo.jpg" alt="Logo CasaRes Play" class="logo">
      <h1>CasaRes Play</h1>
    </div>
    <p class="lead">Aluguel de máquinas de pelúcia — diversão garantida nas festas!</p>
  </header>

  <main>
    <h2 class="pacotes">Pacotes com máquina (4 horas)</h2>
    <!-- Conteúdo principal aqui -->
  </main>

  <footer>
    <p>© CasaRes Play — Aluguel de máquinas de pelúcia.<br>Contato: (21) 96888-4003 — casaresplayfesta@gmail.com</p>
  </footer>

  <!-- Script para esconder e mostrar o topo dinamicamente -->
  <script>
    const header = document.getElementById("header");
    let lastScroll = 0;

    window.addEventListener("scroll", () => {
      const currentScroll = window.pageYOffset;

      if (currentScroll > lastScroll && currentScroll > 100) {
        // rolando para baixo -> esconder o topo
        header.classList.add("hide");
      } else {
        // rolando para cima -> mostrar o topo
        header.classList.remove("hide");
      }

      lastScroll = currentScroll;
    });
  </script>
</body>
</html>
