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

    /* Botão flutuante WhatsApp premium */
    .whatsapp-premium {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: #25D366;
      color: white;
      padding: 16px 20px;
      border-radius: 50px;
      text-decoration: none;
      font-weight: bold;
      display: flex;
      align-items: center;
      gap: 10px;
      z-index: 10000;
      box-shadow: 0 0 20px rgba(37, 211, 102, 0.6);
      animation: glowPulse 2s infinite;
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .whatsapp-premium img {
      width: 26px;
      height: 26px;
    }

    .whatsapp-premium:hover {
      transform: scale(1.15);
      box-shadow: 0 0 30px rgba(37, 211, 102, 0.9), 0 0 40px rgba(37, 211, 102, 0.6);
    }

    @keyframes glowPulse {
      0% { transform: scale(1); box-shadow: 0 0 20px rgba(37, 211, 102, 0.6); }
      50% { transform: scale(1.1); box-shadow: 0 0 30px rgba(37, 211, 102, 0.8); }
      100% { transform: scale(1); box-shadow: 0 0 20px rgba(37, 211, 102, 0.6); }
    }
  </style>
</head>
<body>
  <header>
    <h1>CasaRes Play</h1>
    <p class="lead">Aluguel de máquinas de pelúcia — diversão garantida nas festas!</p>
  </header>

  <main>
    <h2>Pacotes com máquina (4 horas)</h2>
    <div class="pricing">
      <div class="pkg">
        <h3>30 pelúcias + máquina</h3>
        <div class="price">R$ 1.000</div>
        <ul>
          <li>30 pelúcias inclusas</li>
          <li>Uso da máquina por 4 horas</li>
          <li>Frete grátis (Paracambi, Seropédica, Japeri, Conrado)</li>
        </ul>
        <a class="cta" href="https://wa.me/5521968884003?text=Olá,%20quero%20reservar%20o%20pacote%20de%2030%20pelúcias%20com%20máquina" target="_blank">Reservar pelo WhatsApp</a>
      </div>

      <div class="pkg">
        <h3>50 pelúcias + máquina</h3>
        <div class="price">R$ 1.300</div>
        <ul>
          <li>50 pelúcias inclusas</li>
          <li>Uso da máquina por 4 horas</li>
          <li>Frete grátis (Paracambi, Seropédica, Japeri, Conrado)</li>
        </ul>
        <a class="cta" href="https://wa.me/5521968884003?text=Olá,%20quero%20reservar%20o%20pacote%20de%2050%20pelúcias%20com%20máquina" target="_blank">Reservar pelo WhatsApp</a>
      </div>

      <div class="pkg">
        <h3>80 pelúcias + máquina</h3>
        <div class="price">R$ 1.750</div>
        <ul>
          <li>80 pelúcias inclusas</li>
          <li>Uso da máquina por 4 horas</li>
          <li>Frete grátis (Paracambi, Seropédica, Japeri, Conrado)</li>
        </ul>
        <a class="cta" href="https://wa.me/5521968884003?text=Olá,%20quero%20reservar%20o%20pacote%20de%2080%20pelúcias%20com%20máquina" target="_blank">Reservar pelo WhatsApp</a>
      </div>

      <div class="pkg">
        <h3>Somente máquina</h3>
        <div class="price">R$ 500</div>
        <ul>
          <li>Uso da máquina por 4 horas</li>
          <li>Sem pelúcias inclusas</li>
          <li>Frete grátis (Paracambi, Seropédica, Japeri, Conrado)</li>
        </ul>
        <a class="cta" href="https://wa.me/5521968884003?text=Olá,%20quero%20reservar%20apenas%20a%20máquina" target="_blank">Reservar pelo WhatsApp</a>
      </div>
    </div>

    <section class="details">
      <div>
        <h2>Informações importantes</h2>
        <p>Tempo de locação: 4 horas. Caso precise de horário estendido ou transporte fora das regiões atendidas, entre em contato.</p>

        <h3 style="margin-top:12px">Onde entregamos</h3>
        <p>Paracambi, Seropédica, Japeri e Conrado — frete grátis nessas localidades.</p>

        <h3 style="margin-top:12px">Como reservar</h3>
        <ol>
          <li>Entre em contato por WhatsApp: <a href="https://wa.me/5521968884003" target="_blank">(21) 96888-4003</a>.</li>
          <li>Combine data, horário e endereço de entrega.</li>
          <li>Pagamento: na hora de receber a máquina.</li>
        </ol>
      </div>

      <aside class="contact-card">
        <h3>Contato</h3>
        <div class="contact-line"><strong>WhatsApp:</strong> <a href="https://wa.me/5521968884003" target="_blank">(21) 96888-4003</a></div>
        <div class="contact-line"><strong>E‑mail:</strong> <a href="mailto:casaresplayfesta@gmail.com">casaresplayfesta@gmail.com</a></div>
        <p style="font-size:13px;color:var(--muted);margin-top:6px">Atendimento para Paracambi, Seropédica, Japeri e Conrado. Frete grátis.</p>
      </aside>
    </section>
  </main>

  <!-- Botão flutuante WhatsApp premium -->
  <a href="https://wa.me/5521968884003?text=Olá,%20quero%20mais%20informações%20sobre%20o%20aluguel%20da%20máquina%20de%20pelúcia" 
     target="_blank" 
     class="whatsapp-premium">
     <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" alt="WhatsApp">
     WhatsApp
  </a>

  <footer>
    <p>© CasaRes Play — Aluguel de máquinas de pelúcia.<br>Contato: (21) 96888-4003 — casaresplayfesta@gmail.com</p>
  </footer>
</body>
</html>

    
  </style>
</head>
<body>
  <header>
    <h1>CasaRes Play</h1>
    <p class="lead">Aluguel de máquinas de pelúcia — diversão garantida nas festas!</p>
  </header>

  <main>
    <h2>Pacotes com máquina (4 horas)</h2>
    <div class="pricing">
      <div class="pkg">
        <h3>30 pelúcias + máquina</h3>
        <div class="price">R$ 1.000</div>
        <ul>
          <li>30 pelúcias inclusas</li>
          <li>Uso da máquina por 4 horas</li>
          <li>Frete grátis (Paracambi, Seropédica, Japeri, Conrado)</li>
        </ul>
        <a class="cta" href="https://wa.me/5521968884003?text=Olá,%20quero%20reservar%20o%20pacote%20de%2030%20pelúcias%20com%20máquina" target="_blank">Reservar pelo WhatsApp</a>
      </div>

      <div class="pkg">
        <h3>50 pelúcias + máquina</h3>
        <div class="price">R$ 1.300</div>
        <ul>
          <li>50 pelúcias inclusas</li>
          <li>Uso da máquina por 4 horas</li>
          <li>Frete grátis (Paracambi, Seropédica, Japeri, Conrado)</li>
        </ul>
        <a class="cta" href="https://wa.me/5521968884003?text=Olá,%20quero%20reservar%20o%20pacote%20de%2050%20pelúcias%20com%20máquina" target="_blank">Reservar pelo WhatsApp</a>
      </div>

      <div class="pkg">
        <h3>80 pelúcias + máquina</h3>
        <div class="price">R$ 1.750</div>
        <ul>
          <li>80 pelúcias inclusas</li>
          <li>Uso da máquina por 4 horas</li>
          <li>Frete grátis (Paracambi, Seropédica, Japeri, Conrado)</li>
        </ul>
        <a class="cta" href="https://wa.me/5521968884003?text=Olá,%20quero%20reservar%20o%20pacote%20de%2080%20pelúcias%20com%20máquina" target="_blank">Reservar pelo WhatsApp</a>
      </div>

      <div class="pkg">
        <h3>Somente máquina</h3>
        <div class="price">R$ 500</div>
        <ul>
          <li>Uso da máquina por 4 horas</li>
          <li>Sem pelúcias inclusas</li>
          <li>Frete grátis (Paracambi, Seropédica, Japeri, Conrado)</li>
        </ul>
        <a class="cta" href="https://wa.me/5521968884003?text=Olá,%20quero%20reservar%20apenas%20a%20máquina" target="_blank">Reservar pelo WhatsApp</a>
      </div>
    </div>

    <section class="details">
      <div>
        <h2>Informações importantes</h2>
        <p>Tempo de locação: 4 horas. Caso precise de horário estendido ou transporte fora das regiões atendidas, entre em contato.</p>

        <h3 style="margin-top:12px">Onde entregamos</h3>
        <p>Paracambi, Seropédica, Japeri e Conrado — frete grátis nessas localidades.</p>

        <h3 style="margin-top:12px">Como reservar</h3>
        <ol>
          <li>Entre em contato por WhatsApp: <a href="https://wa.me/5521968884003" target="_blank">(21) 96888-4003</a>.</li>
          <li>Combine data, horário e endereço de entrega.</li>
          <li>Pagamento: na hora de receber a máquina.</li>
        </ol>
      </div>

      <aside class="contact-card">
        <h3>Contato</h3>
        <div class="contact-line"><strong>WhatsApp:</strong> <a href="https://wa.me/5521968884003" target="_blank">(21) 96888-4003</a></div>
        <div class="contact-line"><strong>E‑mail:</strong> <a href="mailto:casaresplayfesta@gmail.com">casaresplayfesta@gmail.com</a></div>
        <p style="font-size:13px;color:var(--muted);margin-top:6px">Atendimento para Paracambi, Seropédica, Japeri e Conrado. Frete grátis.</p>
      </aside>
    </section>
  </main>

  <!-- Botão flutuante WhatsApp premium -->
  <a href="https://wa.me/5521968884003?text=Olá,%20quero%20mais%20informações%20sobre%20o%20aluguel%20da%20máquina%20de%20pelúcia" 
     target="_blank" 
     class="whatsapp-premium">
     <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" alt="WhatsApp">
     WhatsApp
  </a>

  <footer>
    <p>© CasaRes Play — Aluguel de máquinas de pelúcia.<br>Contato: (21) 96888-4003 — casaresplayfesta@gmail.com</p>
  </footer>
</body>
</html>

