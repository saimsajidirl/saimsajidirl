<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Muhammad Saim Sajid - GitHub Profile</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap');

        :root {
            --primary-color: #3776AB;
            --secondary-color: #092E20;
            --accent-color: #ff1709;
            --background-color: #0d1117;
            --text-color: #c9d1d9;
            --card-background: #161b22;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Roboto', sans-serif;
            background-color: var(--background-color);
            color: var(--text-color);
            line-height: 1.6;
            padding: 20px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
        }

        header {
            text-align: center;
            margin-bottom: 40px;
        }

        h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            color: var(--primary-color);
        }

        .profile-image {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            object-fit: cover;
            border: 4px solid var(--primary-color);
        }

        .tabs {
            display: flex;
            justify-content: center;
            margin-bottom: 30px;
        }

        .tab {
            padding: 10px 20px;
            background-color: var(--card-background);
            color: var(--text-color);
            border: none;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .tab:hover, .tab:focus {
            background-color: var(--primary-color);
        }

        .tab-content {
            display: none;
            background-color: var(--card-background);
            padding: 20px;
            border-radius: 5px;
            margin-bottom: 30px;
        }

        .tab-content.active {
            display: block;
        }

        .skills {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }

        .skill {
            width: 120px;
            height: 120px;
            position: relative;
        }

        .skill-circle {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            background: conic-gradient(var(--primary-color) var(--percentage), var(--card-background) 0);
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .skill-inner {
            width: 80%;
            height: 80%;
            background-color: var(--card-background);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }

        .social-link {
            color: var(--text-color);
            font-size: 24px;
            transition: color 0.3s;
        }

        .social-link:hover {
            color: var(--primary-color);
        }

        .stats {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 20px;
        }

        .stat-card {
            background-color: var(--card-background);
            padding: 20px;
            border-radius: 5px;
            text-align: center;
            flex: 1;
            min-width: 200px;
        }

        .badges {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
            margin-top: 30px;
        }

        .badge {
            background-color: var(--secondary-color);
            color: var(--text-color);
            padding: 5px 10px;
            border-radius: 15px;
            font-size: 0.8rem;
        }

        footer {
            text-align: center;
            margin-top: 40px;
            font-size: 0.9rem;
            color: var(--text-color);
        }

        @media (max-width: 768px) {
            .tabs {
                flex-direction: column;
            }

            .tab {
                width: 100%;
            }

            .stats {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Hi there 👋, I'm Muhammad Saim Sajid</h1>
            <img src="/api/placeholder/200/200" alt="Profile Picture" class="profile-image">
        </header>

        <div class="tabs">
            <button class="tab" onclick="openTab(event, 'about')">About</button>
            <button class="tab" onclick="openTab(event, 'skills')">Skills</button>
            <button class="tab" onclick="openTab(event, 'stats')">Stats</button>
            <button class="tab" onclick="openTab(event, 'contact')">Contact</button>
        </div>

        <div id="about" class="tab-content active">
            <ul>
                <li>🔭 Currently working with Django</li>
                <li>🌱 Actively expanding my skills in Machine Learning</li>
                <li>💬 Open to inquiries regarding Django; I'm here to assist</li>
                <li>⚡ Fun fact: I embrace a passion for problem-solving and continuous learning</li>
            </ul>
        </div>

        <div id="skills" class="tab-content">
            <div class="skills">
                <div class="skill">
                    <div class="skill-circle" style="--percentage: 90%;">
                        <div class="skill-inner">Python</div>
                    </div>
                </div>
                <div class="skill">
                    <div class="skill-circle" style="--percentage: 85%;">
                        <div class="skill-inner">Django</div>
                    </div>
                </div>
                <div class="skill">
                    <div class="skill-circle" style="--percentage: 80%;">
                        <div class="skill-inner">REST</div>
                    </div>
                </div>
                <div class="skill">
                    <div class="skill-circle" style="--percentage: 75%;">
                        <div class="skill-inner">SQL</div>
                    </div>
                </div>
                <div class="skill">
                    <div class="skill-circle" style="--percentage: 70%;">
                        <div class="skill-inner">HTML</div>
                    </div>
                </div>
                <div class="skill">
                    <div class="skill-circle" style="--percentage: 65%;">
                        <div class="skill-inner">CSS</div>
                    </div>
                </div>
            </div>
        </div>

        <div id="stats" class="tab-content">
            <div class="stats">
                <div class="stat-card">
                    <h3>GitHub Stats</h3>
                    <img src="/api/placeholder/300/150" alt="GitHub Stats">
                </div>
                <div class="stat-card">
                    <h3>Top Languages</h3>
                    <img src="/api/placeholder/300/150" alt="Top Languages">
                </div>
            </div>
        </div>

        <div id="contact" class="tab-content">
            <p>📫 Feel free to reach out via:</p>
            <div class="social-links">
                <a href="https://www.linkedin.com/in/your-profile/" class="social-link">LinkedIn</a>
                <a href="https://www.github.com/saimsajidirl" class="social-link">GitHub</a>
                <a href="https://twitter.com/your-profile" class="social-link">Twitter</a>
                <a href="https://www.youtube.com/@MuhammadSaimDev" class="social-link">YouTube</a>
            </div>
        </div>

        <div class="badges">
            <span class="badge">Python</span>
            <span class="badge">Django</span>
            <span class="badge">REST</span>
            <span class="badge">PostgreSQL</span>
            <span class="badge">AWS</span>
            <span class="badge">Docker</span>
            <span class="badge">Machine Learning</span>
        </div>

        <footer>
            <p>Profile views: <img src="/api/placeholder/100/20" alt="Profile Views" style="vertical-align: middle;"></p>
        </footer>
    </div>

    <script>
        function openTab(evt, tabName) {
            var i, tabContent, tabLinks;
            tabContent = document.getElementsByClassName("tab-content");
            for (i = 0; i < tabContent.length; i++) {
                tabContent[i].style.display = "none";
            }
            tabLinks = document.getElementsByClassName("tab");
            for (i = 0; i < tabLinks.length; i++) {
                tabLinks[i].className = tabLinks[i].className.replace(" active", "");
            }
            document.getElementById(tabName).style.display = "block";
            evt.currentTarget.className += " active";
        }
    </script>
</body>
</html>
