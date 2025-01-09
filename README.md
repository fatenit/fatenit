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
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 10px 20px;
            background-color: #222;
        }
        header .search-bar {
            max-width: 300px;
        }
        header input {
            width: 100%;
            padding: 8px;
            border: 2px solid #FFD700;
            border-radius: 5px;
        }
        .profile {
            margin: 20px;
        }
        .profile img {
            max-width: 150px;
            border: 3px solid #FFD700;
            border-radius: 50%;
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
        .about-me button {
            margin-top: 10px;
            padding: 8px 15px;
            background-color: #FFD700;
            color: black;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .video-container {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin: 0;
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
        .play-button, .download-button {
            display: block;
            margin: 10px auto;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
        }
        .play-button {
            background-color: #FFD700;
            color: black;
            text-decoration: none;
        }
        .play-button:hover {
            background-color: white;
        }
        .download-button {
            background-color: #555;
            color: white;
            text-decoration: none;
        }
        .download-button:hover {
            background-color: #FFD700;
        }
    </style>
</head>
<body>
    <header>
        <h1>Bienvenue 🤧✨ Opening gratuit</h1>
        <div class="search-bar">
            <input type="text" placeholder="Rechercher...">
        </div>
    </header>

    <div class="profile">
        <img src="https://raw.githubusercontent.com/fatenit/fatenit/7c2d0cadb356838482ad2638b63c88137fe94c58/file-EGrZGMs3WV5mgdC4QSABj1.webp" alt="Mon profil">
        <h2>Mon Profil</h2>
        <button onclick="toggleAboutMe()">À propos de moi</button>
    </div>

    <div id="aboutMe" class="about-me">
        <p>
            J'ai créé ce site pour aider ceux qui ont du mal à télécharger des contenus. Je suis un grand fan du codage et des animés, 
            même si l'animation n'est pas mon point fort. Ce site est limité, mais je l'améliore constamment. Si vous avez des suggestions, 
            contactez-moi à <a href="mailto:firs1tsiteweb@gmail.com">firs1tsiteweb@gmail.com</a>. Merci pour votre soutien !
        </p>
        <button onclick="toggleAboutMe()">Fermer</button>
    </div>

    <div class="video-container">
        <!-- Exemple avec multiples vidéos -->
        <div class="video-card">
            <img src="https://github.com/fatenit/open/blob/7bf8632a2c9bd2e474c31f67a5c6dbc55b2d07c2/chnagro%20la.jpg?raw=true" alt="Shangri-La Frontier">
            <h2>Shangri-La Frontier</h2>
            <select id="shangriOptions">
                <option value="1">Vidéo 1</option>
                <option value="2">Vidéo 2</option>
            </select>
            <button class="play-button" onclick="playSelected('shangriOptions', ['https://github.com/fatenit/open/blob/.../1.mp4', '...'])">▶ Play</button>
        </div>
    </div>

    <script>
        function toggleAboutMe() {
            const aboutMe = document.getElementById('aboutMe');
            aboutMe.style.display = aboutMe.style.display === 'none' || aboutMe.style.display === '' ? 'block' : 'none';
        }

        function playSelected(selectId, videoUrls) {
            const selected = document.getElementById(selectId).value;
            const videoUrl = videoUrls[selected - 1];
            window.open(videoUrl, '_blank');
        }
    </script>
</body>
</html>
