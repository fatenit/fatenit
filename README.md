FATENIT🪽
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ma Page Vidéo</title>

    <script async src="https://www.googletagmanager.com/gtag/js?id=G-NR6N2SFPSD"></script>
    <script>
      window.dataLayer = window.dataLayer || [];
      function gtag(){dataLayer.push(arguments);}
      gtag('js', new Date());
      gtag('config', 'G-NR6N2SFPSD');
    </script>

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
            margin-bottom: 40px;
        }
        .profile img {
            max-width: 150px;
            border: 3px solid #FFD700;
            border-radius: 50%;
        }
        .profile h2 {
            margin: 10px 0;
            color: #FFD700;
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
            margin: 0;
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
            transition: background-color 0.3s, transform 0.3s;
        }
        .play-button:hover {
            background-color: white;
            color: black;
            transform: scale(1.1);
        }
        video {
            max-width: 100%;
            border-radius: 10px;
            border: 3px solid #FFD700;
            display: none;
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
    <h1>Bienvenue 🤧✨ Opening gratuit</h1>

    <div class="profile">
        <img src="https://raw.githubusercontent.com/fatenit/fatenit/7c2d0cadb356838482ad2638b63c88137fe94c58/file-EGrZGMs3WV5mgdC4QSABj1.webp" alt="Mon profil">
        <h2>Mon Profil</h2>
    </div>

    <div class="video-container">
        <!-- Solo Leveling -->
        <div class="video-card">
            <img src="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/images.jpeg" alt="Solo Leveling">
            <h2>Solo Leveling</h2>
            <a href="#" class="play-button" onclick="playVideo(event, 'video1')">▶ Play la vidéo</a>
            <video id="video1" controls>
                <source src="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/VID_20250108_235757_560.mp4?raw=true" type="video/mp4">
            </video>
            <a href="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/VID_20250108_235757_560.mp4?raw=true" class="download-button" download>🕳️🪽 Télécharger</a>
        </div>

        <!-- Chainsaw Man -->
        <div class="video-card">
            <img src="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/MV5BZGY2ZTM2MWMtNzA2OS00ZjJlLWIwZTMtMDBhN2EwYjZjZjEyXkEyXkFqcGc%40._V1_FMjpg_UX1000_.jpg" alt="Chainsaw Man">
            <h2>Chainsaw Man</h2>
            <a href="#" class="play-button" onclick="playVideo(event, 'video2')">▶ Play la vidéo</a>
            <video id="video2" controls>
                <source src="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/VID_20250108_204359_261.mp4?raw=true" type="video/mp4">
            </video>
            <a href="https://raw.githubusercontent.com/fatenit/open/7a9b81ff379b9c10b20945e26ce476d3dff0d3f1/VID_20250108_204359_261.mp4?raw=true" class="download-button" download>🕳️🪽 Télécharger</a>
        </div>

        <!-- Beastars -->
        <div class="video-card">
            <img src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/Beastars_Anime_Cover_1.jpg?raw=true" alt="Beastars">
            <h2>Beastars</h2>
            <a href="#" class="play-button" onclick="playVideo(event, 'video3')">▶ Play la vidéo</a>
            <video id="video3" controls>
                <source src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/beastars1.mp4?raw=true" type="video/mp4">
            </video>
            <a href="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/beastars1.mp4?raw=true" class="download-button" download>🕳️🪽 Télécharger</a>
        </div>

        <!-- Changri La Frontière -->
        <div class="video-card">
            <img src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/chnagro%20la.jpg?raw=true" alt="Changri La Frontière">
            <h2>Changri La Frontière</h2>
            <a href="#" class="play-button" onclick="playVideo(event, 'video4')">▶ Play la vidéo</a>
            <video id="video4" controls>
                <source src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/1%20changrila.mp4?raw=true" type="video/mp4">
            </video>
            <a href="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/1%20changrila.mp4?raw=true" class="download-button" download>🕳️🪽 Télécharger</a>
        </div>

        <!-- Oshi no Ko -->
        <div class="video-card">
            <img src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/oshi%20no%20ko.jpg?raw=true" alt="Oshi no Ko">
            <h2>Oshi no Ko</h2>
            <a href="#" class="play-button" onclick="playVideo(event, 'video5')">▶ Play la vidéo</a>
            <video id="video5" controls>
                <source src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/oshi%20no%20ko%201.mp4?raw=true" type="video/mp4">
            </video>
            <a href="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/oshi%20no%20ko%201.mp4?raw=true" class="download-button" download>🕳️🪽 Télécharger</a>
        </div>

        <!-- Dandadan -->
        <div class="video-card">
            <img src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/dandan.jpg?raw=true" alt="Dandadan">
            <h2>Dandadan</h2>
            <a href="#" class="play-button" onclick="playVideo(event, 'video6')">▶ Play la vidéo</a>
            <video id="video6" controls>
                <source src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/danddanddab.mp4?raw=true" type="video/mp4">
            </video>
            <a href="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/danddanddab.mp4?raw=true" class="download-button" download>🕳️🪽 Télécharger</a>
        </div>
    </div>

    <script>
        function playVideo(event, videoId) {
            event.preventDefault();
            var allVideos = document.querySelectorAll('video');
            allVideos.forEach(function(video) {
                video.pause();
                video.style.display = "none";
            });

            var video = document.getElementById(videoId);
            video.style.display = "block";
            video.play();
        }
    </script>
</body>
</html>