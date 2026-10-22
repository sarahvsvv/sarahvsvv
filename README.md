
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sarah | GitHub Profile</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background: #ffe6f2;
            color: #4a2438;
            min-height: 100vh;
            padding: 40px 20px;
        }

        .container {
            max-width: 900px;
            margin: auto;
        }

        .header {
            text-align: center;
            padding: 40px 20px;
            background: linear-gradient(135deg, #ffb6d9, #f7c8ff);
            border-radius: 25px;
            box-shadow: 0 8px 25px #d98bb855;
        }

        .profile-image {
            width: 130px;
            height: 130px;
            border-radius: 50%;
            border: 5px solid white;
            object-fit: cover;
            margin-bottom: 20px;
        }

        .header h1 {
            font-size: 36px;
            margin-bottom: 12px;
        }

        .header p {
            font-size: 16px;
            line-height: 1.7;
        }

        .section {
            background: #fff7fb;
            padding: 25px;
            margin-top: 25px;
            border-radius: 20px;
            box-shadow: 0 5px 18px #d98bb822;
        }

        .section h2 {
            color: #d63384;
            margin-bottom: 15px;
        }

        .section p {
            line-height: 1.8;
        }

        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
        }

        .skill {
            background: #ffd0e6;
            color: #8b2459;
            padding: 10px 16px;
            border-radius: 30px;
            font-size: 14px;
            font-weight: bold;
        }

        .projects {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 15px;
        }

        .project-card {
            background: #ffe6f2;
            border: 1px solid #ffc1df;
            padding: 20px;
            border-radius: 15px;
            transition: 0.3s;
        }

        .project-card:hover {
            transform: translateY(-5px);
            background: #ffd6e9;
        }

        .project-card h3 {
            color: #c02675;
            margin-bottom: 10px;
        }

        .project-card p {
            font-size: 14px;
        }

        .social-links {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            margin-top: 15px;
        }

        .social-links a {
            text-decoration: none;
            background: #e7549b;
            color: white;
            padding: 12px 18px;
            border-radius: 25px;
            transition: 0.3s;
        }

        .social-links a:hover {
            background: #bd347b;
            transform: scale(1.05);
        }

        .footer {
            text-align: center;
            padding: 30px 10px;
            font-size: 13px;
            color: #995778;
        }

        @media (max-width: 600px) {
            .header h1 {
                font-size: 28px;
            }

            body {
                padding: 20px 12px;
            }
        }
    </style>
</head>

<body>
    <div class="container">

        <div class="header">
            <!-- Ganti URL foto dengan foto kamu -->
            <img
                src="sarah-casual.png"
                alt="Sarah's profile photo"
                class="profile-image"
            >

            <h1>Hi, I'm Sarah! ♡</h1>

            <p>
                Multimedia Graduate | Sociology Education Student<br>
                Interested in Digital Marketing, Design, and Web Development.
            </p>
        </div>

        <div class="section">
            <h2>💗 About Me</h2>

            <p>
                I'm a vocational high school graduate majoring in Multimedia
                and currently studying Sociology Education at Jakarta State
                University. I have experience in graphic design, video editing,
                content creation, and digital marketing. I enjoy learning new
                skills and creating digital projects.
            </p>
        </div>

        <div class="section">
            <h2>🎀 Skills</h2>

            <div class="skills">
                <div class="skill">HTML</div>
                <div class="skill">CSS</div>
                <div class="skill">JavaScript</div>
                <div class="skill">Graphic Design</div>
                <div class="skill">Video Editing</div>
                <div class="skill">Digital Marketing</div>
                <div class="skill">Content Creation</div>
            </div>
        </div>

        <div class="section">
            <h2>🌸 Featured Projects</h2>

            <div class="projects">

                <div class="project-card">
                    <h3>Interactive Lanyard</h3>
                    <p>
                        An interactive 3D-inspired pink lanyard animation
                        built using HTML, CSS, and JavaScript.
                    </p>
                </div>

                <div class="project-card">
                    <h3>Graphic Design</h3>
                    <p>
                        Creative designs including logos, product packaging,
                        and promotional materials.
                    </p>
                </div>

                <div class="project-card">
                    <h3>Digital Marketing</h3>
                    <p>
                        Product photography, promotional videos, and
                        social media content for businesses.
                    </p>
                </div>

            </div>
        </div>

        <div class="section">
            <h2>🌐 Connect With Me</h2>

            <p>Let's connect and create something amazing!</p>

            <div class="social-links">
                <a href="https://github.com/" target="_blank">
                    GitHub
                </a>

                <a href="https://www.linkedin.com/" target="_blank">
                    LinkedIn
                </a>

                <a href="https://www.instagram.com/" target="_blank">
                    Instagram
                </a>
            </div>
        </div>

        <div class="footer">
            <p>Made with ♡ by Sarah | 2026</p>
        </div>

    </div>
</body>
</html>