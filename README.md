<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MAXIM | DESIGN & DEV</title>
    <style>
        :root {
            --bg: #050505;
            --accent: #00ff41;
            --text: #ffffff;
            --card-bg: #111;
        }
        body {
            font-family: 'Inter', -apple-system, sans-serif;
            background-color: var(--bg);
            color: var(--text);
            margin: 0;
            padding: 40px 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        header {
            text-align: center;
            margin-bottom: 50px;
        }
        h1 {
            font-size: 2rem;
            letter-spacing: 5px;
            text-transform: uppercase;
            margin: 0;
            color: var(--accent);
        }
        .subtitle {
            color: #555;
            font-size: 0.9rem;
            margin-top: 10px;
        }
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            width: 100%;
            max-width: 900px;
        }
        .project-card {
            background: var(--card-bg);
            border: 1px solid #222;
            padding: 25px;
            border-radius: 12px;
            text-decoration: none;
            color: inherit;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
        }
        .project-card:hover {
            border-color: var(--accent);
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(0, 255, 65, 0.1);
        }
        .project-card h2 {
            margin: 0 0 10px 0;
            font-size: 1.2rem;
        }
        .project-card p {
            color: #888;
            font-size: 0.85rem;
            margin: 0;
        }
        .tag {
            display: inline-block;
            font-size: 0.7rem;
            background: #222;
            color: var(--accent);
            padding: 4px 10px;
            border-radius: 20px;
            margin-top: 15px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        .grid-bg {
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background-image: linear-gradient(#111 1px, transparent 1px), linear-gradient(90deg, #111 1px, transparent 1px);
            background-size: 40px 40px;
            z-index: -1;
            opacity: 0.3;
        }
    </style>
</head>
<body>

<div class="grid-bg"></div>

<header>
    <h1>MAXIM</h1>
    <div class="subtitle">Design, 3D Visualization & Automation</div>
</header>

<div class="grid">
    <!-- КАРТОЧКА АРТУРА -->
    <a href="artur/" class="project-card">
        <h2>Артур</h2>
        <p>Дизайн интерьера и экстерьера. Пивная Дом.</p>
        <div class="tag">В работе</div>
    </a>

    <!-- КАРТОЧКА АЛЕКСЕЯ ВИКТОРОВИЧА -->
    <a href="aleksey/" class="project-card">
        <h2>Алексей Викторович</h2>
        <p>Ландшафт и система автополива.</p>
        <div class="tag">Проектирование</div>
    </a>

    <!-- КАРТОЧКА НАТАЛКИ -->
    <a href="natalka/" class="project-card">
        <h2>Наталка</h2>
        <p>Реставрация и покраска (Дверь).</p>
        <div class="tag">В очереди</div>
    </a>

    <!-- ШВЕДИНО -->
    <a href="shvedino/" class="project-card">
        <h2>Шведино</h2>
        <p>Автоматизация полива яблочного сада.</p>
        <div class="tag">Разработка ESP32</div>
    </a>
</div>

</body>
</html>
