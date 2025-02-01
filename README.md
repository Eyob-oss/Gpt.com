<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Assistant</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
            scroll-behavior: smooth;
        }
        body {
            background-color: #0D1117;
            color: #fff;
            text-align: center;
        }
        /* Navigation Bar */
        nav {
            background: #161B22;
            padding: 15px 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            gap: 30px;
        }
        nav ul li {
            display: inline;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
            font-size: 18px;
            transition: 0.3s;
        }
        nav ul li a:hover {
            color: cyan;
        }

        /* Sections */
        section {
            padding: 100px 20px;
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
        }
        .home {
            background: url('https://source.unsplash.com/1600x900/?ai,robot') no-repeat center center/cover;
            position: relative;
            color: white;
        }
        .home h1 {
            font-size: 3rem;
            animation: fadeIn 1.5s forwards;
        }
        .ai-robot {
            width: 150px;
            height: 150px;
            background: url('https://i.imgur.com/9RVOaRF.png') no-repeat center center/cover;
            animation: float 3s infinite ease-in-out;
        }

        /* About Section */
        .about, .features, .contact {
            background: #161B22;
        }

        .features .card-container {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }
        .card {
            background: #1F2935;
            padding: 20px;
            border-radius: 10px;
            width: 250px;
            text-align: center;
            box-shadow: 0 0 10px rgba(255, 255, 255, 0.1);
            opacity: 0;
            transform: scale(0.8);
            animation: fadeInScale 1.5s forwards;
        }

        /* Animations */
        @keyframes fadeIn {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        @keyframes fadeInScale {
            to {
                opacity: 1;
                transform: scale(1);
            }
        }
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        /* Footer */
        footer {
            background: #121212;
            padding: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About Us</a></li>
            <li><a href="#features">Features</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Home Section -->
    <section id="home" class="home">
        <h1>Welcome to AI Assistant</h1>
        <div class="ai-robot"></div>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <h2>About AI Assistant</h2>
        <p>AI Assistant is a smart chatbot designed to help you with conversations, coding, and more.</p>
    </section>

    <!-- Features Section -->
    <section id="features" class="features">
        <h2>Features</h2>
        <div class="card-container">
            <div class="card" style="animation-delay: 0.5s;">
                <h3>Smart Conversations</h3>
                <p>Talk with AI naturally and get instant responses.</p>
            </div>
            <div class="card" style="animation-delay: 1s;">
                <h3>Code Helper</h3>
                <p>Write and debug code effortlessly.</p>
            </div>
            <div class="card" style="animation-delay: 1.5s;">
                <h3>Creative Writing</h3>
                <p>Generate blogs, scripts, and creative text.</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <h2>Contact Us</h2>
        <p>Email: support@aiassistant.com</p>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 AI Assistant. All rights reserved.</p>
    </footer>
</body>
</html>
