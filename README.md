<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ma Page Vidéo Optimisée</title>
    <style>
        /* Styles globaux */
        body {
            background-color: black;
            color: white;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
        }

        h1 {
            color: #FFD700;
            margin: 20px 0;
        }

        /* Barre de recherche */
        .search-bar {
            margin: 20px;
        }

        .search-bar input {
            padding: 10px;
            width: 80%;
            max-width: 400px;
            border-radius: 5px;
            border: 1px solid #FFD700;
        }

        /* Conteneur des vidéos */
        .video-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            padding: 20px;
        }

        .video-card {
            background-color: #222;
            border-radius: 10px;
            padding: 15px;
            max-width: 300px;
            text-align: center;
        }

        .video-card img {
            max-width: 100%;
            height: auto;
            border: 3px solid #FFD700;
            border-radius: 10px;
        }

        .video-card h2 {
            margin: 10px 0;
            font-size: 18px;
            color: #FFD700;
        }
    </style>
</head>
<body>
    <h1>Bienvenue sur Mon Site</h1>

    <!-- Barre de recherche -->
    <div class="search-bar">
        <input type="text" id="search" placeholder="Rechercher un animé..." onkeyup="filterVideos()">
    </div>

    <!-- Conteneur des vidéos -->
    <div class="video-container" id="video-container">
        <!-- Exemple de carte vidéo -->
        <div class="video-card" data-title="Shangri-La Frontier">
            <img src="https://github.com/fatenit/open/blob/7bf8632a2c9bd2e474c31f67a5c6dbc55b2d07c2/chnagro%20la.jpg" alt="Shangri-La Frontier">
            <h2>Shangri-La Frontier</h2>
        </div>
        <div class="video-card" data-title="Beastars">
            <img src="https://github.com/fatenit/open/blob/7bf8632a2c9bd2e474c31f67a5c6dbc55b2d07c2/Beastars_Anime_Cover_1.jpg" alt="Beastars">
            <h2>Beastars</h2>
        </div>
    </div>

    <script>
        // Fonction pour filtrer les vidéos
        function filterVideos() {
            const searchInput = document.getElementById('search').value.toLowerCase();
            const videoCards = document.querySelectorAll('.video-card');

            videoCards.forEach(card => {
                const title = card.getAttribute('data-title').toLowerCase();
                card.style.display = title.includes(searchInput) ? 'block' : 'none';
            });
        }
    </script>
</body>
</html>
