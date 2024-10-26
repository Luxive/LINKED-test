<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LINKED!</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: Arial, sans-serif;
            background-color: #121212;
            color: white;
            display: flex;
            height: 100vh;
            overflow: hidden;
        }
        .sidebar {
            width: 250px;
            background: linear-gradient(135deg, #3a3a3a, #1e1e1e);
            padding: 20px;
            box-shadow: 2px 0 10px rgba(0, 0, 0, 0.5);
            overflow-y: auto;
        }
        .sidebar h2 {
            color: #1abc9c;
            margin-bottom: 40px;
            font-size: 1.8rem;
            text-align: center;
        }
        .sidebar a {
            display: block;
            color: white;
            padding: 12px;
            margin: 8px 0;
            text-decoration: none;
            font-size: 1.1rem;
            background-color: #333;
            border-radius: 8px;
            transition: background 0.3s, transform 0.2s;
        }
        .sidebar a:hover {
            background-color: #1abc9c;
            transform: scale(1.05);
        }
        .main-content {
            flex: 1;
            padding: 20px;
            background-color: #262626;
            overflow-y: auto;
            display: none;
        }
        .main-content.active {
            display: block;
        }
        .main-content h1 {
            font-size: 2.2rem;
            color: #1abc9c;
            margin-bottom: 20px;
        }
        .accordion {
            width: 100%;
            background-color: #444;
            border: none;
            color: white;
            padding: 18px;
            text-align: left;
            font-size: 18px;
            cursor: pointer;
            transition: background-color 0.3s;
            border-radius: 8px;
            margin-bottom: 10px;
        }
        .accordion:hover {
            background-color: #1abc9c;
        }
        .accordion.active {
            background-color: #1abc9c;
        }
        .accordion:after {
            content: '\002B';
            font-size: 20px;
            float: right;
            color: white;
        }
        .accordion.active:after {
            content: "\2212";
        }
        .panel {
            padding: 0 18px;
            background-color: #333;
            display: none;
            overflow: hidden;
            border-radius: 0 0 8px 8px;
        }
        .panel a {
            display: block;
            color: #1abc9c;
            margin: 10px 0;
            text-decoration: none;
        }
        .panel a:hover {
            text-decoration: underline;
        }
        footer {
            text-align: center;
            padding: 20px;
            color: #ccc;
            background-color: #1e1e1e;
            border-top: 1px solid #333;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="sidebar">
        <h2>LINKED!</h2>
        <a onclick="showSection('home')">Home</a>
        <a onclick="showSection('proxies')">Proxies</a>
        <a onclick="showSection('games')">Games</a>
        <a onclick="showSection('movies')">Movies</a>
        <a onclick="showSection('multipurpose')">Education</a>
        <a onclick="showSection('coder')">Coder Stuff</a>
        <a onclick="showSection('credits')">Credits</a>
        <a onclick="showSection('proxy')">Make a Proxy</a>
    </div>

<div id="home" class="main-content active">
        <h1>Welcome to LINKED!</h1>
        <p>Select a category from the sidebar to get started.</p>
    </div>

<div id="proxies" class="main-content">
        <h1>Proxies</h1>
        <button class="accordion">Rammerhead</button>
        <div class="panel">
            <a href="#">Link 1 for RammerHead</a>
            <a href="#">Link 2 for RammerHead</a>
        </div>
        <button class="accordion">Interstellar</button>
        <div class="panel">
            <a href="#">Link 1 for Interstellar</a>
            <a href="#">Link 2 for Interstellar</a>
        </div>
    </div>

 <div id="games" class="main-content">
        <h1>Games</h1>
        <button class="accordion">Extreme math</button>
        <div class="panel">
            <a href="https://tutoring4free.org/">Extreme math Link 1</a>
            <a href="https://easytutoring.app/">Extreme math link 2</a>
            <a href="https://extrememath.dev/">Extreme math link 3</a>
            <a href="https://simply-history.xyz/#google_vignette">Extreme math link 4</a>
            <a href="https://extrememath.org/">Extreme math link 5</a>
            <a href="https://simple-education.xyz/#google_vignette">Extreme math link 6</a>
        </div>
        <button class="accordion">Minecraft</button>
        <div class="panel">
            <a href="https://g.deev.is/">Minecraft link 1</a>
            <a href="https://eaglercraft.q13x.com/">Minecraft link 2</a>
            <a href="https://ubg100.github.io/eaglercraft.html">Minecraft link 3</a>
            <a href="https://burritoedition.github.io/emu/Minecraft/web/index.html">Minecraft link 4</a>
            <a href="https://reslauncher.vercel.app/">Minecraft link 5</a>
            <a href="https://sd592g.github.io/zj684od4lfg/">Minecraft link 6</a>
            <a href="https://eagler.almondnet.cn/Nebula.html">Minecraft link 7</a>
            <a href="https://mess.eu.org/">Minecraft link 8</a>
            <a href="https://precisionclient-88k.pages.dev/">Minecraft link 9</a>
        </div>
        <button class="accordion">Google sites</button>
        <div class="panel">
            <a href="https://sites.google.com/site/tyronesgameshack/">Tyrones games link 1</a>
            <a href="https://sites.google.com/site/unblockedgames66ez/">Unblocked games 66 link 2</a>
            <a href="https://sites.google.com/site/unblockedgame76/">Unblocked games 76 link 3</a>
            <a href="https://sites.google.com/view/games-unblockedd/">games unblocked link 4</a>
            <a href="https://sites.google.com/site/classroom6x/unblockedgames">Classroom6x link 5</a>
            <a href="https://sites.google.com/view/games-unblocked/">games unblocked2 link 6</a>
            <a href="https://sites.google.com/site/thegamecompilation/home?authuser=0">unblocked games world link 7</a>
        </div>
    </div>

<div id="movies" class="main-content">
        <h1>Movies</h1>
        <button class="accordion">Movies</button>
        <div class="panel">
            <a href="https://hdtoday.tv/filter?type=tv&quality=all&release_year=all&genre=3&country=all&page=46">HDTODAY link 1</a>
            <a href="https://genesishd.tv/">HDTODAY link 2</a>
            <a href="https://hdtoday.cc/">HDTODAY link 3</a>
        </div>
    </div>

<div id="multipurpose" class="main-content">
        <h1>Education</h1>
        <button class="accordion">Tools</button>
        <div class="panel">
            <a href="https://chatgpt.com/">CHATGPT</a>
        </div>
    </div>

 <div id="coder" class="main-content">
        <h1>Coder Stuff</h1>
        <button class="accordion">Coding Resources</button>
        <div class="panel">
            <a href="#">Resource Link 1</a>
        </div>
    </div>

 <div id="credits" class="main-content">
        <h1>Credits</h1>
        <button class="accordion">Acknowledgements</button>
        <div class="panel">
            <a href="#">Credit Link 1</a>
        </div>
    </div>

<div id="proxy" class="main-content">
        <h1>Make a Proxy</h1>
        <button class="accordion">Guides</button>
        <div class="panel">
            <a href="#">Proxy Guide Link 1</a>
        </div>
    </div>

   <footer>
        <p>&copy; 2024 LINKED! | All Rights Reserved</p>
    </footer>

 <script>
        function showSection(sectionId) {
            var sections = document.getElementsByClassName("main-content");
            for (var i = 0; i < sections.length; i++) {
                sections[i].classList.remove("active");
            }
            document.getElementById(sectionId).classList.add("active");
        }

        var acc = document.getElementsByClassName("accordion");
        for (var i = 0; i < acc.length; i++) {
            acc[i].addEventListener("click", function() {
                this.classList.toggle("active");
                var panel = this.nextElementSibling;
                if (panel.style.display === "block") {
                    panel.style.display = "none";
                } else {
                    panel.style.display = "block";
                }
            });
        }
    </script>
</body>
</html>
