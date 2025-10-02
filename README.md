<html lang="pt-BR">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>CasaRes Play - Aluguel de Máquina de Pelúcia</title>
  <style>
    :root{
      --accent:#ff6b6b;
      --dark:#0f1724;
      --muted:#6b7280;
      --card:#ffffff;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family:Inter,system-ui,Segoe UI,Roboto,Helvetica,Arial,sans-serif;
      background:linear-gradient(180deg,#f8fafc 0%, #eef2f7 100%);
      color:#0b1220;
      -webkit-font-smoothing:antialiased
    }
    header{
      background:linear-gradient(90deg,#ff6b6b,#f9c74f,#43aa8b,#577590);
      color:white;
      padding:36px 18px;
      text-align:center;
      position:sticky;
      top:0;
      z-index:1000;
      box-shadow:0 4px 12px rgba(0,0,0,0.15);
    }
    .container{max-width:1000px;margin:0 auto;padding:24px}
    h1{
      margin:0;
      font-size:34px;
      background: linear-gradient(90deg,#ff0000,#ff6b6b,#ff9a76,#ffd166,#06d6a0,#118ab2,#9d4edd);
      -webkit-background-clip:text;
      -webkit-text-fill-color:transparent;
      font-weight:900;
    }
    p.lead{margin:8px 0 0;font-size:16px;opacity:.95;color:#333}

    .hero{display:flex;gap:24px;align-items:center;justify-content:space-between;margin-top:18px}
    .hero .info{flex:1}
    .hero .card{background:var(--card);border-radius:14px;padding:18px;box-shadow:0 6px 20px rgba(11,18,32,0.08)}

    .pricing{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:16px;margin-top:18px}
    .pkg{background:white;border-radius:12px;padding:16px;border:1px solid #eef2f6}
    .pkg h3{margin:0 0 8px;font-size:18px;color:#333}
    .price{font-size:22px;font-weight:700;color:var(--accent)}
    .pkg ul{padding-left:18px;margin:8px 0}
    .cta{display:inline-block;margin-top:12px;padding:10px 14px;border-radius:10px;background:var(--accent);color:white;text-decoration:none;font-weight:600;cursor:pointer;transition:0.3s ease;}
    .cta:hover{background:#ff4c4c}

    .details{display:grid;grid-template-columns:1fr 320px;gap:18px;margin-top:20px}
    .map-card{background:white;padding:14px;border-radius:12px;border:1px solid #eef2f6}

    footer{margin-top:30px;padding:18px;text-align:center;color:var(--muted);font-size:14px}

    .contact-card{background:linear-gradient(180deg, rgba(255,255,255,0.98), rgba(255,255,255,0.95));padding:16px;border-radius:12px;border:1px solid #f1f5f9}
    .contact-line{display:flex;gap:10px;align-items:center;margin:8px 0}
    .small{font-size:13px;color:var(--muted)}

    h2{
      background: linear-gradient(90deg,#ff6b6b,#f9c74f,#43aa8b,#577590);
      -webkit-background-clip:text;
      -webkit-text-fill-color:transparent;
      font-size:22px;
    }

    @media (max-width:780px){
      .hero{flex-direction:column}
      .details{grid-template-columns:1fr}
    }
  </style>
</head>
<body>
  <header>
    <div class="container">
      <h1>CasaRes Play</h1>
      <p class="lead">Aluguel de máquinas de pelúcia para festas e eventos — entrega grátis em regiões atendidas.</p>
    </div>
  </header>

  <main class="container">
    <section class="hero">
      <div class="info">
        <div class="card">
          <h2>Alugue a máquina de pelúcia</h2>
          <p style="margin:6px 0 0" class="small">Máquina disponível para eventos com ou sem pelúcias. Fácil operação — ideal para festas infantis, feiras e eventos corporativos.</p>

          <div style="margin-top:12px;display:flex;gap:12px;flex-wrap:wrap">
            <div style="min-width:170px">
              <div style="font-size:13px;color:var(--muted)">Aluguel da máquina (4 horas)</div>
              <div style="font-weight:700;font-size:18px;color:#ff6b6b">R$ 500</div>
            </div>
            <div style="min-width:170px">
              <div style="font-size:13px;color:var(--muted)">Pagamento</div>
              <div style="font-weight:700;font-size:16px;color:#43aa8b">Na hora de receber a máquina</div>
            </div>
          </div>

        </div>
      </div>

      <div style="width:320px">
        <div class="contact-card">
          <h3 style="background: linear-gradient(90deg,#ff6b6b,#f9c74f,#43aa8b,#577590);-webkit-background-clip:text;-webkit-text-fill-color:transparent;">Contato</h3>
          <div class="contact-line"><strong>WhatsApp / Telefone:</strong><a href="tel:+5521968884003"> (21) 96888-4003</a></div>
          <div class="contact-line"><strong>E‑mail:</strong><a href="mailto:casaresplayfesta@gmail.com"> casaresplayfesta@gmail.com</a></div>
          <p class="small" style="margin-top:6px">Atendimento para Paracambi, Seropédica, Japeri e Conrado. Frete grátis.</p>
          <a class="cta" href="https://wa.me/5521968884003?text=Olá,%20gostaria%20de%20reservar%20uma%20máquina" target="_blank">Reservar via WhatsApp</a>
        </div>
      </div>
    </section>

    <section style="margin-top:24px">
      <h2>Pacotes com pelúcias (4 horas)</h2>
      <div class="pricing">
        <div class="pkg">
          <h3>30 pelúcias + máquina</h3>
          <div class="price">R$ 1.000</div>
          <ul>
            <li>Inclui 30 pelúcias</li>
            <li>Uso da máquina por 4 horas</li>
            <li>Frete grátis nas regiões atendidas</li>
          </ul>
          <a class="cta" href="https://wa.me/5521968884003?text=Olá,%20gostaria%20de%20reservar%20a%20máquina%20com%2030%20pelúcias" target="_blank">Reservar</a>
        </div>

        <div class="pkg">
          <h3>50 pelúcias + máquina</h3>
          <div class="price">R$ 1.300</div>
          <ul>
            <li>Inclui 50 pelúcias</li>
            <li>Uso da máquina por 4 horas</li>
            <li>Frete grátis nas regiões atendidas</li>
          </ul>
          <a class="cta" href="https://wa.me/5521968884003?text=Olá,%20gostaria%20de%20reservar%20a%20máquina%20com%2050%20pelúcias" target="_blank">Reservar</a>
        </div>

        <div class="pkg">
          <h3>80 pelúcias + máquina</h3>
          <div class="price">R$ 1.750</div>
          <ul>
            <li>Inclui 80 pelúcias</li>
            <li>Uso da máquina por 4 horas</li>
            <li>Frete grátis nas regiões atendidas</li>
          </ul>
          <a class="cta" href="https://wa.me/5521968884003?text=Olá,%20gostaria%20de%20reservar%20a%20máquina%20com%2080%20pelúcias" target="_blank">Reservar</a>
        </div>

        <div class="pkg">
          <h3>Somente máquina (sem pelúcias)</h3>
          <div class="price">R$ 500</div>
          <ul>
            <li>Máquina por 4 horas</li>
            <li>Sem pelúcias</li>
            <li>Frete grátis nas regiões atendidas</li>
          </ul>
          <a class="cta" href="https://wa.me/5521968884003?text=Olá,%20gostaria%20de%20reservar%20somente%20a%20máquina" target="_blank">Reservar</a>
        </div>
      </div>
    </section>

    <section class="details">
      <div>
        <h2>Informações importantes</h2>
        <p class="small">Tempo de locação padrão: 4 horas. Caso precise de horário estendido ou transporte fora das regiões atendidas, entre em contato e
