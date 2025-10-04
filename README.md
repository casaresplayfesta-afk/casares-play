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
      --card: #ffffff;
    }
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body { font-family: Inter, system-ui, Segoe UI, Roboto, Helvetica, Arial, sans-serif; background: #f8fafc; color: #0b1220; line-height: 1.5; letter-spacing: 0.5px; -webkit-font-smoothing: antialiased; }

    header {
      background: linear-gradient(90deg, var(--accent), #ff9a76);
      color: white; text-align: center; padding: 20px 12px;
      position: fixed; top: 0; left: 0; right: 0; z-index: 1000;
      box-shadow: 0 2px 8px rgba(0,0,0,0.15);
    }
    header h1 { font-size: 24px; margin-bottom: 4px; }
    header .lead { font-size: 14px; color: #fff; opacity: .9; }

    main { padding: 120px 16px 40px; max-width: 1100px; margin: 0 auto; }

    h2 { font-size: 20px; margin-bottom: 10px; color: var(--dark); }

    .pricing {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px,1fr));
      gap: 16px;
      margin-top: 16px;
    }
    .pkg {
      background: white; border-radius: 12px; padding: 16px; border: 1px solid #eef2f6; text-align: center;
      box-shadow: 0 3px 12px rgba(0,0,0,0.06); transition: 0.3s;
    }
    .pkg:hover { transform: translateY(-4px); box-shadow: 0 6px 16px rgba(0,0,0,0.12); }
    .pkg h3 { margin: 0 0 6px; font-size: 16px; color: #111; }
    .price { font-size: 20px; color: var(--accent); font-weight: 700; margin-bottom: 8px; }
    .pkg ul { padding-left: 18px; margin: 8px 0; text-align: left; font-size: 14px; color: #444; }

    .cta {
      display: inline-block; margin-top: 10px; padding: 10px 14px; border-radius: 10px;
      background: var(--accent); color: white; text-decoration: none; font-weight: 600; font-size: 14px; transition: 0.2s;
    }
    .cta:hover { opacity: 0.9; }

    .details {
      display: grid; grid-template-columns: 2fr 1fr; gap: 18px; margin-top: 24px;
    }
    .contact-card {
      background: #fff; padding: 16px; border-radius: 12px; border: 1px solid #eef2f6;
      box-shadow: 0 2px 10px rgba(0,0,0,0.05);
    }
    .contact-card h3 { margin-bottom: 6px; color: var(--accent); }
    .contact-line { margin: 6px 0; font-size: 14px; }
    .contact-line a { text-decoration: none; color: var(--dark); }
    .contact-line a:hover { color: var(--accent); text-decoration: underline; }

    footer { margin-top: 30px; padding: 14px; text-align: center; color: var(--muted); font-size: 12px; }

    @media (max-width:700px){
      .details{ grid-template-columns: 1fr; }
      .pricing { gap: 20px; }
    }
<!-- Botões flutuantes WhatsApp + Instagram -->
  <style>
    /* (estilos que te mandei aqui) */
  </style>

  <div class="floating-buttons">
    <!-- Botão WhatsApp -->
    <a href="https://wa.me/5521968884003?text=Olá,%20quero%20mais%20informações%20sobre%20o%20aluguel%20da%20máquina%20de%20pelúcia" target="_blank">
      <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" alt="WhatsApp">
    </a>

    <!-- Botão Instagram -->
    <a href="https://www.instagram.com/diversao_em_festas_?utm_source=ig_web_button_share_sheet&igsh=c3U2a2xudTFibTE5" 
       target="_blank" class="instagram">
      <img src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Instagram_icon.png" alt="Instagram">
    </a>
  </div>

  <footer>
    <p>© CasaRes Play — Aluguel de máquinas de pelúcia.<br>Contato: (21) 96888-4003 — casaresplayfesta@gmail.com</p>
  </footer>
