<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Roblox Tasarım Taslağı | ibo_ucatli</title>
    <style>
        /* Roblox Koyu Tema Renkleri */
        :root {
            --bg-color: #232527;
            --nav-color: #393b3d;
            --card-color: #393b3d;
            --text-color: #ffffff;
            --accent-blue: #00a2ff;
        }

        body {
            margin: 0;
            padding: 0;
            background-color: var(--bg-color);
            color: var(--text-color);
            font-family: 'Segoe UI', Arial, sans-serif;
        }

        /* Navigasyon Çubuğu */
        nav {
            background-color: var(--nav-color);
            height: 60px;
            display: flex;
            align-items: center;
            padding: 0 20px;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 100;
            box-sizing: border-box;
        }

        .logo {
            font-weight: bold;
            font-size: 24px;
            margin-right: 30px;
            cursor: pointer;
        }

        .nav-links a {
            color: #ddd;
            text-decoration: none;
            margin-right: 20px;
            font-size: 16px;
        }

        .nav-links a:hover { color: white; }

        /* Ana İçerik Alanı */
        .container {
            margin-top: 80px;
            padding: 20px;
            max-width: 1200px;
            margin-left: auto;
            margin-right: auto;
        }

        h2 { margin-bottom: 20px; }

        /* Oyun Kartları Düzeni (Grid) */
        .game-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
            gap: 20px;
        }

        .game-card {
            background-color: var(--card-color);
            border-radius: 8px;
            overflow: hidden;
            transition: transform 0.2s;
            cursor: pointer;
        }

        .game-card:hover {
            transform: scale(1.05);
        }

        .thumbnail {
            width: 100%;
            aspect-ratio: 1 / 1;
            background-color: #555;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 12px;
            color: #ccc;
        }

        .game-info {
            padding: 10px;
        }

        .game-title {
            font-weight: bold;
            font-size: 14px;
            margin-bottom: 5px;
            white-space: nowrap;
            overflow: hidden;
            text-overflow: ellipsis;
        }

        .game-stats {
            font-size: 12px;
            color: #bbb;
        }

        .play-btn {
            background-color: var(--accent-blue);
            color: white;
            border: none;
            padding: 8px 15px;
            border-radius: 5px;
            cursor: pointer;
            width: 100%;
            margin-top: 10px;
            font-weight: bold;
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo">ROBLOX_CLONE</div>
        <div class="nav-links">
            <a href="#">Ana Sayfa</a>
            <a href="#">Market</a>
            <a href="#">Oluştur</a>
            <a href="#">Robux</a>
        </div>
    </nav>

    <div class="container">
        <h2>Senin İçin Önerilenler</h2>
        
        <div class="game-grid">
            <div class="game-card">
                <div class="thumbnail">[Görüntü Yok]</div>
                <div class="game-info">
                    <div class="game-title">Adopt Me Clone</div>
                    <div class="game-stats">👍 92% | 👥 150K</div>
                    <button class="play-btn">Oyna</button>
                </div>
            </div>

            <div class="game-card">
                <div class="thumbnail">[Görüntü Yok]</div>
                <div class="game-info">
                    <div class="game-title">Brookhaven RP</div>
                    <div class="game-stats">👍 88% | 👥 240K</div>
                    <button class="play-btn">Oyna</button>
                </div>
            </div>

            <div class="game-card">
                <div class="thumbnail">[Görüntü Yok]</div>
                <div class="game-info">
                    <div class="game-title">Blox Fruits</div>
                    <div class="game-stats">👍 95% | 👥 500K</div>
                    <button class="play-btn">Oyna</button>
                </div>
            </div>

            <div class="game-card">
                <div class="thumbnail">[Görüntü Yok]</div>
                <div class="game-info">
                    <div class="game-title">Tower of Hell</div>
                    <div class="game-stats">👍 80% | 👥 45K</div>
                    <button class="play-btn">Oyna</button>
                </div>
            </div>
        </div>
    </div>

    <script>
        // İstersen buraya butonlara tıklayınca ne olacağını yazabilirsin
        document.querySelectorAll('.play-btn').forEach(button => {
            button.addEventListener('click', () => {
                alert("Oyun başlatılıyor... (Simülasyon)");
            });
        });
    </script>
</body>
</html>
