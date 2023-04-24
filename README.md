<!DOCTYPE html>

<html>
<link rel="stylesheet" href="css/style.css">

<head>
    <title>Podcast App</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" type="text/css" href="style.css">
</head>

<body>
    <header>
        <div class="logo">
            <h1>Podcast App</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="/podacsts">Podcasts</a></li>
                <li><a href="#">Favorites</a></li>
                <li><a href="loginpg.html">Login</a></li>
                <li><a href="signuppg.html">Signup</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <div class="search">
            <input type="text" placeholder="Search for podcasts...">
            <button type="submit">Search</button>
        </div>

        <section class="popular-podcasts">
            <h2>Popular Podcasts</h2>
            <ul>
                <li>
                    <img src="https://via.placeholder.com/150" alt="Podcast Image">
                    <h3>Podcast Name</h3>
                    <p>Podcast Description</p>
                </li>
                <li>
                    <img src="https://via.placeholder.com/150" alt="Podcast Image">
                    <h3>Podcast Name</h3>
                    <p>Podcast Description</p>
                </li>
                <li>
                    <img src="https://via.placeholder.com/150" alt="Podcast Image">
                    <h3>Podcast Name</h3>
                    <p>Podcast Description</p>
                </li>
            </ul>
        </section>

        <section class="podcast-player">
            <h2>Podcast Player</h2>
            <div class="player-controls">
                <button class="play">Play</button>
                <button class="pause">Pause</button>
                <button class="stop">Stop</button>
                <button class="forward">Forward 10s</button>
                <button class="backward">Backward 10s</button>
            </div>
            <div class="podcast-details">
                <h3>Podcast Name</h3>
                <p>Podcast Description</p>
            </div>
            <audio src="podcast.mp3"></audio>
        </section>
    </main>

    <footer>
        <p>&copy; 2023 Podcast App. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #333;
            color: #fff;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 10px;
        }

        .logo {
            font-size: 24px;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-right: 20px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
        }

        main {
            margin: 20px;
        }

        .search {
            display: flex;
            margin-bottom: 20px;
        }

        .search input {
            flex: 1;
            padding: 10px;
        }

        .search button {
            background-color: #333;
            color: #fff;
            border: none;
            padding: 10px 20px;
            cursor: pointer;
        }

        .podcast-card {
            display: flex;
            margin-bottom: 20px;
            border: 1px solid #ddd;
            padding: 10px;
        }

        .podcast-card img {
            max-width: 150px;
            margin-right: 20px;
        }

        .podcast-card h2 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .podcast-card p {
            font-size: 14px;
            color: #666;
            margin-bottom: 10px;
        }

        .favorite {
            color: red;
        }

        .player {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }

        .player audio,
        .player video {
            flex: 1;
        }

        .player button {
            background-color: #333;
            color: #fff;
            border: none;
            padding: 10px 20px;
            margin-left: 10px;
            cursor: pointer;
        }

        @media (max-width: 768px) {
            header {
                flex-direction: column;
            }

            .logo {
                margin-bottom: 10px;
            }

            nav ul {
                margin-top: 10px;
                justify-content: center;
            }

            .search {
                flex-direction: column;
                align-items: center;
                text-align: center;
            }

            .search input {
                width: 100%;
            }

            .podcast-card {
                flex-direction: column;
            }

            .podcast-card img {
                margin-right: 0;
                margin-bottom: 10px;
            }

            .player {
                flex-direction: column;
                align-items: flex-start;
            }

            .player button {
                margin-left: 0;
                margin-top: 10px;
            }

            #popular-podcasts {
                margin: 20px;
            }

            #popular-podcasts h2 {
                font-size: 24px;
                margin-bottom: 10px;
            }

            .podcast-list {
                display: flex;
                flex-wrap: wrap;
            }

            .podcast-item {
                width: 300px;
                margin-right: 20px;
                margin-bottom: 20px;
                padding: 10px;
                background-color: #f5f5f5;
                border-radius: 5px;
            }

            .podcast-item h3 {
                font-size: 18px;
                margin-bottom: 5px;
            }

            .podcast-item p {
                font-size: 14px;
                margin-bottom: 10px;
            }

            .podcast-item a {
                display: block;
                font-size: 14px;
                text-align: right;
            }

            @media (max-width: 768px) {
                .podcast-item {
                    width: 100%;
                    margin-right: 0;
                }
            }

        }
    </style>
    <script>src="dbforpodif.js"</script>
    <script src="asp.js"></script>
</body>
</html>
