<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Made In Abyss - Thông tin phim</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #1c1c1c;
            color: #dcdcdc;
            margin: 0;
            padding: 0;
        }
        .container {
            max-width: 1200px;
            margin: auto;
            padding: 20px;
        }
        .header {
            background-color: #282828;
            padding: 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .header h1 {
            margin: 0;
            color: #fff;
        }
        .header button {
            background-color: #e74c3c;
            color: white;
            border: none;
            padding: 10px 20px;
            cursor: pointer;
        }
        .header button:hover {
            background-color: #c0392b;
        }
        .content {
            display: flex;
            margin-top: 20px;
        }
        .poster {
            flex: 1;
            text-align: center;
        }
        .poster img {
            max-width: 100%;
            border-radius: 10px;
        }
        .details {
            flex: 2;
            margin-left: 20px;
        }
        .details h2 {
            margin: 0;
            color: #fff;
        }
        .details p {
            margin-top: 10px;
            font-size: 16px;
        }
        .info {
            margin-top: 20px;
        }
        .info table {
            width: 100%;
            border-collapse: collapse;
        }
        .info table th, .info table td {
            border: 1px solid #555;
            padding: 10px;
            text-align: left;
        }
        .info table th {
            background-color: #333;
        }

        /* Tabs Styles */
        .tabs {
            margin-top: 40px;
        }
        .tabs ul {
            list-style: none;
            padding: 0;
            display: flex;
            background-color: #333;
            border-radius: 10px;
            overflow: hidden;
        }
        .tabs ul li {
            flex: 1;
            text-align: center;
        }
        .tabs ul li a {
            display: block;
            padding: 10px;
            color: #fff;
            text-decoration: none;
            background-color: #333;
        }
        .tabs ul li a:hover, .tabs ul li a.active {
            background-color: #e74c3c;
        }
        .tab-content {
            display: none;
            padding: 20px;
            background-color: #282828;
            margin-top: 20px;
            border-radius: 10px;
        }
        .tab-content.active {
            display: block;
        }
        .video-section {
            display: flex;
            justify-content: center; /* Căn giữa theo chiều ngang */
            align-items: center; /* Căn giữa theo chiều dọc nếu cần */
            padding: 10px;
        }
        .video-section iframe {
            width: 100%; 
            height: auto; 
            aspect-ratio: 16/9; 
        }
        .footer {
            margin-top: 40px;
            padding: 20px;
            background-color: #333;
            text-align: center;
            color: #999;
        }
        .footer a {
            color: #e74c3c;
            text-decoration: none;
        }
        .footer a:hover {
            text-decoration: underline;
        }
        .characters {
            display: flex;
            gap: 20px;
            flex-wrap: wrap;
            justify-content: space-around;
        }
        .character {
            text-align: center;
            color: #fff;
        }
        .character img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            object-fit: cover;
            background-color: #444;
        }
        .character p {
            margin-top: 10px;
            font-size: 14px;
        }
        /* Phim khác Styles */
        .related-movies {
            margin-top: 40px;
            width: 100%;
        }
        .related-movies h2 {
            text-align: center;
            color: #e74c3c;
        }
        .movies-grid {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 10px;
        }
        .movie {
            flex: 1 1 calc(25% - 10px);
            margin-bottom: 20px;
            cursor: pointer;
        }
        .movie img {
            width: 100%;
            border-radius: 10px;
            object-fit: cover;
        }
        .movie-title {
            text-align: center;
            margin-top: 10px;
            color: #fff;
        }
    </style>
