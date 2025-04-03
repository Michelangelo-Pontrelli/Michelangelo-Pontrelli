# Michrelangelo-Pontrelli
HI EVERYONE!

<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Michelangelo Pontrelli - Portfolio</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #ff7eb3, #ff758c);
            color: white;
        }
        .container {
            max-width: 800px;
            margin: auto;
            padding: 20px;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 15px;
            box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.2);
        }
        h1, h2 {
            color: #fff;
        }
        ul {
            list-style-type: none;
            padding: 0;
        }
        li {
            padding: 5px;
        }
        .icons a {
            margin: 10px;
            text-decoration: none;
            font-size: 24px;
            color: #fff;
        }
        #counter {
            font-size: 18px;
            margin-top: 20px;
            font-weight: bold;
        }
        #game {
            margin-top: 20px;
        }
        .button {
            padding: 10px 20px;
            background-color: #fff;
            color: #ff758c;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            font-weight: bold;
        }
        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 3px solid white;
        }
    </style>
</head>
<body>
    <div class="container">
        <img src="profile.jpg" alt="Michelangelo Pontrelli" class="profile-img">
        <h1>👨‍💻 Michelangelo Pontrelli</h1>
        <p>Appassionato di videogiochi e informatica, specializzato nello sviluppo back-end.</p>
        <h2>💡 Competenze</h2>
        <ul>
            <li>🔹 HTML, CSS, JavaScript</li>
            <li>🔹 Java, PHP (base), Laravel?</li>
            <li>🔹 MySQL</li>
        </ul>
        <h2>📜 Esperienze</h2>
        <p>Attestato di Full Stack Developer (Java) e due progetti importanti.</p>
        <h2>🔗 Contatti</h2>
        <div class="icons">
            <a href="#" target="_blank">🔗 GitHub</a>
            <a href="#" target="_blank">💼 LinkedIn</a>
            <a href="mailto:tuamail@example.com">📧 Email</a>
        </div>
        <h2>👀 Visite al sito</h2>
        <p id="counter">0</p>
        <h2>🎮 Mini Gioco</h2>
        <div id="game">
            <button class="button" onclick="playGame()">Cliccami!</button>
            <p id="gameMessage"></p>
        </div>
    </div>
    <script>
        // Contatore visitatori (simulazione)
        let count = localStorage.getItem('visitCount') || 0;
        count++;
        localStorage.setItem('visitCount', count);
        document.getElementById('counter').innerText = count;

        // Mini gioco
        function playGame() {
            document.getElementById('gameMessage').innerText = "Hai vinto! 🎉";
        }
    </script>
</body>
</html>
