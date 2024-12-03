<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        :root {
            --primary-color: #0366d6;
            --text-color: #24292e;
            --bg-color: #ffffff;
            --border-color: #e1e4e8;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            background-color: var(--bg-color);
        }

        .container {
            width: 100%;
            max-width: 1000px;
            margin: 0 auto;
        }

        .header {
            text-align: center;
            margin-bottom: 40px;
            border-bottom: 2px solid var(--border-color);
            padding-bottom: 20px;
        }

        .header h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
            color: var(--primary-color);
        }

        .header p {
            font-size: 1.2em;
            color: #586069;
        }

        .section {
            margin-bottom: 40px;
            padding: 20px;
            border: 1px solid var(--border-color);
            border-radius: 6px;
            background-color: #f6f8fa;
        }

        .section h2 {
            color: var(--primary-color);
            border-bottom: 1px solid var(--border-color);
            padding-bottom: 10px;
            margin-bottom: 20px;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .skill-category {
            background-color: white;
            padding: 15px;
            border-radius: 4px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.12);
        }

        .skill-category h3 {
            color: var(--primary-color);
            margin-bottom: 10px;
        }

        .skill-list {
            list-style: none;
            padding: 0;
            margin: 0;
        }

        .skill-list li {
            margin-bottom: 5px;
            display: flex;
            align-items: center;
        }

        .skill-list li::before {
            content: "•";
            color: var(--primary-color);
            margin-right: 8px;
        }

        .projects {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }

        .project-card {
            background-color: white;
            border: 1px solid var(--border-color);
            border-radius: 6px;
            padding: 20px;
            transition: transform 0.2s;
        }

        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }

        .project-card h3 {
            color: var(--primary-color);
            margin-bottom: 10px;
        }

        .stats {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 20px;
        }

        .stat-card {
            flex: 1;
            min-width: 250px;
            background-color: white;
            padding: 20px;
            border-radius: 6px;
            text-align: center;
            box-shadow: 0 1px 3px rgba(0,0,0,0.12);
        }

        .contact {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }

        .contact a {
            color: var(--primary-color);
            text-decoration: none;
            padding: 8px 16px;
            border: 1px solid var(--primary-color);
            border-radius: 4px;
            transition: all 0.2s;
        }

        .contact a:hover {
            background-color: var(--primary-color);
            color: white;
        }

        .quote {
            text-align: center;
            font-style: italic;
            color: #586069;
            margin-top: 40px;
            padding: 20px;
            background-color: #f6f8fa;
            border-radius: 6px;
        }

        @media (max-width: 768px) {
            .skills-grid {
                grid-template-columns: 1fr;
            }

            .projects {
                grid-template-columns: 1fr;
            }

            .stats {
                flex-direction: column;
            }

            .contact {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>Oftanenus Kasa</h1>
            <p>Full Stack Developer | React Specialist | JavaScript & Python Engineer</p>
        </div>

        <div class="section">
            <h2>👨‍💻 Professional Summary</h2>
            <p>Dedicated Full Stack Developer with expertise in React, JavaScript, and Python. Former intern at Xion Computing PLC, currently expanding knowledge in Cloud Computing and actively seeking collaborative opportunities.</p>
        </div>

        <div class="section">
            <h2>🛠️ Technical Stack</h2>
            <div class="skills-grid">
                <div class="skill-category">
                    <h3>Frontend</h3>
                    <ul class="skill-list">
                        <li>React.js</li>
                        <li>JavaScript (ES6+)</li>
                        <li>HTML5/CSS3</li>
                        <li>SCSS</li>
                        <li>Responsive Design</li>
                    </ul>
                </div>
                <div class="skill-category">
                    <h3>Backend</h3>
                    <ul class="skill-list">
                        <li>Node.js</li>
                        <li>Python</li>
                        <li>RESTful APIs</li>
                        <li>Database Management</li>
                    </ul>
                </div>
                <div class="skill-category">
                    <h3>Tools & Technologies</h3>
                    <ul class="skill-list">
                        <li>Git & GitHub</li>
                        <li>Docker</li>
                        <li>Cloud Platforms</li>
                        <li>Development Tools</li>
                    </ul>
                </div>
            </div>
        </div>

        <div class="section">
            <h2>💼 Featured Projects</h2>
            <div class="projects">
                <div class="project-card">
                    <h3>Inventory Management System</h3>
                    <p>Full-stack inventory solution for businesses</p>
                    <p><strong>Technologies:</strong> React, Node.js, MongoDB</p>
                    <p><strong>Features:</strong> Real-time tracking, analytics, reporting</p>
                </div>
                <div class="project-card">
                    <h3>School Management System</h3>
                    <p>Comprehensive educational institution management platform</p>
                    <p><strong>Technologies:</strong> Python, Django, PostgreSQL</p>
                    <p><strong>Features:</strong> Student management, attendance tracking, grade management</p>
                </div>
            </div>
        </div>

        <div class="section">
            <h2>📫 Contact</h2>
            <div class="contact">
                <a href="https://www.linkedin.com/in/oftanenus-kasa-4692aa257/" target="_blank">LinkedIn</a>
                <a href="https://github.com/Oftanenuskasa" target="_blank">GitHub</a>
                <a href="https://web.facebook.com/Oftanenuskasa/" target="_blank">Facebook</a>
            </div>
        </div>

        <div class="quote">
            "Code is like humor. When you have to explain it, it's bad." - Cory House
        </div>
    </div>
</body>
</html>
