<!doctype html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ma Page VidÃ©o</title>
    <style>
        body {
            background-color: black; /* Fond noir */
            color: white; /* Texte en blanc */
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center; /* Centrer le contenu */
        }
        h1 {
            color: #FFD700; /* Titre en couleur dorÃ©e */
            margin: 20px 0;
        }
        .profile {
            margin-bottom: 40px; /* Espace entre le profil et les vidÃ©os */
        }
        .profile img {
            max-width: 150px;
            border: 3px solid #FFD700; /* Bordure dorÃ©e */
            border-radius: 50%; /* Cercle pour l'image du profil */
        }
        .profile h2 {
            margin: 10px 0;
            color: #FFD700; /* Texte du profil en dorÃ© */
        }
        .video-container {
            display: flex;
            justify-content: center; /* Centrer les vidÃ©os horizontalement */
            gap: 20px; /* Espacement entre les vidÃ©os */
            flex-wrap: wrap; /* Permet le retour Ã  la ligne sur mobile */
            margin: 0; /* Enlever les marges */
        }
        .video-card {
            background-color: #222; /* Fond des cartes vidÃ©o */
            border-radius: 10px;
            padding: 15px;
            max-width: 300px;
            text-align: center;
            margin: 0; /* Enlever la marge */
        }
        .video-card img {
            max-width: 100%;
            height: auto;
            border: 3px solid #FFD700; /* Bordure dorÃ©e */
            border-radius: 10px; /* Coins arrondis */
        }
        .video-card h2 {
            margin: 10px 0;
            font-size: 18px;
            color: #FFD700; /* Couleur des titres des vidÃ©os */
        }
        .play-button {
            display: inline-block;
            margin-top: 10px;
            padding: 10px 20px;
            background-color: #FFD700; /* Fond dorÃ© */
            color: black; /* Texte noir */
            font-size: 16px;
            font-weight: bold;
            text-decoration: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.3s; /* Animation pour un effet plus fluide */
        }
        .play-button:hover {
            background-color: white;
            color: black;
            transform: scale(1.1); /* Effet d'agrandissement au survol */
        }
        video {
            max-width: 100%;
            border-radius: 10px;
            border: 3px solid #FFD700;
            display: none; /* Cacher la vidÃ©o par dÃ©faut */
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
        }
    </style>
</head>
<body>
    <!-- Titre principal -->
    <h1>Bienvenue ðŸ¤§âœ¨ Opening gratuit</h1>

    <!-- Profil -->
    <div class="profile">
        <img src="https://raw.githubusercontent.com/fatenit/fatenit/7c2d0cadb356838482ad2638b63c88137fe94c58/file-EGrZGMs3WV5mgdC4QSABj1.webp" alt="Mon profil">
        <h2>Mon Profil</h2>
    </div>

    <!-- Conteneur des vidÃ©os -->
    <div class="video-container">
        <!-- VidÃ©o 1 : Solo Leveling -->
        <div class="video-card">
            <img src="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/images.jpeg" alt="Solo Leveling">
            <h2>Solo Leveling</h2>
            <!-- Bouton qui dÃ©clenche la lecture -->
            <a href="#" class="play-button" onclick="playVideo(event, 'video1')">â–¶ Play la vidÃ©o</a>
            <!-- VidÃ©o cachÃ©e initialement -->
            <video id="video1" controls>
                <source src="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/VID_20250108_235757_560.mp4" type="video/mp4">
                Votre navigateur ne prend pas en charge la lecture des vidÃ©os.
            </video>
            <!-- Bouton de tÃ©lÃ©chargement -->
            <a href="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/VID_20250108_235757_560.mp4" class="download-button" download>ðŸ“¥ TÃ©lÃ©charger</a>
        </div>

        <!-- VidÃ©o 2 : Chainsaw Man -->
        <div class="video-card">
            <img src="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/MV5BZGY2ZTM2MWMtNzA2OS00ZjJlLWIwZTMtMDBhN2EwYjZjZjEyXkEyXkFqcGc%40._V1_FMjpg_UX1000_.jpg" alt="Chainsaw Man">
            <h2>Chainsaw Man</h2>
            <!-- Bouton qui dÃ©clenche la lecture -->
            <a href="#" class="play-button" onclick="playVideo(event, 'video2')">â–¶ Play la vidÃ©o</a>
            <!-- VidÃ©o cachÃ©e initialement -->
            <video id="video2" controls>
                <source src="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/VID_20250108_204359_261.mp4" type="video/mp4">
                Votre navigateur ne prend pas en charge la lecture des vidÃ©os.
            </video>
            <!-- Bouton de tÃ©lÃ©chargement -->
            <a href="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/VID_20250108_204359_261.mp4" class="download-button" download>ðŸ“¥ TÃ©lÃ©charger</a>
        </div>
    </div>

    <script>
        function playVideo(event, videoId) {
            event.preventDefault();  // EmpÃªche la page de remonter ou de recharger

            // Cacher toutes les vidÃ©os
            var allVideos = document.querySelectorAll('video');
            allVideos.forEach(function(video) {
                video.pause();  // Stopper la lecture
                video.style.display = "none";  // Cacher la vidÃ©o
            });

            // Afficher la vidÃ©o et la jouer
            var video = document.getElementById(videoId);
            video.style.display = "block";
            video.play();
        }
    </script>

</body></html>
