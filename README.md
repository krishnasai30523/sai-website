# sai-website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <style>
        /* Basic Reset */
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: Arial, sans-serif; line-height: 1.6; background-color: #dfcece; color: #333; }

        /* Header */
        header {
            background-color: #c6dbc6;
            color: rgb(105, 93, 93);
            padding: 20px 0;
            text-align: center;
        }

        header h1 { margin-bottom: 10px; }
        header p { font-size: 18px; }

        /* Navigation */
        nav { background: #786c6c; }
        nav ul {
            display: flex;
            list-style: none;
            justify-content: center;
        }
        nav ul li { margin: 0 15px; }
        nav ul li a {
            color: rgb(196, 160, 160);
            text-decoration: none;
            padding: 15px 0;
            display: block;
        }
        nav ul li a:hover { color: #947e5d; }

        /* Sections */
        section { padding: 50px 20px; max-width: 1000px; margin: auto; }
        section h2 { text-align: center; margin-bottom: 30px; color: #75f279; }

        /* About Section */
        #about p { text-align: center; max-width: 800px; margin: auto; }

        /* Projects Section */
        .projects { display: flex; flex-wrap: wrap; justify-content: center; gap: 20px; }
        .project-card {
            background: rgb(101, 77, 77);
            padding: 20px;
            width: 250px;
            border-radius: 10px;
            box-shadow: 0 2px 8px rgba(172, 109, 109, 0.2);
            text-align: center;
            transition: transform 0.3s;
        }
        .project-card:hover { transform: translateY(-5px); }

        /* Contact Section */
        form { max-width: 600px; margin: auto; display: flex; flex-direction: column; }
        input, textarea {
            padding: 10px;
            margin: 10px 0;
            border-radius: 5px;
            border: 1px solid #9a5353;
            font-size: 16px;
        }
        button {
            padding: 10px;
            background: #e7b5b5;
            color: rgb(169, 104, 104);
            border: none;
            cursor: pointer;
            font-size: 18px;
            border-radius: 5px;
            transition: background 0.3s;
        }
        button:hover { background: #868f87; }

        /* Footer */
        footer { text-align: center; padding: 20px; background: #333; color: rgb(255, 255, 255); }

        /* Responsive */
        @media(max-width:768px) {
            .projects { flex-direction: column; align-items: center; }
            nav ul { flex-direction: column; }
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <h1>krishna sai</h1>
        <p>Frontend Developer | Web Designer | Programmer</p>
    </header>

    <!-- Navigation -->
    <nav>
        <ul>
            <li><a href="#about">About</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- About Section -->
    <section id="about">
        <h2>About Me</h2>
        <p>Hello! I'm karnati krishna sai, a passionate frontend developer. I love creating beautiful and functional websites, learning new technologies, and building projects that help people. My skills include HTML, CSS, JavaScript, and React. I enjoy turning ideas into real web applications and i now graduating in vbit 3rd year THANK YOU...</p>
    </section>

    <!-- Projects Section -->
    <section id="projects">
        <h2>My Projects</h2>
        <div class="projects">
            <div class="project-card">
                <h3>Portfolio Website</h3>
                <p>A responsive personal portfolio built with HTML, CSS, and JS.</p>
            </div>
            <div class="project-card">
                <h3>ToDo App</h3>
                <p>A JavaScript app to manage daily tasks with add/delete functionality.</p>
            </div>
            <div class="project-card">
                <h3>Weather App</h3>
                <p>Real-time weather updates fetched from OpenWeatherMap API.</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Contact Me</h2>
        <form onsubmit="sendMessage(event)">
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea placeholder="Your Message" rows="5" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        &copy; 2025 krishna sai | All Rights Reserved
    </footer>

    <!-- JavaScript -->
    <script>
        function sendMessage(event) {
            event.preventDefault();
            alert("Thank you! Your message has been sent.");
        }
    </script>

</body>
</html>
