<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AliYTGame.com | Official</title>
  <style>
    :root {
      --primary-color: #ff8c00;
      --bg-color: #ffffff;
      --card-bg: #f5f5f5;
      --text-main: #1a1a1a;
      --header-bg: rgba(255, 255, 255, 0.95);
      --border-color: #dddddd;
      --neon-shadow: 0 0 15px rgba(255, 140, 0, 0.7);
    }

    @media (prefers-color-scheme: dark) {
      :root {
        --bg-color: #0f0f0f;
        --card-bg: #1a1a1a;
        --text-main: #ffffff;
        --header-bg: rgba(26, 26, 26, 0.95);
        --border-color: #222222;
      }
    }

    body {
      margin: 0;
      font-family: 'Segoe UI', Roboto, sans-serif;
      background-color: var(--bg-color);
      color: var(--text-main);
      transition: 0.3s;
      text-align: center;
    }

    header {
      background: var(--header-bg);
      padding: 10px 5%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 100;
      border-bottom: 2px solid var(--primary-color);
    }

    .logo-section {
      display: flex;
      align-items: center;
      gap: 10px;
      cursor: pointer;
    }

    .avatar-placeholder {
      width: 40px;
      height: 40px;
      border-radius: 50%;
      background: var(--primary-color);
      color: white;
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: bold;
      border: 2px solid #fff;
      box-shadow: var(--neon-shadow);
      font-size: 16px;
    }

    .burger-menu {
      font-size: 30px;
      cursor: pointer;
      color: var(--primary-color);
    }

    .menu-overlay {
      position: fixed;
      top: 0;
      right: -100%;
      width: 100%;
      height: 100%;
      background: var(--bg-color);
      z-index: 1000;
      transition: 0.4s;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding-top: 60px;
    }

    .menu-overlay.active {
      right: 0;
    }

    .close-btn {
      position: absolute;
      top: 20px;
      right: 20px;
      font-size: 40px;
      color: #ff5252;
      cursor: pointer;
    }

    .menu-links {
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    .menu-item {
      text-decoration: none;
      color: var(--text-main);
      font-weight: bold;
      font-size: 18px;
      text-transform: uppercase;
    }

    .container {
      max-width: 900px;
      margin: 30px auto;
      padding: 0 20px;
    }

    .section {
      background: var(--card-bg);
      padding: 30px;
      border-radius: 25px;
      margin-bottom: 25px;
      border: 1px solid var(--border-color);
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    .big-avatar {
      width: 120px;
      height: 120px;
      border-radius: 30px;
      background: var(--primary-color);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 50px;
      color: white;
      font-weight: bold;
      box-shadow: var(--neon-shadow);
      margin-bottom: 20px;
    }

    .history-list {
      list-style: none;
      padding: 0;
      text-align: left;
      display: inline-block;
    }

    .history-list li {
      margin-bottom: 15px;
      padding-left: 15px;
      border-left: 3px solid var(--primary-color);
    }

    textarea {
      width: 100%;
      max-width: 500px;
      box-sizing: border-box;
      border-radius: 10px;
      background: var(--bg-color);
      color: var(--text-main);
      border: 1px solid var(--primary-color);
      padding: 12px;
    }

    .btn-send {
      margin-top: 15px;
      padding: 12px 35px;
      background: var(--primary-color);
      color: white;
      border: none;
      border-radius: 10px;
      font-weight: bold;
      cursor: pointer;
      box-shadow: var(--neon-shadow);
    }

    #admin-panel {
      display: none;
      border: 2px dashed #ff5252;
    }
  </style>
</head>
<body>

  <header>
    <div class="logo-section" onclick="activateAdmin()">
      <div class="avatar-placeholder">AY</div>
      <span style="font-weight:bold; color:var(--primary-color);">AliYTGame.com</span>
    </div>
    <div class="burger-menu" onclick="toggleMenu()">☰</div>
  </header>

  <div class="menu-overlay" id="menu">
    <div class="close-btn" onclick="toggleMenu()">×</div>
    <div class="menu-links">
      <a href="#about" class="menu-item" onclick="toggleMenu()">👤 ОБО МНЕ</a>
      <a href="#my-game" class="menu-item" onclick="toggleMenu()">🎮 МОЯ ИГРА</a>
      <a href="#history" class="menu-item" onclick="toggleMenu()">📖 ИСТОРИЯ</a>
      <a href="#idea-form" class="menu-item" onclick="toggleMenu()">💡 ИДЕИ</a>
      <a href="https://www.youtube.com/@AliYTGAME005" class="menu-item" target="_blank">🔴 YOUTUBE</a>
      <a href="https://t.me/AliYTGame005" class="menu-item" target="_blank">✈️ TELEGRAM</a>
      <a href="https://www.roblox.com" class="menu-item" target="_blank">🕹️ ROBLOX</a>
      <a href="#admin-panel" class="menu-item" id="secret-tab" style="display: none; color: #ff5252;" onclick="toggleMenu()">🔒 АДМИН</a>
    </div>
  </div>

  <div class="container">
    <section class="section" id="about">
      <div class="big-avatar">AY</div>
      <h1>Привет, я Али! 😎</h1>
      <div style="max-width: 600px; line-height: 1.6;">
        <p>Я <strong>AliYTGame</strong> — ютубер и разработчик.</p>
        <p>Мне 11 лет, я учусь в 5 классе и являюсь <strong>отличником</strong>.</p>
        <p>Для записи видео я использую профессиональный микрофон <strong>Jmary MC-PW9</strong>.</p>
        <p>Помимо YouTube, я активно работаю над созданием <strong>собственной игры</strong>.</p>
        <p>Мои любимые игры: <strong>Brawl Stars</strong> и <strong>Roblox</strong>.</p>
      </div>
    </section>

    <section class="section" id="my-game">
      <h2>🎮 Моя игра</h2>
      <p>Я вкладываю много сил в разработку своего проекта. Следите за обновлениями на канале, чтобы не пропустить выход!</p>
    </section>

    <section class="section" id="history">
      <h2>📖 История моего пути</h2>
      <ul class="history-list">
        <li><strong>2024 год:</strong> Покупка микрофона Jmary и первые шаги.</li>
        <li><strong>Лето 2025:</strong> Разработка планов для канала и новых проектов.</li>
        <li><strong>Апрель 2026:</strong> Запуск официального сайта.</li>
        <li><strong>Главная цель:</strong> Набрать <strong>100,000 подписчиков</strong>!</li>
      </ul>
    </section>

    <section class="section" id="idea-form">
      <h2>💡 Предложить идею</h2>
      <textarea id="idea-input" rows="4" placeholder="Напиши идею для видео или моей игры..."></textarea>
      <button class="btn-send" onclick="sendIdea()">ОТПРАВИТЬ</button>
    </section>

    <section class="section" id="admin-panel">
      <h2 style="color:#ff5252;">🔒 Входящие идеи (Панель Али)</h2>
      <div id="ideas-list">Идей пока нет...</div>
    </section>
  </div>

  <script>
    function toggleMenu() {
      document.getElementById('menu').classList.toggle('active');
    }

    function sendIdea() {
      const input = document.getElementById('idea-input');
      if (input.value.trim() === "") return alert("Напиши текст!");
      let ideas = JSON.parse(localStorage.getItem('ali_ideas') || '[]');
      ideas.push(input.value);
      localStorage.setItem('ali_ideas', JSON.stringify(ideas));
      alert("Идея сохранена!");
      input.value = "";
      renderIdeas();
    }

    function renderIdeas() {
      const list = document.getElementById('ideas-list');
      let ideas = JSON.parse(localStorage.getItem('ali_ideas') || '[]');
      if (ideas.length === 0) return;
      list.innerHTML = ideas.map((id, index) => `<div style="padding:10px; border-bottom:1px solid #444; text-align:left;">${index + 1}. ${id}</div>`).join('');
    }

    let taps = 0;
    function activateAdmin() {
      taps++;
      if (taps === 5) {
        let pass = prompt("Введите секретный пароль:");
        if (pass === "Ali100k") {
          document.getElementById('admin-panel').style.display = 'block';
          document.getElementById('secret-tab').style.display = 'block';
          renderIdeas();
          alert('✅ Добро пожаловать, Али!');
        } else {
          alert('❌ Доступ запрещен!');
          taps = 0;
        }
      }
    }
  </script>
</body>
</html>
