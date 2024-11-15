<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Online Games Hub</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <h1>Welcome to Online Games Hub</h1>
            <nav>
                <ul>
                    <li><a href="#poki-games">Poki Games</a></li>
                    <li><a href="#crazy-games">Crazy Games</a></li>
                    <li><a href="#1v1lol">1v1.LOL</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Main Content -->
    <main>
        <!-- Poki Games Section -->
        <section id="poki-games">
            <h2>Poki Games</h2>
            <div class="game-container">
                <div class="game-card">
                    <iframe src="https://www.poki.com/en/g/retro-bowl" title="Retro Bowl" allowfullscreen></iframe>
                    <p>Retro Bowl</p>
                </div>
                <div class="game-card">
                    <iframe src="https://www.poki.com/en/g/retro-golf" title="Retro Golf" allowfullscreen></iframe>
                    <p>Retro Golf</p>
                </div>
            </div>
        </section>

        <!-- Crazy Games Section -->
        <section id="crazy-games">
            <h2>Crazy Games</h2>
            <div class="game-container">
                <div class="game-card">
                    <iframe src="https://www.crazygames.com/game/tower-defense-kingdom" title="Tower Defense Kingdom" allowfullscreen></iframe>
                    <p>Tower Defense Kingdom</p>
                </div>
                <div class="game-card">
                    <iframe src="https://www.crazygames.com/game/krunker-io" title="Krunker.io" allowfullscreen></iframe>
                    <p>Krunker.io</p>
                </div>
            </div>
        </section>

        <!-- 1v1.LOL Section -->
        <section id="1v1lol">
            <h2>Play 1v1.LOL</h2>
            <p>Click below to play the famous 1v1.LOL game!</p>
            <a href="https://1v1.lol/" target="_blank" class="play-button">Play 1v1.LOL</a>
        </section>
    </main>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2024 Online Games Hub | All Rights Reserved</p>
        </div>
    </footer>

    <script src="script.js"></script>
</body>
</html>
/* Global Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    color: #333;
}

/* Header Styling */
header {
    background-color: #333;
    color: #fff;
    padding: 10px 0;
    text-align: center;
}

header h1 {
    margin: 0;
    font-size: 2em;
}

nav ul {
    list-style-type: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
    font-size: 1.1em;
}

nav ul li a:hover {
    text-decoration: underline;
}

/* Main Content */
main {
    padding: 20px;
}

/* Game Section */
section {
    margin-bottom: 30px;
}

h2 {
    font-size: 1.8em;
    text-align: center;
    margin-bottom: 20px;
}

.game-container {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    gap: 20px;
}

.game-card {
    width: 250px;
    text-align: center;
    background-color: #fff;
    padding: 15px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
}

.game-card iframe {
    width: 100%;
    height: 200px;
    border-radius: 8px;
}

.game-card p {
    margin-top: 10px;
    font-size: 1.2em;
}

/* Play Button for 1v1.LOL */
.play-button {
    display: inline-block;
    padding: 10px 20px;
    background-color: #4CAF50;
    color: #fff;
    font-size: 1.2em;
    text-decoration: none;
    border-radius: 5px;
    margin-top: 20px;
}

.play-button:hover {
    background-color: #45a049;
}

/* Footer Styles */
footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 10px 0;
}

/* Responsive Design */
@media (max-width: 768px) {
    .game-container {
        flex-direction: column;
        align-items: center;
    }

    .game-card {
        width: 90%;
    }
}
document.addEventListener("DOMContentLoaded", () => {
    const games = document.querySelectorAll('.game-card');

    games.forEach(game => {
        game.addEventListener('click', () => {
            alert('Enjoy the game!');
        });
    });
});
