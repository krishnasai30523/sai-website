# sai-website
portfolio website built with HTML, CSS, and JavaScript.</p>
            </div>
            <div class="project-card">
                <img src="https://via.placeholder.com/300x180" alt="ToDo App">
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

    <section id="contact">
        <h2>Contact Me</h2>
        <form onsubmit="sendMessage(event)">
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea placeholder="Your Message" rows="5" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <footer>
        &copy; 2025 Krishna Sai | All Rights Reserved
    </footer>

    <script>
        function sendMessage(event) {
            event.preventDefault();
            alert("Thank you! Your message has been sent.");
        }
    </script>

</body>
</html>

