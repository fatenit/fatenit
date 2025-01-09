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
            font-size: 16px;
        }

        /* Section "À propos de moi" */
        .about-section {
            display: none;
            background-color: #333;
            color: white;
            padding: 20px;
            border-radius: 10px;
            margin: 20px auto;
            max-width: 800px;
            position: relative;
        }

        .close-about {
            position: absolute;
            top: 10px;
            right: 10px;
            color: #FFD700;
            cursor: pointer;
            font-size: 20px;
        }

        /* Profil */
        .profile img {
            max-width: 150px;
            border: 3px solid #FFD700;
            border-radius: 50%;
            cursor: pointer;
            transition: transform 0.3s;
        }

        .profile img:hover {
            transform: scale(1.1);
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

        .play-button {
            display: inline-block;
            margin-top: 10px;
            padding: 10px 20px;
            background-color: #FFD700;
            color: black;
            font-size: 16px;
            font-weight: bold;
            text-decoration: none;
            border-radius: 5px;
            cursor: pointer;
        }

        .play-button:hover {
            background-color: white;
            color: black;
            transform: scale(1.1);
            transition: all 0.3s ease;
        }

        video {
            max-width: 100%;
            border-radius: 10px;
            border: 3px solid #FFD700;
            display: none; /* Masqué par défaut */
        }

        .download-button {
            display: inline-block;
            margin-top: 10px;
            padding: 10px 20px;
            background-color: #555;
            color: white;
            font-size: 14px;
            font-weight: bold;
            text-decoration: none;
            border-radius: 5px;
            cursor: pointer;
        }

        .download-button:hover {
            background-color: #FFD700;
            color: black;
            transform: scale(1.1);
            transition: all 0.3s ease;
        }
    </style>
</head>
<body>
    <h1>Bienvenue sur Mon Site</h1>

    <!-- Barre de recherche -->
    <div class="search-bar">
        <input type="text" id="search" placeholder="Rechercher un animé..." onkeyup="filterVideos()">
    </div>

    <!-- Profil -->
    <div class="profile">
        <img src="https://github.com/fatenit/fatenit/blob/main/profile.jpg" alt="Mon profil" onclick="toggleAbout()">
    </div>

    <!-- Section "À propos de moi" -->
    <div class="about-section" id="about">
        <span class="close-about" onclick="toggleAbout()">✖</span>
        <h2>À propos de moi</h2>
        <p>
            J'ai créé ce site pour aider ceux qui ont des difficultés à télécharger certains contenus. 
            Je suis passionné par le codage et les animés. Ce site est en constante évolution, 
            et vos suggestions sont toujours les bienvenues !
        </p>
        <p>Email : <a href="mailto:firs1tsiteweb@gmail.com">firs1tsiteweb@gmail.com</a></p>
        <p>Code promo pour me soutenir : <strong>1XBET : ALLER</strong></p>
    </div>

    <!-- Conteneur des vidéos -->
    <div class="video-container" id="video-container">
        <!-- Exemple de carte vidéo -->
        <div class="video-card" data-title="Shangri-La Frontier">
            <img src="https://github.com/fatenit/open/blob/7bf8632a2c9bd2e474c31f67a5c6dbc55b2d07c2/chnagro%20la.jpg" alt="Shangri-La Frontier">
            <h2>Shangri-La Frontier</h2>
            <button class="play-button" onclick="chooseVideo('Shangri-La Frontier', ['Vidéo 1', 'Vidéo 2'])">▶ Play</button>
            <a href="https://github.com/fatenit/open/blob/7bf8632a2c9bd2e474c31f67a5c6dbc55b2d07c2/1%20changrila.mp4" class="download-button" download>🕳️ Télécharger</a>
        </div>
        <!-- Ajouter d'autres vidéos ici -->
    </div>

    <script>
        // Affichage de la section "À propos de moi"
        function toggleAbout() {
            const aboutSection = document.getElementById('about');
            aboutSection.style.display = aboutSection.style.display === 'block' ? 'none' : 'block';
        }

        // Gestion du choix de vidéo
        function chooseVideo(title, options) {
            const choice = prompt(`Choisissez une vidéo pour ${title} :\n` + options.join('\n'));
            if (choice) {
                alert(`Vous avez choisi ${choice}`);
                // Ajouter une logique pour afficher et lire la vidéo choisie
            }
        }

        // Filtrage des vidéos avec la barre de recherche
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
