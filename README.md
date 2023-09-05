<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your GitHub Profile</title>
    <style>
        /* CSS styles here */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
            transition: background-color 0.3s ease-in-out;
        }
        
        header {
            background-color: #007BFF;
            color: white;
            padding: 20px;
            text-align: center;
            transition: background-color 0.3s ease-in-out;
        }
        
        /* ... (rest of your CSS styles) */
    </style>
</head>
<body>
    <header>
        <h1>Your Name</h1>
        <p>Passionate Full-Stack Web Developer</p>
    </header>

    <main>
        <section class="about">
            <h2>About Me</h2>
            <p>
                I am a full-stack web developer with a strong passion for creating amazing web experiences. I love working with both frontend and backend technologies to bring ideas to life.
            </p>
        </section>

        <section class="skills">
            <h2>Skills</h2>
            <ul>
                <li>HTML, CSS, JavaScript</li>
                <li>React, Node.js, Express</li>
                <li>Database Design (SQL, NoSQL)</li>
                <li>UI/UX Design</li>
            </ul>
        </section>
    </main>

    <footer>
        <p>Connect with me on GitHub: <a href="https://github.com/yourusername" target="_blank">yourusername</a></p>
    </footer>

    <script>
        // JavaScript code here
        document.addEventListener('DOMContentLoaded', () => {
            const body = document.body;
            const header = document.querySelector('header');
            const footer = document.querySelector('footer');
        
            // Apply background color transitions on hover
            header.addEventListener('mouseover', () => {
                body.style.backgroundColor = '#007BFF';
                header.style.backgroundColor = '#0056b3';
                footer.style.color = 'white';
            });
        
            header.addEventListener('mouseout', () => {
                body.style.backgroundColor = '#f5f5f5';
                header.style.backgroundColor = '#007BFF';
                footer.style.color = '#777';
            });
        
            // Apply transform and shadow transitions on section hover
            const sections = document.querySelectorAll('section');
            sections.forEach(section => {
                section.addEventListener('mouseover', () => {
                    section.style.transform = 'scale(1.05)';
                    section.style.boxShadow = '0 0 15px rgba(0, 0, 0, 0.2)';
                });
        
                section.addEventListener('mouseout', () => {
                    section.style.transform = 'scale(1)';
                    section.style.boxShadow = '0 0 10px rgba(0, 0, 0, 0.1)';
                });
            });
        });
    </script>
</body>
</html>
