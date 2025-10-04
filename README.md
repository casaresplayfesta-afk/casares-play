<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>Botões WhatsApp e Instagram</title>
  <style>
    /* Container dos botões */
    .social-buttons {
      position: fixed;
      bottom: 20px;
      right: 20px;
      display: flex;
      flex-direction: row;
      gap: 12px;
      z-index: 10000;
    }

    /* Botão WhatsApp */
    .whatsapp-premium {
      background: #25D366;
      color: white;
      padding: 16px 20px;
      border-radius: 50px;
      text-decoration: none;
      font-weight: bold;
      display: flex;
      align-items: center;
      gap: 10px;
      box-shadow: 0 0 20px rgba(37, 211, 102, 0.6);
      transition: transform 0.2s, box-shadow 0.2s;
      animation: glowPulseWhats 2s infinite;
    }

    .whatsapp-premium img {
      width: 26px;
      height: 26px;
    }

    .whatsapp-premium:hover {
      transform: scale(1.15);
      box-shadow: 0 0 30px rgba(37, 211, 102, 0.9), 0 0 40px rgba(37, 211, 102, 0.6);
    }

    @keyframes glowPulseWhats {
      0% { transform: scale(1); box-shadow: 0 0 20px rgba(37, 211, 102, 0.6); }
      50% { transform: scale(1.1); box-shadow: 0 0 30px rgba(37, 211, 102, 0.8); }
      100% { transform: scale(1); box-shadow: 0 0 20px rgba(37, 211, 102, 0.6); }
    }

    /* Botão Instagram */
    .instagram-premium {
      background: linear-gradient(45deg, #f09433, #e6683c, #dc2743, #cc2366, #bc1888);
      color: white;
      padding: 16px 20px;
      border-radius: 50px;
      text-decoration: none;
      font-weight: bold;
      display: flex;
      align-items: center;
      gap: 10px;
      box-shadow: 0 0 20px rgba(220, 39, 67, 0.6);
      transition: transform 0.2s, box-shadow 0.2s;
      animation: glowPulseInsta 2s infinite;
    }

    .instagram-premium img {
      width: 26px;
      height: 26px;
    }

    .instagram-premium:hover {
      transform: scale(1.15);
      box-shadow: 0 0 30px rgba(220, 39, 67, 0.9), 0 0 40px rgba(220, 39, 67, 0.6);
    }

    @keyframes glowPulseInsta {
      0% { transform: scale(1); box-shadow: 0 0 20px rgba(220, 39, 67, 0.6); }
      50% { transform: scale(1.1); box-shadow: 0 0 30px rgba(220, 39, 67, 0.8); }
      100% { transform: scale(1); box-shadow: 0 0 20px rgba(220, 39, 67, 0.6); }
    }
  </style>
</head>
<body>

  <!-- Botões flutuantes WhatsApp e Instagram -->
  <div class="social-buttons">
    <a href="https://wa.me/5521968884003?text=Olá,%20quero%20mais%20informações%20sobre%20o%20aluguel%20da%20máquina%20de%20pelúcia" 
       target="_blank" 
       class="whatsapp-premium">
       <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" alt="WhatsApp">
       WhatsApp
    </a>

    <a href="https://www.instagram.com/diversao_em_festas_?utm_source=ig_web_button_share_sheet&igsh=c3U2a2xudTFibTE5" 
       target="_blank" 
       class="instagram-premium">
       <img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="Instagram">
       Instagram
    </a>
  </div>

</body>
</html>
