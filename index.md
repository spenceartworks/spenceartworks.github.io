><!-- One-Page Portfolio for Spence Artworks -->
---
layout: none  # No default Jekyll layout for full customization
---

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Spence Artworks</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Montserrat', sans-serif;
            background: #111;
            color: #fff;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 10px;
            padding: 20px;
        }
        .gallery img {
            width: 100%;
            height: auto;
            border-radius: 5px;
            transition: transform 0.3s ease;
        }
        .gallery img:hover {
            transform: scale(1.05);
        }
        .about {
            padding: 50px 20px;
            background: #222;
        }
        .socials {
            margin-top: 20px;
        }
        .socials a {
            color: #fff;
            text-decoration: none;
            margin: 0 10px;
            font-size: 1.5rem;
        }
    </style>
</head>
<body>
    <h1>Spence Artworks</h1>
    <p>Modern Pin-up Illustrations by Mr. Spence</p>

    <section class="gallery">
        {% for i in (3128..3075) reversed %}
            {% if i != 3100 and i != 3102 and i != 3103 and i != 3105 and i != 3106 %}
                <img src="IMG_{{ i }}.jpeg" alt="Artwork {{ i }}">
            {% endif %}
        {% endfor %}
    </section>

    <section class="about">
        <h2>About Me</h2>
        <p>Scottish pin-up artist bringing classic beauty into the modern era. My work is inspired by vintage glamour, bold confidence, and watercolor mastery.</p>
        <p>Follow my journey and discover more of my work on social media:</p>
        <div class="socials">
            <a href="https://www.tiktok.com/@spencepinups">TikTok</a>
            <a href="https://www.facebook.com/SpencePinups/photos/">Facebook</a>
        </div>
    </section>
</body>
</html>