</head>
<body>

    <div class="header">
        <h1>Attack On Titan</h1>
    </div>

    <div class="container">
        <div class="content">
            <div class="poster">
                <img src="https://static.wikia.nocookie.net/attack-on-titan/images/b/b4/%C4%90%E1%BA%A1i_chi%E1%BA%BFn_Titan_M%C3%B9a_1.jpg/revision/latest?cb=20220502203959&path-prefix=vi" alt="Attack On Titan">
            </div>
            <div class="details">
                <h2>Đến Từ Abyss</h2>
                <p>
                    "Hệ thống hang động không lồ, nơi duy nhất trên thế giới còn chưa được khám phá, chính là 
                    cuộc hành trình đến với đáy vực Abyss. Không ai biết có gì nằm sâu dưới đáy vực, nhưng bao 
                    cuộc đời đã được cống hiến để khám phá điều đó. Nhiều nhà thám hiểm đã đâm sâu vào nơi này 
                    nhưng không phải ai cũng trở về. Riko, một cô bé sống ở tầng đầu tiên, quyết tâm tìm kiếm 
                    mẹ mình và bắt đầu cuộc hành trình xuống dưới cùng với một người bạn robot..."
                </p>
                <p><strong>Thời lượng:</strong> 13 tập</p>
                <p><strong>Ngày phát hành:</strong> 2017</p>
            </div>
        </div>

        <!-- Tabs Section -->
        <div class="tabs">
            <ul>
                <li><a href="#" class="active" onclick="showTab(event, 'info')">Thông tin phim</a></li>
                <li><a href="#" onclick="showTab(event, 'characters')">Nhân vật</a></li>
                <li><a href="#" onclick="showTab(event, 'trailer')">Trailer</a></li>
                <li><a href="#" onclick="showTab(event, 'gallery')">Hình ảnh</a></li>
            </ul>

            <div id="info" class="tab-content active">
                <h3>Thông tin chi tiết về Made In Abyss</h3>
                <table>
                    <tr>
                        <th style="width: 30%;">Thể loại</th>
                        <td>Anime, Fantasy, Adventure, Mystery</td>
                    </tr>
                    <tr>
                        <th style="width: 30%;">Trạng thái</th>
                        <td>Hoàn thành</td>
                    </tr>
                    <tr>
                        <th style="width: 30%;">Đạo diễn</th>
                        <td>Masayuki Kojima</td>
                    </tr>
                    <tr>
                        <th style="width: 30%;">Ngôn ngữ</th>
                        <td>Tiếng Nhật (VietSub)</td>
                    </tr>
                    <tr>
                        <th style="width: 30%;">Độ tuổi</th>
                        <td>R - 17+ (Bạo lực và ngôn từ)</td>
                    </tr>
                    <tr>
                        <th style="width: 30%;">Studio</th>
                        <td>Kinema Citrus</td>
                    </tr>
                    <tr>
                        <th style="width: 30%;">Chất lượng</th>
                        <td>HD</td>
                    </tr>
                </table>
            </div>
            

            <div id="characters" class="tab-content">
                <h3>Nhân vật chính</h3>
                <div class="characters">
                    <!-- Character 1 -->
                    <div class="character">
                        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSw_obfeQbzVXmc7T8nr6GaiilWPLpkkF-uTQ&s" alt="Regu">
                        <p>Reg</p>
                    </div>
                    <!-- Character 2 -->
                    <div class="character">
                        <img src="https://static.wikia.nocookie.net/madeinabyss/images/0/08/Anime_Riko_Square.png/revision/latest?cb=20190326030020" alt="Riko">
                        <p>Riko</p>
                    </div>
                    <!-- Character 3 -->
                    <div class="character">
                        <img src="https://static.wikia.nocookie.net/vsbattles/images/8/82/Nanachi.png/revision/latest?cb=20220923072745" alt="Nanachi">
                        <p>Nanachi</p>
                    </div>
                    <!-- Add more characters as needed -->
                </div>
            </div>

            <div id="trailer" class="tab-content">
                <h3>Trailer phim</h3>
                <div class="video-section">
                    <iframe src="https://www.youtube.com/embed/kqBNQEUI8dM?si=eqS8___KAtfJUYTR" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
                </div>
            </div>

            <div id="gallery" class="tab-content">
                <h3>Hình ảnh nổi bật</h3>
                <img src="https://formeinfullbloom.wordpress.com/wp-content/uploads/2017/12/riko3.png" alt="Gallery Image 1" style="width: 100%; margin-top: 10px;">
                <img src="https://images.danet.vn/images/src/f4/b1a/d490fbf46469b452fa018086122cde89.jpg" alt="Gallery Image 2" style="width: 100%; margin-top: 10px;">
                <img src="https://imgsrv.crunchyroll.com/cdn-cgi/image/fit=contain,format=auto,quality=85,width=1200,height=675/catalog/crunchyroll/532d3659db86ed0d86fcc57ef38acc45.jpe" alt="Gallery Image 3" style="width: 100%; margin-top: 10px;">
                <img src="https://img.tripi.vn/cdn-cgi/image/width=700,height=700/https://gcs.tripi.vn/public-tripi/tripi-feed/img/476318szl/anh-mo-ta.png" alt="Gallery Image 4" style="width: 100%; margin-top: 10px;">
                <img src="https://static.wikia.nocookie.net/madeinabyss/images/3/3d/Slider-Characters.png/revision/latest/scale-to-width-down/500?cb=20220123025511" alt="Gallery Image 5" style="width: 100%; margin-top: 10px;">
                <img src="https://www.siliconera.com/wp-content/uploads/2021/11/madeinabyss.jpg?fit=767%2C432" alt="Gallery Image 6" style="width: 100%; margin-top: 10px;">
            </div>
        </div>
    </div>
    <div class="related-movies">
        <h2>Phim khác bạn có thể xem</h2>
        <div class="movies-grid">
            <!-- Movie 1 -->
            <div class="movie" onclick="window.location.href='movie1.html'">
                <img src="https://static.wikia.nocookie.net/attack-on-titan/images/b/b4/%C4%90%E1%BA%A1i_chi%E1%BA%BFn_Titan_M%C3%B9a_1.jpg/revision/latest?cb=20220502203959&path-prefix=vi" alt="Movie 1">
                <p class="movie-title">Attack on Titan</p>
            </div>
            <!-- Movie 2 -->
            <div class="movie" onclick="window.location.href='movie2.html'">
                <img src="https://static.wikia.nocookie.net/fma/images/c/ca/Fma2_intro.jpg/revision/latest?cb=20140602095111" alt="Movie 2">
                <p class="movie-title">Fullmetal Alchemist</p>
            </div>
            <!-- Movie 3 -->
            <div class="movie" onclick="window.location.href='movie3.html'">
                <img src="https://dw9to29mmj727.cloudfront.net/products/782009238652.jpg" alt="Movie 3">
                <p class="movie-title">Naruto</p>
            </div>
            <!-- Movie 4 -->
            <div class="movie" onclick="window.location.href='movie4.html'">
                <img src="https://pic0.iqiyipic.com/image/20240618/f2/2e/a_100421840_m_601_en_m6_260_360.jpg" alt="Movie 4">
                <p class="movie-title">One Piece</p>
            </div>
            <!-- Movie 5 -->
            <div class="movie" onclick="window.location.href='movie5.html'">
                <img src="https://resizing.flixster.com/-XZAfHZM39UwaGJIFWKAE8fS0ak=/v3/t/assets/p12793542_b_v13_ak.jpg" alt="Movie 5">
                <p class="movie-title">My Hero Academia</p>
            </div>
            <!-- Movie 6 -->
            <div class="movie" onclick="window.location.href='movie6.html'">
                <img src="https://m.media-amazon.com/images/M/MV5BN2NhYzU2NDEtYzI1NS00MjgzLThjZGUtOTYxNGJkZjZmNDdjXkEyXkFqcGc@._V1_FMjpg_UX1000_.jpg" alt="Movie 6">
                <p class="movie-title">Sword Art Online</p>
            </div>
            <!-- Movie 7 -->
            <div class="movie" onclick="window.location.href='movie7.html'">
                <img src="https://image.api.playstation.com/vulcan/ap/rnd/202106/1704/2ZfAUG5CTXdM34S1OhmMW1zF.jpg" alt="Movie 7">
                <p class="movie-title">Demon Slayer</p>
            </div>
            <!-- Movie 8 -->
            <div class="movie" onclick="window.location.href='movie8.html'">
                <img src="https://m.media-amazon.com/images/M/MV5BYTgyZDhmMTEtZDFhNi00MTc4LTg3NjUtYWJlNGE5Mzk2NzMxXkEyXkFqcGc@._V1_FMjpg_UX1000_.jpg" alt="Movie 8">
                <p class="movie-title">Death Note</p>
            </div>
            <!-- Movie 9 -->
            <div class="movie" onclick="window.location.href='movie9.html'">
                <img src="https://www.justwatch.com/images/poster/311344951/s718/dragon-ball-super.jpg" alt="Movie 9">
                <p class="movie-title">Dragon Ball Super</p>
            </div>
            <!-- Movie 10 -->
            <div class="movie" onclick="window.location.href='movie10.html'">
                <img src="https://image.api.playstation.com/vulcan/ap/rnd/202007/1308/StbziMS5VEhNntVpqjIRyOl1.png" alt="Movie 10">
                <p class="movie-title">Fairy Tail</p>
            </div>
            <!-- Movie 11 -->
            <div class="movie" onclick="window.location.href='movie11.html'">
                <img src="https://m.media-amazon.com/images/M/MV5BYzYxOTlkYzctNGY2MC00MjNjLWIxOWMtY2QwYjcxZWIwMmEwXkEyXkFqcGc@._V1_FMjpg_UX1000_.jpg" alt="Movie 11">
                <p class="movie-title">Hunter x Hunter</p>
            </div>
            <!-- Movie 12 -->
            <div class="movie" onclick="window.location.href='movie12.html'">
                <img src="https://yvolve.shop/cdn/shop/files/GBYDCO630.jpg?v=1716466240" alt="Movie 12">
                <p class="movie-title">Bleach</p>
            </div>
            <!-- Movie 13 -->
            <div class="movie" onclick="window.location.href='movie13.html'">
                <img src="https://m.media-amazon.com/images/M/MV5BZWI2NzZhMTItOTM3OS00NjcyLThmN2EtZGZjMjlhYWMwODMzXkEyXkFqcGc@._V1_.jpg" alt="Movie 13">
                <p class="movie-title">Tokyo Ghoul</p>
            </div>
            <!-- Movie 14 -->
            <div class="movie" onclick="window.location.href='movie14.html'">
                <img src="https://m.media-amazon.com/images/M/MV5BZmZkZjNhMWMtM2U0Mi00MjdlLTk3NmMtMTMwZjgwOTJmODMzXkEyXkFqcGc@._V1_FMjpg_UX1000_.jpg" alt="Movie 14">
                <p class="movie-title">Black Clover</p>
            </div>
            <!-- Movie 15 -->
            <div class="movie" onclick="window.location.href='movie15.html'">
                <img src="https://m.media-amazon.com/images/I/813ek5yvX1L._AC_UF894,1000_QL80_.jpg" alt="Movie 15">
                <p class="movie-title">Code Geass</p>
            </div>
            <!-- Movie 16 -->
            <div class="movie" onclick="window.location.href='movie16.html'">
                <img src="https://m.media-amazon.com/images/M/MV5BMGRiOWQyOTAtZDQ0Ny00NGRiLWIyYTYtZWM1MjNjNzg0ZjE3XkEyXkFqcGc@._V1_.jpg" alt="Movie 16">
                <p class="movie-title">Neon Genesis Evangelion</p>
            </div>
            <!-- Movie 17 -->
            <div class="movie" onclick="window.location.href='movie17.html'">
                <img src="https://m.media-amazon.com/images/M/MV5BZGMyYmFmNzgtMWQ4NS00MWE2LTg4YmEtZGY1MTBiODE0YmE5XkEyXkFqcGc@._V1_FMjpg_UX1000_.jpg" alt="Movie 17">
                <p class="movie-title">Your Lie In April</p>
            </div>
            <!-- Movie 18 -->
            <div class="movie" onclick="window.location.href='movie18.html'">
                <img src="https://external-preview.redd.it/re-zero-season-3-new-key-visual-v0-pEs8RGhSmENJC8bXvh_D390t-0JcshAfoGTb8JOypOw.jpg?auto=webp&s=edcc4cb38a7fc05042af42ffd3e8dadbd08caa3e" alt="Movie 18">
                <p class="movie-title">Re:Zero</p>
            </div>
            <!-- Movie 19 -->
            <div class="movie" onclick="window.location.href='movie19.html'">
                <img src="https://m.media-amazon.com/images/M/MV5BYjNjNDBmZjAtMGZiMS00ODBkLWFjYWItZWQ1ZjEwOGNmZDBjXkEyXkFqcGc@._V1_.jpg" alt="Movie 19">
                <p class="movie-title">Overlord</p>
            </div>
            <!-- Movie 20 -->
            <div class="movie" onclick="window.location.href='movie20.html'">
                <img src="https://m.media-amazon.com/images/M/MV5BNDA3MGNmZTEtMzFiMy00ZmViLThhNmQtMjQ4ZDc5MDEyN2U1XkEyXkFqcGc@._V1_FMjpg_UX1000_.jpg" alt="Movie 20">
                <p class="movie-title">Vinland Saga</p>
            </div>
            <!-- Movie 21 -->
            <div class="movie" onclick="window.location.href='movie21.html'">
                <img src="https://m.media-amazon.com/images/M/MV5BZjI1YjZiMDUtZTI3MC00YTA5LWIzMmMtZmQ0NTZiYWM4NTYwXkEyXkFqcGc@._V1_FMjpg_UX1000_.jpg" alt="Movie 21">
                <p class="movie-title">Steins;Gate</p>
            </div>
            <!-- Movie 22 -->
            <div class="movie" onclick="window.location.href='movie22.html'">
                <img src="https://musicart.xboxlive.com/7/79e65500-0000-0000-0000-000000000002/504/image.jpg" alt="Movie 22">
                <p class="movie-title">Gintama</p>
            </div>
            <!-- Movie 23 -->
            <div class="movie" onclick="window.location.href='movie23.html'">
                <img src="https://i.redd.it/g99hidftyfi91.jpg" alt="Movie 23">
                <p class="movie-title">One Punch Man</p>
            </div>
            <!-- Movie 24 -->
            <div class="movie" onclick="window.location.href='movie24.html'">
                <img src="https://m.media-amazon.com/images/M/MV5BYzU3NDM4ZjgtY2UyMi00YTczLTgyNDEtMjBiMDJlOGUxNjcxXkEyXkFqcGc@._V1_.jpg" alt="Movie 24">
                <p class="movie-title">Mob Psycho 100</p>
            </div>
            <!-- Movie 25 -->
            <div class="movie" onclick="window.location.href='movie25.html'">
                <img src="https://m.media-amazon.com/images/M/MV5BMGQ4ZGJhZTUtZDQ5Mi00NTI1LWEyYjItMzIxM2VlNmY4MDEyXkEyXkFqcGc@._V1_FMjpg_UX1000_.jpg" alt="Movie 25">
                <p class="movie-title">The Promised Neverland</p>
            </div>
            <!-- Movie 25 -->
            <div class="movie" onclick="window.location.href='movie25.html'">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRjjydKUpH1rz3V2N2oTcKX7O3QIMkH_-xqqw&s" alt="Movie 26">
                <p class="movie-title">Solo Leveling</p>
            </div>
            <!-- Movie 25 -->
            <div class="movie" onclick="window.location.href='movie25.html'">
                <img src="https://m.media-amazon.com/images/M/MV5BZjM4ODA5YTktNjliMC00NzI5LTk3ZTctZWYyYWEyNTJhMmQzXkEyXkFqcGc@._V1_.jpg" alt="Movie 27">
                <p class="movie-title">Made In Abyss</p>
            </div>
            <!-- Movie 25 -->
            <div class="movie" onclick="window.location.href='movie25.html'">
                <img src="https://m.media-amazon.com/images/M/MV5BMThhODExMTUtZmIyMC00OTY4LTk5YWMtN2YxYWRhNmNiNDNmXkEyXkFqcGc@._V1_.jpg" alt="Movie 28">
                <p class="movie-title">Fire Force</p>
            </div>
        </div>
    </div>
    <div class="footer">
        <p>Theo dõi các cập nhật mới nhất tại <a href="#">Facebook</a> hoặc <a href="#">Telegram</a>.</p>
    </div>

    <script>
        function showTab(event, tabName) {
            event.preventDefault();
            var tabs = document.getElementsByClassName('tab-content');
            for (var i = 0; i < tabs.length; i++) {
                tabs[i].classList.remove('active');
            }
            var links = document.querySelectorAll('.tabs ul li a');
            for (var j = 0; j < links.length; j++) {
                links[j].classList.remove('active');
            }
            document.getElementById(tabName).classList.add('active');
            event.currentTarget.classList.add('active');
        }
    </script>

</body>
</html>
