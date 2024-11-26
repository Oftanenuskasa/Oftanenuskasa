<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        @keyframes gradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0px); }
        }

        @keyframes glow {
            0% { box-shadow: 0 0 5px #4CAF50; }
            50% { box-shadow: 0 0 20px #4CAF50; }
            100% { box-shadow: 0 0 5px #4CAF50; }
        }

        .profile-container {
            background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
            background-size: 400% 400%;
            animation: gradient 15s ease infinite;
            padding: 2rem;
            border-radius: 15px;
            color: white;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        .profile-header {
            text-align: center;
            margin-bottom: 2rem;
        }

        .profile-image {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            border: 5px solid white;
            animation: float 6s ease-in-out infinite;
            margin: 20px auto;
            display: block;
            box-shadow: 0 0 15px rgba(0,0,0,0.3);
        }

        .skill-container {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            justify-content: center;
            margin: 20px 0;
        }

        .skill-badge {
            padding: 8px 15px;
            border-radius: 20px;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: all 0.3s ease;
        }

        .skill-badge:hover {
            transform: scale(1.1);
            background: rgba(255, 255, 255, 0.2);
        }

        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }

        .stats-card {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 10px;
            backdrop-filter: blur(10px);
            animation: glow 3s infinite;
        }

        .project-card {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 10px;
            margin: 10px 0;
            transition: transform 0.3s ease;
        }

        .project-card:hover {
            transform: translateX(10px);
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin: 20px 0;
        }

        .social-icon {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: white;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: transform 0.3s ease;
        }

        .social-icon:hover {
            transform: scale(1.2);
        }

        .typing-text {
            border-right: 2px solid white;
            white-space: nowrap;
            overflow: hidden;
            animation: typing 3.5s steps(40, end), blink-caret 0.75s step-end infinite;
        }

        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }

        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: white }
        }
    </style>
</head>
<body>
    <div class="profile-container">
        <div class="profile-header">
            <img src="https://z-p3-scontent.fadd2-1.fna.fbcdn.net/v/t39.30808-6/461327921_1924092578003254_2405530486380552276_n.jpg" alt="Oftanenus Kasa" class="profile-image">
            <h1 class="typing-text">Hi, I'm Oftanenus Kasa! 👋</h1>
            <p>Full Stack Developer | React Enthusiast | JavaScript & Python Lover</p>
        </div>

        <div class="skill-container">
            <div class="skill-badge">JavaScript</div>
            <div class="skill-badge">Python</div>
            <div class="skill-badge">React</div>
            <div class="skill-badge">Node.js</div>
            <div class="skill-badge">Docker</div>
            <div class="skill-badge">Git</div>
        </div>

        <div class="stats-container">
            <div class="stats-card">
                <h3>About Me</h3>
                <p>🔭 Former Intern at Xion Computing PLC</p>
                <p>🌱 Currently learning Cloud Computing</p>
                <p>👨‍💻 Open to collaboration</p>
            </div>
            <div class="stats-card">
                <h3>GitHub Stats</h3>
                <!-- Add your GitHub stats here -->
            </div>
        </div>

        <h2>Featured Projects</h2>
        <div class="project-card">
            <h3>Inventory Management System</h3>
            <p>A comprehensive system for business inventory management</p>
        </div>
        <div class="project-card">
            <h3>School Management System</h3>
            <p>Efficient platform for academic institution management</p>
        </div>

        <div class="social-links">
            <a href="https://www.linkedin.com/in/oftanenus-kasa-4692aa257/" class="social-icon">
                <img src="linkedin-icon.png" alt="LinkedIn">
            </a>
            <a href="https://github.com/Oftanenuskasa" class="social-icon">
                <img src="github-icon.png" alt="GitHub">
            </a>
            <a href="https://web.facebook.com/Oftanenuskasa/" class="social-icon">
                <img src="facebook-icon.png" alt="Facebook">
            </a>
        </div>
    </div>
</body>
</html>
