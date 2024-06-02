<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Codex Academy</title>
    <link rel="stylesheet" href="styles.css">
    <script defer src="scripts.js"></script>
</head>
<body>
    <header>
        <h1>Codex Academy</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#courses">Courses</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    <section id="home" class="hero">
        <h2>Welcome to Codex Academy</h2>
        <p>Learn Computer Basics and Programming Languages</p>
        <a href="#contact" class="btn">Enroll Now</a>
    </section>
    <section id="about" class="content">
        <h2>About Us</h2>
        <p>Codex Academy offers comprehensive courses on computer basics and programming languages.</p>
    </section>
    <section id="courses" class="content">
        <h2>Courses</h2>
        <h3>Computer Basics</h3>
        <p>Learn MS Word, Excel, and other essential tools.</p>
        <h3>Programming Languages</h3>
        <p>Courses in C, Java, and more.</p>
    </section>
    <section id="contact" class="content">
        <h2>Contact Us</h2>
        <form id="contactForm">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required><br><br>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required><br><br>
            <label for="message">Message:</label><br>
            <textarea id="message" name="message" rows="4" cols="50" required></textarea><br><br>
            <input type="submit" value="Submit">
        </form>
        <p>Email: info@codexacademy.com</p>
        <p>Phone: 123-456-7890</p>
    </section>
    <footer>
        <p>&copy; 2024 Codex Academy. All rights reserved.</p>
    </footer>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

header {
    background: #333;
    color: #fff;
    padding: 10px 0;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
}

.hero {
    background: #e2e2e2;
    padding: 50px 20px;
    text-align: center;
}

.hero h2 {
    margin: 0;
    font-size: 2.5em;
}

.hero p {
    font-size: 1.2em;
}

.hero .btn {
    display: inline-block;
    margin-top: 20px;
    padding: 10px 20px;
    background: #333;
    color: #fff;
    text-decoration: none;
}

.content {
    padding: 20px;
    background: #fff;
    margin: 20px;
    border-radius: 5px;
}

footer {
    background: #333;
    color: #fff;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}

form {
    display: flex;
    flex-direction: column;
}

form label {
    margin-top: 10px;
}

form input, form textarea {
    padding: 10px;
    margin-top: 5px;
    border: 1px solid #ccc;
    border-radius: 5px;
}
document.getElementById('contactForm').addEventListener('submit', function(event) {
    event.preventDefault();
    alert('Thank you for your message. We will get back to you soon.');
    this.reset();
});

