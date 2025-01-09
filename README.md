<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ma Page Vidéo</title>
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
            color: #FFD700; /* Titre en couleur dorée */
            margin: 20px 0;
        }
        .profile {
            margin-bottom: 40px; /* Espace entre le profil et les vidéos */
        }
        .profile img {
            max-width: 150px;
            border: 3px solid #FFD700; /* Bordure dorée */
            border-radius: 50%; /* Cercle pour l'image du profil */
        }
        .profile h2 {
            margin: 10px 0;
            color: #FFD700; /* Texte du profil en doré */
        }
        .video-container {
            display: flex;
            justify-content: center; /* Centrer les vidéos horizontalement */
            gap: 20px; /* Espacement entre les vidéos */
            flex-wrap: wrap; /* Permet le retour à la ligne sur mobile */
        }
        .video-card {
            background-color: #222; /* Fond des cartes vidéo */
            border-radius: 10px;
            padding: 15px;
            max-width: 300px;
            text-align: center;
        }
        .video-card img {
            max-width: 100%;
            height: auto;
            border: 3px solid #FFD700; /* Bordure dorée */
            border-radius: 10px; /* Coins arrondis */
        }
        .video-card h2 {
            margin: 10px 0;
            font-size: 18px;
            color: #FFD700; /* Couleur des titres des vidéos */
        }
        .play-button {
            display: inline-block;
            margin-top: 10px;
            padding: 10px 20px;
            background-color: #FFD700; /* Fond doré */
            color: black; /* Texte noir */
            font-size: 16px;
            font-weight: bold;
            text-decoration: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .play-button:hover {
            background-color: white;
            color: black;
        }
        video {
            max-width: 100%;
            border-radius: 10px;
            border: 3px solid #FFD700;
        }
    </style>
</head>
<body>
    <!-- Titre principal -->
    <h1>Bienvenue 🤧✨ Opening gratuit</h1>

    <!-- Profil -->
    <div class="profile">
        <img src="https://raw.githubusercontent.com/fatenit/fatenit/7c2d0cadb356838482ad2638b63c88137fe94c58/file-EGrZGMs3WV5mgdC4QSABj1.webp" alt="Mon profil">
        <h2>Mon Profil</h2>
    </div>

    <!-- Conteneur des vidéos -->
    <div class="video-container">
        <!-- Vidéo 1 : Solo Leveling -->
        <div class="video-card">
            <img src="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/images.jpeg" alt="Solo Leveling">
            <h2>Solo Leveling</h2>
            <!-- Lecture directe avec autoplay -->
            <video controls autoplay>
                <source src="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/VID_20250108_235757_560.mp4" type="video/mp4">
                Votre navigateur ne prend pas en charge la lecture des vidéos.
            </video>
        </div>

        <!-- Vidéo 2 : Chainsaw Man -->
        <div class="video-card">
            <img src="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/MV5BZGY2ZTM2MWMtNzA2OS00ZjJlLWIwZTMtMDBhN2EwYjZjZjEyXkEyXkFqcGc%40._V1_FMjpg_UX1000_.jpg" alt="Chainsaw Man">
            <h2>Chainsaw Man</h2>
            <!-- Lecture directe avec autoplay -->
            <video controls autoplay>
                <source src="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/VID_20250108_204359_261.mp4" type="video/mp4">
                Votre navigateur ne prend pas en charge la lecture des vidéos.
            </video>
        </div>
    </div>
</body>
</html>
