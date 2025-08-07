<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Иван Курчук — TikTok Style</title>
  <style>
    :root {
      --bg: #0b0b0f;
      --text: #eaeaf5;
      --muted: #9a9fb2;
      --purple: #8b5cf6;
      --accent: #c084fc;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; }
    body {
      background: radial-gradient(1200px 800px at 80% -10%, rgba(139,92,246,0.2), transparent),
                  radial-gradient(1000px 700px at -10% 20%, rgba(168,85,247,0.2), transparent),
                  var(--bg);
      font-family: "Inter", sans-serif;
      color: var(--text);
      position: relative;
    }

    .nav {
      position: sticky;
      top: 0;
      backdrop-filter: blur(10px);
      background: rgba(11,11,15,0.7);
      padding: 16px 32px;
      display: flex;
      justify-content: flex-end;
      gap: 24px;
      z-index: 999;
    }

    .nav a {
      color: var(--muted);
      text-decoration: none;
      font-weight: 500;
      transition: color 0.2s ease;
    }

    .nav a:hover {
      color: var(--text);
    }

    .hero {
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
      padding: 100px 20px 60px;
      animation: fadeIn 1s ease forwards;
    }

    .avatar {
      width: 96px;
      height: 96px;
      border-radius: 20px;
      overflow: hidden;
      margin-bottom: 24px;
      box-shadow: 0 0 24px rgba(192,132,252,0.3);
    }

    .avatar img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .name {
      font-size: 48px;
      font-weight: 800;
      background: linear-gradient(90deg, #fff, var(--accent), var(--purple));
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      text-shadow: 0 0 14px rgba(167,139,250,0.3);
    }

    .subtitle {
      margin-top: 16px;
      color: var(--muted);
      max-width: 600px;
    }

    section {
      padding: 60px 24px;
      max-width: 800px;
      margin: 0 auto;
      animation: fadeInUp 1.2s ease forwards;
    }

    h2 {
      font-size: 28px;
      margin-bottom: 12px;
    }

    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .card {
      background: rgba(255,255,255,0.03);
      border: 1px solid rgba(255,255,255,0.06);
      padding: 20px;
      border-radius: 16px;
      box-shadow: 0 0 30px rgba(139,92,246,0.15);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      margin-top: 24px;
    }

    .card:hover {
      transform: translateY(-4px);
      box-shadow: 0 0 40px rgba(139,92,246,0.3);
    }

    .socials {
      display: flex;
      gap: 16px;
      justify-content: center;
      margin-top: 20px;
      flex-wrap: wrap;
    }

    .socials a {
      padding: 12px 18px;
      border: 1px solid var(--accent);
      border-radius: 10px;
      color: #fff;
      text-decoration: none;
      background: rgba(139,92,246,0.1);
      box-shadow: 0 0 14px rgba(192,132,252,0.2);
      transition: all 0.2s ease;
    }

    .socials a:hover {
      background: rgba(139,92,246,0.3);
      box-shadow: 0 0 22px rgba(192,132,252,0.4);
    }

    footer {
      text-align: center;
      padding: 40px 20px 60px;
      font-size: 14px;
      color: var(--muted);
      backdrop-filter: blur(6px);
    }

    footer p {
      margin-bottom: 6px;
    }

    .music-toggle {
      position: fixed;
      bottom: 20px;
      left: 20px;
      z-index: 1000;
    }

    .music-toggle button {
      background: rgba(139, 92, 246, 0.25);
      border: 1px solid var(--accent);
      color: #fff;
      font-weight: 600;
      padding: 10px 16px;
      border-radius: 12px;
      box-shadow: 0 0 14px rgba(192,132,252,0.25);
      cursor: pointer;
      transition: background 0.2s ease;
    }

    .music-toggle button:hover {
      background: rgba(139, 92, 246, 0.4);
    }
  </style>
</head>
<body>


  <audio id="bgMusic" autoplay loop>
    <source src="https://s.muzrecord.com/files/nekoglay-ivanzolo2004-obychnyy-paren.mp3" type="audio/mpeg">
  </audio>

  <nav class="nav">
    <a href="#about">Обо мне</a>
    <a href="#contact">Связаться</a>
  </nav>

  <div class="hero">
    <div class="avatar">
      <img src="https://cdn.discordapp.com/attachments/1346567060695547936/1403093449523204320/14B11E09-312C-41F4-8A0E-24F2A5C4CCEC.png?ex=68964c1a&is=6894fa9a&hm=bc4fa58e8439675e18878de06a45252f71574446437f00925a8fe8fecf5425d3&" alt="Фото Ивана">
    </div>
    <h1 class="name">Иван Курчук</h1>
    <p class="subtitle">ну я кароче играю хнсик у меня есть друзья я тиктокер</p>
  </div>

  <section id="about">
    <h2>Обо мне</h2>
    <div class="card">
      <p>ну я кароче играю хнсик у меня есть друзья я тиктокер</p>
    </div>
    <div class="card">
      <p>ставьте лайки подписывайтесь на канал всем пока.</p>
    </div>
  </section>

  <section id="contact">
    <h2>Связаться со мной</h2>
    <div class="socials">
      <a href="https://www.tiktok.com/@4o3a4ejl" target="_blank">TikTok</a>
      <a href="https://t.me/DarkKillerBrawlAssasin" target="_blank">Telegram</a>
      <a href="https://discord.com/users/647735114364878858" target="_blank">Discord</a>
    </div>
  </section>

  <footer>
    <p>&copy; <span id="year"></span> Все права защищены.</p>
    <p>Made by Ivan Kurchuk</p>
  </footer>

  <script>
    // Автоматический год
    document.getElementById
