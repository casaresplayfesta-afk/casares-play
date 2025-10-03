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

    .logo-container {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 12px;
    }
    .logo {
      max-height: 60px;
      border-radius: 8px;
    }
    /* Texto colorido neon */
    .logo-text {
      font-size: 28px;
      font-weight: 800;
      background: linear-gradient(90deg, #ff0000, #ff9900, #33cc33, #3399ff, #cc33ff);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      text-shadow: 0 0 8px rgba(255,255,255,0.8);
    }
    .logo-text span {
      color: white;
      text-shadow: 0 0 6px #ff00ff, 0 0 12px #ff33cc;
    }

    header .lead { font-size: 14px; color: #fff; opacity: .9; margin-top: 6px; }

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
      display: grid; grid-template-co
