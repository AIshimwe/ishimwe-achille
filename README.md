<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Awesome Website</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* Header Styles */
        header {
            background-color: #1f2937;
            padding: 1rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 1rem;
        }

        .header-logo img {
            max-height: 40px;
            width: auto;
            transition: transform 0.3s ease;
        }

        .header-logo img:hover {
            transform: scale(1.1);
        }

        .header-links {
            display: flex;
            gap: 2rem;
            flex-wrap: wrap;
        }

        .header-links a {
            color: #9ca3af;
            text-decoration: none;
            padding: 0.5rem;
            transition: color 0.3s ease, transform 0.3s ease;
        }

        .header-links a:hover {
            color: white;
            transform: translateY(-2px);
        }

        /* Hero Section */
        .hero {
            background-color: #1f2937;
            padding: 4rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 2rem;
            flex-wrap: wrap;
        }

        .hero-content {
            flex: 1;
            min-width: 300px;
        }

        .hero h1 {
            color: white;
            font-size: clamp(2rem, 5vw, 3rem);
            margin-bottom: 1rem;
        }

        .hero p {
            color: #9ca3af;
            margin-bottom: 1.5rem;
            font-size: clamp(1rem, 2vw, 1.2rem);
        }

        .hero-image {
            flex: 1;
            min-width: 300px;
            height: 300px;
            background-color: #6b7280;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            background-size: cover;
            background-position: center top;
            background-repeat: no-repeat;
        }

        /* Info Section */
        .info-section {
            padding: 4rem 5%;
            text-align: center;
        }

        .info-section h2 {
            font-size: clamp(1.5rem, 4vw, 2rem);
            margin-bottom: 2rem;
            color: #1f2937;
        }

        .info-cards {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin-top: 2rem;
            flex-wrap: wrap;
        }

        .info-card {
            flex: 1;
            min-width: 250px;
            max-width: 300px;
            transition: transform 0.3s ease;
            cursor: pointer;
        }

        .info-card:hover {
            transform: translateY(-10px);
        }

        .card-image {
            border: 3px solid #3b82f6;
            border-radius: 8px;
            height: 150px;
            background-size: cover;
            background-position: center;
            margin-bottom: 1rem;
            transition: border-color 0.3s ease;
        }

        .info-card:hover .card-image {
            border-color: #2563eb;
        }

        .info-card p {
            color: #6b7280;
            font-size: 0.9rem;
        }

        .info-card a {
            text-decoration: none;
            color: inherit;
        }

        /* Quote Section */
        .quote-section {
            background-color: #e5e7eb;
            padding: 4rem 5%;
            transition: background-color 0.3s ease;
        }

        .quote-section:hover {
            background-color: #d1d5db;
        }

        .quote {
            font-style: italic;
            font-size: clamp(1.2rem, 3vw, 1.5rem);
            color: #1f2937;
            margin-bottom: 1rem;
        }

        .quote-author {
            text-align: right;
            font-weight: bold;
            font-size: clamp(1rem, 2vw, 1.2rem);
        }

        /* CTA Section */
        .cta-section {
            padding: 4rem 5%;
        }

        .cta-container {
            background-color: #3b82f6;
            color: white;
            padding: 3rem;
            border-radius: 8px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 2rem;
            flex-wrap: wrap;
            transition: transform 0.3s ease;
        }

        .cta-container:hover {
            transform: scale(1.02);
        }

        /* Button Styles */
        .btn {
            background-color: #3b82f6;
            color: white;
            padding: 0.5rem 2rem;
            border-radius: 6px;
            text-decoration: none;
            display: inline-block;
            white-space: nowrap;
            transition: all 0.3s ease;
        }

        .btn:hover {
            background-color: #2563eb;
            transform: translateY(-2px);
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        .btn-outline {
            border: 2px solid white;
        }

        .btn-outline:hover {
            background-color: white;
            color: #3b82f6;
        }

        /* Footer */
        footer {
            background-color: #1f2937;
            color: white;
            text-align: center;
            padding: 2rem;
        }

        /* Media Queries */
        @media (max-width: 768px) {
            header {
                justify-content: center;
                text-align: center;
            }

            .hero {
                text-align: center;
            }

            .hero-content, .hero-image {
                flex: 100%;
            }

            .cta-container {
                text-align: center;
                justify-content: center;
            }

            .cta-container > div {
                flex: 100%;
            }
        }

        @media (max-width: 480px) {
            .header-links {
                gap: 1rem;
                justify-content: center;
                width: 100%;
            }

            .hero {
                padding: 2rem 5%;
            }

            .info-card {
                min-width: 100%;
            }

            .cta-container {
                padding: 2rem 1rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="header-logo">
            <img src="curry-brand-3m.png" alt="Header Logo" />
        </div>
        <nav class="header-links">
            <a href="#Home" target="_blank" rel="noopener noreferrer">25782</a>
            <a href="#Pictures" target="_blank" rel="noopener noreferrer">Ishimwe</a>
            <a href="#Comments" target="_blank" rel="noopener noreferrer">Achille</a>
        </nav>
    </header>

    <section id="Home" class="hero">
        <div class="hero-content">
            <h1>Welcome to the Court</h1>
            <p>Stay updated with the latest games, news, and stats. Dive into the world of basketball.</p>
            <a href="https://www.nba.com/" class="btn" target="_blank" rel="noopener noreferrer">Join the Game</a>
        </div>
        <div class="hero-image" style="background-image: url('curry.jpg')">
        </div>
    </section>

    <section id="Pictures" class="info-section">
        <h2>Explore the Game</h2>
        <div class="info-cards">
            <div class="info-card">
                <a href="https://www.nba.com/games" target="_blank" rel="noopener noreferrer">
                    <div class="card-image" style="background-image: url('NBAMobile.png')"></div>
                    <p>Latest Game Highlights</p>
                </a>
            </div>
            <div class="info-card">
                <a href="https://www.nba.com/stats/players" target="_blank" rel="noopener noreferrer">
                    <div class="card-image" style="background-image: url('ball (7).jpg')"></div>
                    <p>Top Players and Stats</p>
                </a>
            </div>
            <div class="info-card">
                <a href="https://www.nba.com/standings" target="_blank" rel="noopener noreferrer">
                    <div class="card-image" style="background-image: url('ball (1).jfif')"></div>
                    <p>Team Rankings</p>
                </a>
            </div>
            <div class="info-card">
                <a href="https://www.nba.com/schedule" target="_blank" rel="noopener noreferrer">
                    <div class="card-image" style="background-image: url('ball (5).jpg')"></div>
                    <p>Upcoming Tournaments</p>
                </a>
            </div>
        </div>
    </section>

    <section id="Comments" class="quote-section">
        <div class="quote">
            Be the best version of yourself in anything that you do. You don't have to live anybody else's story.
        </div>
        <div class="quote-author">-Stephen curry, Chef curry</div>
    </section>

    <section class="cta-section">
        <div class="cta-container">
            <div>
                <h3>Call to action! It's game time!</h3>
                <p>Sign up for on our website to keep up with the game!</p>
            </div>
            <a href="https://www.nba.com/" class="btn btn-outline" target="_blank" rel="noopener noreferrer">Sign up</a>
        </div>
    </section>

    <footer>
        Copyright © The Project 2025
    </footer>
</body>
</html>
