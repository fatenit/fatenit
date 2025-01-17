💢FATENIT🪽
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ma Page Vidéo</title>
    <!-- Google tag (gtag.js) -->
    <script async src="https://www.googletagmanager.com/gtag/js?id=G-NR6N2SFPSD"></script>
    <script>
      window.dataLayer = window.dataLayer || [];
      function gtag(){dataLayer.push(arguments);}
      gtag('js', new Date());

      gtag('config', 'G-NR6N2SFPSD');
    </script>

    <style>
        /* Styles identiques */
    </style>
</head>
<body>
    <h1>Bienvenue 🤧✨ Opening gratuit</h1>

    <div class="profile">
        <img src="https://raw.githubusercontent.com/fatenit/fatenit/7c2d0cadb356838482ad2638b63c88137fe94c58/file-EGrZGMs3WV5mgdC4QSABj1.webp" alt="Mon profil">
        <h2>Mon Profil</h2>
    </div>

    <div class="video-container">
        <!-- Solo Leveling et Chainsaw Man (existants) -->

        <!-- Bestars -->
        <div class="video-card">
            <img src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/Beastars_Anime_Cover_1.jpg" alt="Beastars">
            <h2>Beastars</h2>
            <a href="#" class="play-button" onclick="playVideo(event, 'video3')">▶ Play Vidéo 1</a>
            <video id="video3" controls>
                <source src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/beastars1.mp4" type="video/mp4">
            </video>
            <a href="#" class="play-button" onclick="playVideo(event, 'video4')">▶ Play Vidéo 2</a>
            <video id="video4" controls>
                <source src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/beastar2.mp4" type="video/mp4">
            </video>
        </div>

        <!-- Charngri la frontière -->
        <div class="video-card">
            <img src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/chnagro%20la.jpg" alt="Charngri la frontière">
            <h2>Charngri la frontière</h2>
            <a href="#" class="play-button" onclick="playVideo(event, 'video5')">▶ Play Vidéo 1</a>
            <video id="video5" controls>
                <source src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/1%20changrila.mp4" type="video/mp4">
            </video>
            <a href="#" class="play-button" onclick="playVideo(event, 'video6')">▶ Play Vidéo 2</a>
            <video id="video6" controls>
                <source src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/2%20changrila.mp4" type="video/mp4">
            </video>
        </div>

        <!-- Oshi no Ko -->
        <div class="video-card">
            <img src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/oshi%20no%20ko.jpg" alt="Oshi no Ko">
            <h2>Oshi no Ko</h2>
            <a href="#" class="play-button" onclick="playVideo(event, 'video7')">▶ Play Vidéo 1</a>
            <video id="video7" controls>
                <source src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/oshi%20no%20ko%201.mp4" type="video/mp4">
            </video>
            <a href="#" class="play-button" onclick="playVideo(event, 'video8')">▶ Play Vidéo 2</a>
            <video id="video8" controls>
                <source src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/oshi%20no%20ko%202.mp4" type="video/mp4">
            </video>
        </div>

        <!-- Dandadan -->
        <div class="video-card">
            <img src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/dandan.jpg" alt="Dandadan">
            <h2>Dandadan</h2>
            <a href="#" class="play-button" onclick="playVideo(event, 'video9')">▶ Play la Vidéo</a>
            <video id="video9" controls>
                <source src="https://github.com/fatenit/open/blob/a81af92122f5b6fa63fa6f9b60f8db33d7a92b1f/danddanddab.mp4" type="video/mp4">
            </video>
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