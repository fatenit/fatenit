<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ma Page Vidéo</title>
    <style>
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
        .profile {
            margin: 20px;
        }
        .profile img {
            max-width: 150px;
            border: 3px solid #FFD700;
            border-radius: 50%;
            cursor: pointer;
        }
        .profile h2 {
            color: #FFD700;
        }
        .about-me {
            display: none;
            background-color: #333;
            padding: 20px;
            border-radius: 10px;
            margin: 20px;
        }
        .search-bar {
            margin: 20px;
        }
        .search-bar input {
            width: 80%;
            padding: 8px;
            border: 2px solid #FFD700;
            border-radius: 5px;
        }
        .video-container {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
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
            border: 3px solid #FFD700;
            border-radius: 10px;
        }
        .video-card h2 {
            margin: 10px 0;
            color: #FFD700;
        }
        .play-button {
            display: block;
            margin: 10px auto;
            padding: 10px 20px;
            border-radius: 5px;
            background-color: #FFD700;
            color: black;
            text-decoration: none;
            cursor: pointer;
        }
        .play-button:hover {
            background-color: white;
        }
    </style>
</head>
<body>
    <h1>Bienvenue 🤧✨ Opening gratuit</h1>

    <!-- Profil -->
    <div class="profile">
        <img src="https://raw.githubusercontent.com/fatenit/fatenit/7c2d0cadb356838482ad2638b63c88137fe94c58/file-EGrZGMs3WV5mgdC4QSABj1.webp" alt="Mon profil" onclick="toggleAboutMe()">
        <h2>Mon Profil</h2>
    </div>

    <!-- À propos de moi -->
    <div id="aboutMe" class="about-me">
        <p>
            J'ai créé ce site pour aider ceux qui ont du mal à télécharger des contenus. Je suis un grand fan du codage et des animés, 
            même si l'animation n'est pas mon point fort. Ce site est limité, mais je l'améliore constamment. Si vous avez des suggestions, 
            contactez-moi à <a href="mailto:firs1tsiteweb@gmail.com">firs1tsiteweb@gmail.com</a>. Merci pour votre soutien !
        </p>
    </div>

    <!-- Barre de recherche -->
    <div class="search-bar">
        <input type="text" id="searchInput" placeholder="Rechercher un titre..." oninput="searchVideo()">
    </div>

    <!-- Liste des vidéos -->
    <div id="videoList" class="video-container">
        <!-- Vidéo : Solo Leveling -->
        <div class="video-card" data-title="Solo Leveling">
            <img src="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/images.jpeg" alt="Solo Leveling">
            <h2>Solo Leveling</h2>
            <a href="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/VID_20250108_235757_560.mp4" class="play-button">▶ Play</a>
        </div>

        <!-- Vidéo : Shangri-La Frontier -->
        <div class="video-card" data-title="Shangri-La Frontier">
            <img src="https://github.com/fatenit/open/blob/7bf8632a2c9bd2e474c31f67a5c6dbc55b2d07c2/chnagro%20la.jpg?raw=true" alt="Shangri-La Frontier">
            <h2>Shangri-La Frontier</h2>
            <select id="shangriOptions">
                <option value="1">Vidéo 1</option>
                <option value="2">Vidéo 2</option>
            </select>
            <button class="play-button" onclick="playSelected('shangriOptions', ['https://github.com/fatenit/open/blob/7bf8632a2c9bd2e474c31f67a5c6dbc55b2d07c2/1%20changrila.mp4', 'https://github.com/fatenit/open/blob/7bf8632a2c9bd2e474c31f67a5c6dbc55b2d07c2/2%20changrila.mp4'])">
                ▶ Lire la vidéo
            </button>
        </div>

        <!-- Vidéo : Mashle -->
        <div class="video-card" data-title="Mashle">
            <img src="https://github.com/fatenit/open/blob/7bf8632a2c9bd2e474c31f67a5c6dbc55b2d07c2/manshel.jpg?raw=true" alt="Mashle">
            <h2>Mashle</h2>
            <a href="https://github.com/fatenit/open/blob/7bf8632a2c9bd2e474c31f67a5c6dbc55b2d07c2/manshel%201.mp4" class="play-button">▶ Play</a>
        </div>
        <!-- Ajoutez les autres vidéos -->
    </div>

    <script>
        function toggleAboutMe() {
            const aboutMe = document.getElementById('aboutMe');
            aboutMe.style.display = aboutMe.style.display === 'none' || aboutMe.style.display === '' ? 'block' : 'none';
        }

        function searchVideo() {
            const input = document.getElementById('searchInput').value.toLowerCase();
            const videoCards = document.querySelectorAll('.video-card');

            videoCards.forEach(card => {
                const title = card.getAttribute('data-title').toLowerCase();
                if (title.includes(input)) {
                    card.style.display = "block";
                } else {
                    card.style.display = "none";
                }
            });
        }

        function playSelected(selectId, videoUrls) {
            const selected = document.getElementById(selectId).value;
            const videoUrl = videoUrls[selected - 1];
            window.open(videoUrl, '_blank');
        }
    </script>
</body>
</html>
