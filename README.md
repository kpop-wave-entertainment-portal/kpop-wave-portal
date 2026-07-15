<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <style>
        /* Modern CSS Reset & Variables */
        :root {
            --bg-color: #0f172a;
            --text-color: #f8fafc;
            --accent-color: #38bdf8;
            --secondary-text: #94a3b8;
            --card-bg: #1e293b;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.6;
            padding: 2rem 1rem;
        }

        /* Container Layout */
        .container {
            max-width: 800px;
            margin: 0 auto;
        }

        /* Header Section */
        header {
            margin-bottom: 3rem;
            text-align: center;
        }

        header h1 {
            font-size: 2.5rem;
            font-weight: 800;
            margin-bottom: 0.5rem;
            background: linear-gradient(to right, #38bdf8, #818cf8);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        header p {
            font-size: 1.1rem;
            color: var(--secondary-text);
        }

        /* About Section */
        .about {
            margin-bottom: 3rem;
        }

        .about h2 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            border-bottom: 1px solid var(--card-bg);
            padding-bottom: 0.5rem;
        }

        /* Projects Section */
        .projects-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 1.5rem;
            margin-top: 1rem;
        }

        @media (min-width: 600px) {
            .projects-grid {
                grid-template-columns: 1fr 1fr;
            }
        }

        .project-card {
            background-color: var(--card-bg);
            padding: 1.5rem;
            border-radius: 8px;
            transition: transform 0.2s ease, box-shadow 0.2s ease;
            text-decoration: none;
            color: inherit;
            display: block;
            border: 1px solid transparent;
        }

        .project-card:hover {
            transform: translateY(-4px);
            border-color: var(--accent-color);
            box-shadow: 0 4px 20px rgba(56, 189, 248, 0.1);
        }

        .project-card h3 {
            font-size: 1.2rem;
            margin-bottom: 0.5rem;
            color: var(--accent-color);
        }

        .project-card p {
            font-size: 0.9rem;
            color: var(--secondary-text);
        }

        /* Contact/Social Links */
        .links {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin-top: 3rem;
            flex-wrap: wrap;
        }

        .links a {
            color: var(--text-color);
            text-decoration: none;
            font-weight: 500;
            padding: 0.5rem 1rem;
            border: 1px solid var(--secondary-text);
            border-radius: 20px;
            transition: all 0.2s ease;
        }

        .links a:hover {
            background-color: var(--accent-color);
            color: var(--bg-color);
            border-color: var(--accent-color);
        }

        footer {
            margin-top: 5rem;
            text-align: center;
            font-size: 0.8rem;
            color: var(--secondary-text);
        }
    </style>
</head>
<body>

    <div class="container">
        <!-- Header -->
        <header>
            <h1>Hi, I'm [Your Name] 👋</h1>
            <p>[Your Title / Bio line, e.g., "Software Engineer & Designer"]</p>
        </header>

        <!-- About -->
        <section class="about">
            <h2>About Me</h2>
            <p>Welcome to my corner of the web! I enjoy building things that live on the internet. My work focuses on creating fast, accessible, and clean user experiences.</p>
        </section>

        <!-- Projects -->
        <section class="projects">
            <h2>Featured Projects</h2>
            <div class="projects-grid">
                
                <!-- Project 1 -->
                <a href="https://github.com/yourusername/project1" class="project-card" target="_blank">
                    <h3>Project One</h3>
                    <p>A brief, engaging description of what this project does, the tech stack used, and the problem it solves.</p>
                </a>

                <!-- Project 2 -->
                <a href="https://github.com/yourusername/project2" class="project-card" target="_blank">
                    <h3>Project Two</h3>
                    <p>Another awesome project goes here. Keep descriptions short, snappy, and focused on outcomes.</p>
                </a>

            </div>
        </section>

        <!-- Links/Socials -->
        <div class="links">
            <a href="https://github.com/yourusername" target="_blank">GitHub</a>
            <a href="https://linkedin.com/in/yourusername" target="_blank">LinkedIn</a>
            <a href="mailto:your.email@example.com">Email</a>
        </div>

        <!-- Footer -->
        <footer>
            <p>&copy; 2026 [Your Name]. Built with plain HTML & CSS.</p>
        </footer>
    </div>

</body>
</html>
