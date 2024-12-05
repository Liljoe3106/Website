<html lang="en">
<head>
    <style>
        /* Global styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #000;
            color: #fff;
            box-sizing: border-box;
        }

        /* Global heading styles */
        h2, h3 {
            color: #FFD700;
        }

        .stars {
            color: #FFD700;
            font-size: 1.2em;
        }

        header {
            background-color: #000;
            color: #FFD700;
            padding: 20px 0;
            text-align: center;
        }

        .header-container {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .header-container img {
            height: 300px;
            width: auto;
            display: block;
            margin: 0 auto;
        }

        nav {
            background-color: #FFD700;
            padding: 10px 0;
        }

        nav ul {
            list-style: none;
            margin: 0;
            padding: 0;
            text-align: center;
        }

        nav ul li {
            display: inline;
            margin: 0 15px;
        }

        nav ul li a {
            text-decoration: none;
            color: #000;
            font-weight: bold;
            font-size: 1.1em;
            padding: 10px 15px;
            border-radius: 5px;
            background-color: rgba(255, 215, 0, 0.2);
            transition: background-color 0.3s ease;
        }

        nav ul li a:hover {
            background-color: rgba(255, 215, 0, 0.5);
        }

        /* Section styles */
        section {
            padding: 40px 20px;
        }

        #about-us p strong {
            color: #FFD700;
        }

        .slider, .gutter-slider, .roof-slider {
            width: 100%;
            max-width: 1000px;
            margin: 0 auto;
            overflow: hidden;
            position: relative;
            background-color: #000;
            border: none;
        }

        .slides {
            display: flex;
            transition: transform 0.6s ease-in-out;
        }

        .slides img {
            width: 100%;
            flex-shrink: 0;
        }

        footer {
            background-color: #000;
            color: #FFD700;
            padding: 20px 0;
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
        }

        footer a {
            color: #FFD700;
            text-decoration: underline;
        }

        footer a:hover {
            text-decoration: underline;
        }

        /* Responsive styles */
        @media (max-width: 800px) {
            section, footer {
                padding: 15px;
            }

            section h2 {
                font-size: 1.5em;
            }
        }

        @media (max-width: 600px) {
            nav ul li {
                display: block;
                margin: 5px 0;
            }
        }
    </style>
</head>

<body>
    <header>
        <div class="header-container">
            <img src="DP MEDIA/logo.png" alt="Dimension Powerwash Logo" loading="lazy">
            <h1>Dimension Powerwash</h1>
            <p>Exterior Cleaning Specialists - Sheffield</p>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="#driveway-patio">Drive & Patio Cleaning</a></li>
            <li><a href="#gutter-cleaning">Gutter Cleaning</a></li>
            <li><a href="#roof-cleaning">Roof Cleaning</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <section id="about-us">
        <h2>About Us</h2>
        <p>Welcome to <strong>Dimension Powerwash</strong>! We are dedicated to providing high-quality exterior cleaning services, specializing in <strong>pressure washing</strong>, <strong>drive cleaning</strong>, <strong>patio cleaning</strong>, <strong>roof cleaning</strong>, and <strong>gutter clearing/cleaning</strong>. Based in <strong>Sheffield</strong>, we proudly serve both residential and commercial clients across the city and surrounding areas.</p>
    </section>

    <section id="driveway-patio">
        <h2>Drive & Patio Cleaning</h2>
        <ul>
            <li>Remove ingrained dirt, moss, algae, and black spots.</li>
            <li><strong style="color: #FFD700;">Professional pathway cleaning</strong> for all surfaces.</li>
        </ul>
        <div class="slider">
            <div class="slides">
                <img src="DP MEDIA/Block paving before after.png" alt="Block paving before after" loading="lazy">
                <img src="DP MEDIA/Patio before after.png" alt="Patio before after" loading="lazy">
                <img src="DP MEDIA/Path before after.png" alt="Path before after" loading="lazy">
            </div>
        </div>
    </section>

    <section id="gutter-cleaning">
        <h2>Gutter Cleaning</h2>
        <ul>
            <li>Prevent expensive repairs from blocked gutters.</li>
            <li>Clear rainwater pathways effectively.</li>
            <li>Restore gutters with a <strong style="color: #FFD700;">complete washdown</strong>.</li>
        </ul>
        <div class="gutter-slider">
            <div class="slides">
                <img src="DP MEDIA/Free Gutter CHECK.png" alt="Free Gutter Check" loading="lazy">
                <img src="DP MEDIA/Gutter Clearing.png" alt="Gutter Clearing" loading="lazy">
                <img src="DP MEDIA/Gutter Cleaning Before After.png" alt="Gutter Cleaning Before After" loading="lazy">
            </div>
        </div>
    </section>

    <section id="roof-cleaning">
        <h2>Roof Cleaning</h2>
        <ul>
            <li>Remove moss with <strong style="color: #FFD700;">anti-fungal treatments</strong>.</li>
            <li>Prevent future moss growth and gutter blockages.</li>
            <li>Use less invasive methods than pressure washing.</li>
        </ul>
        <div class="roof-slider">
            <div class="slides">
                <img src="DP MEDIA/Roof Treatment.png" alt="Roof Treatment" loading="lazy">
            </div>
        </div>
    </section>

    <footer id="contact">
        <h3>Contact Us</h3>
        <a href="https://calendly.com/dimensionpowerwash/free-quote" target="_blank">Get your free gutter check or book a quote!</a>
        <p>Call us at:</p>
        <p>0114 457 3009 | 07494503865</p>
        <p>Follow us on <a href="https://facebook.com/dimensionpowerwash" target="_blank">Facebook</a>.</p>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function () {
            const setUpSlider = (selector) => {
                const slides = document.querySelectorAll(`${selector} .slides img`);
                let index = 0;

                setInterval(() => {
                    slides.forEach(slide => slide.classList.add('hidden'));
                    slides[index].classList.remove('hidden');
                    index = (index + 1) % slides.length;
                }, 3000);
            };

            setUpSlider('.slider');
            setUpSlider('.gutter-slider');
            setUpSlider('.roof-slider');
        });
    </script>
</body>
</html>
