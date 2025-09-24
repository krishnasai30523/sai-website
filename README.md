# sai-website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Krishna Sai | Portfolio</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        /* Basic Reset */
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Roboto', sans-serif; background-color: #f5f5f5; color: #333; scroll-behavior: smooth; }

        /* Header */
        header {
            background-color: #4c6ef5;
            color: #fff;
            padding: 60px 20px 40px 20px;
            text-align: center;
        }
        header h1 { font-size: 3rem; margin-bottom: 10px; }
        header p { font-size: 1.2rem; }

        /* Navigation */
        nav {
            background-color: #364fc7;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        nav ul {
            display: flex;
            justify-content: center;
            list-style: none;
            flex-wrap: wrap;
        }
        nav ul li {
            margin: 0 15px;
        }
        nav ul li a {
            display: block;
            padding: 15px 0;
            text-decoration: none;
            color: #f8f9fa;
            font-weight: 500;
            transition: 0.3s;
        }
        nav ul li a:hover {
            color: #ffec99;
        }

        /* Sections */
        section {
            padding: 80px 20px;
            max-width: 1000px;
            margin: auto;
        }
        section h2 {
            text-align: center;
            margin-bottom: 50px;
            color: #4c6ef5;
            font-size: 2.5rem;
        }

        /* About Section */
        #about {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
        }
        #about img {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 30px;
            box-shadow: 0px 4px 20px rgba(0,0,0,0.2);
        }
        #about p {
            max-width: 700px;
            font-size: 1.1rem;
            line-height: 1.8;
        }

        /* Projects Section */
        .projects {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 30px;
        }
        .project-card {
            background-color: #fff;
            border-radius: 12px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
            overflow: hidden;
            width: 300px;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .project-card img {
            width: 100%;
            height: 180px;
            object-fit: cover;
        }
        .project-card h3 {
            padding: 15px;
            font-size: 1.5rem;
            color: #364fc7;
        }
        .project-card p {
            padding: 0 15px 15px 15px;
            font-size: 1rem;
            color: #495057;
        }
        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 12px 30px rgba(0,0,0,0.2);
        }

        /* Contact Section */
        #contact form {
            display: flex;
            flex-direction: column;
            gap: 15px;
            max-width: 600px;
            margin: auto;
        }
        #contact input, #contact textarea {
            padding: 12px;
            border-radius: 8px;
            border: 1px solid #ced4da;
            font-size: 1rem;
        }
        #contact button {
            padding: 12px;
            font-size: 1.2rem;
            border-radius: 8px;
            border: none;
            background-color: #4c6ef5;
            color: #fff;
            cursor: pointer;
            transition: 0.3s;
        }
        #contact button:hover {
            background-color: #364fc7;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 30px;
            background-color: #212529;
            color: #fff;
        }

        /* Responsive */
        @media(max-width: 768px) {
            nav ul { flex-direction: column; }
            .projects { flex-direction: column; align-items: center; }
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <h1>Krishna Sai</h1>
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
        <img src="https://cdn.corenexis.com/view/7976355168" alt="Profile Image">
        <p>Hello! I'm Karnati Krishna Sai, a passionate frontend developer. I enjoy creating functional and visually appealing websites using modern technologies like HTML, CSS, JavaScript, and React. I love turning ideas into real applications and continuously learning new skills.</p>
    </section>

    <!-- Projects Section -->
    <section id="projects">
        <h2>My Projects</h2>
        <div class="projects">
            <div class="project-card">
                <img src="https://cdn.corenexis.com/view/7976355168" alt="Portfolio Website">
                <h3>Portfolio Website</h3>
                <p>A responsive personal portfolio website built with HTML, CSS, and JavaScript.</p>
            </div>
            <div class="project-card">
                <img src="https://cdn.corenexis.com/view/7976355168" alt="ToDo App">
                <h3>ToDo App</h3>
                <p>A JavaScript application for managing daily tasks with add/delete functionality.</p>
            </div>
            <div class="project-card">
                <img src="https://via.placeholder.com/300x180" alt="Weather App">
                <h3>Weather App</h3>
                <p>Real-time weather application fetching data from OpenWeatherMap API.</p>
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
        &copy; 2025 Krishna Sai | All Rights Reserved
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

