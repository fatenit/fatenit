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
            text-align: center; /* Centrer le contenu */
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        h1 {
            color: #FFD700; /* Titre en couleur dorée */
            margin-top: 20px;
        }
        img {
            max-width: 80%;
            height: auto;
            border: 5px solid #FFD700; /* Bordure dorée autour de l'image */
        }
        .play-button {
            display: inline-block;
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #FFD700; /* Fond doré */
            color: black; /* Texte noir */
            font-size: 18px;
            font-weight: bold;
            text-decoration: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .play-button:hover {
            background-color: white;
            color: black;
        }
    </style>
</head>
<body>
    <h1>Bienvenue sur ma page</h1>
    <img src="https://raw.githubusercontent.com/fatenit/fatenit/main/1736368465598.jpg" alt="Image d'accueil">
    <br>
    <a href="https://raw.githubusercontent.com/fatenit/fatenit/main/VID_20250108_204404_881.mp4" class="play-button" target="_blank">▶ Play la vidéo</a>
</body>
</html>
