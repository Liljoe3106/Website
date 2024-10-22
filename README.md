<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Professional exterior cleaning services in Sheffield. Specialists in pressure washing, drive cleaning, patio cleaning, and gutter cleaning. Serving Sheffield, Rotherham, and Worksop.">
    <meta name="keywords" content="pressure washing, drive cleaning, patio cleaning, gutter cleaning, Sheffield, Rotherham, Worksop">
    <title>Dimension Powerwash | Professional Exterior Cleaning Services Sheffield</title>

    <!-- Open Graph tags for social media sharing -->
    <meta property="og:title" content="Dimension Powerwash - Exterior Cleaning Specialists Sheffield">
    <meta property="og:description" content="Professional pressure washing and gutter cleaning services in Sheffield and surrounding areas.">
    <meta property="og:image" content="https://dimensionpowerwash.com/DP-MEDIA/logo.png">
    <meta property="og:url" content="https://dimensionpowerwash.com">
    
    <style>
        /* Global styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #000;
            color: #fff;
            box-sizing: border-box;
            line-height: 1.6;
        }

        /* Global heading styles */
        h2, h3 {
            color: #FFD700;
        }

        /* Focus styles for accessibility */
        a:focus, button:focus {
            outline: 3px solid #FFD700;
            outline-offset: 2px;
        }

        .stars {
            color: #FFD700;
            font-size: 1.2em;
        }

        header {
            background: linear-gradient(90deg, #000, #333);
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
            display: inline-block;
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

        nav ul li a:hover,
        nav ul li a:focus {
            background-color: rgba(255, 215, 0, 0.5);
        }

        .section {
            padding: 50px 20px;
            text-align: center;
        }

        .slider-container {
            position: relative;
            margin: 20px 0;
            padding: 20px 0;
            border-radius: 8px;
            background: rgba(255, 255, 255, 0.1);
        }

        .slides {
            display: flex;
            overflow: hidden;
        }

        .slides img {
            max-width: 100%;
            border-radius: 10px;
        }

        .slider-controls {
            position: absolute;
            bottom: 20px;
            left: 0;
            right: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 10px;
        }

        .slider-button {
            background: rgba(255, 215, 0, 0.2);
            border: none;
            color: #fff;
            padding: 8px 16px;
            cursor: pointer;
            border-radius: 4px;
        }

        .slider-button:hover,
        .slider-button:focus {
            background: rgba(255, 215, 0, 0.5);
        }

        .review-bubble {
            background: rgba(255, 215, 0, 0.2);
            border-radius: 15px;
            padding: 20px;
            margin: 10px auto;
            position: relative;
            max-width: 90%;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
            min-height: 275px;
            height: auto;
        }

        /* Media query improvements */
        @media (max-width: 600px) {
            nav ul li {
                display: block;
                margin: 5px 0;
            }

            nav ul li a {
                display: block;
                background-color: rgba(255, 215, 0, 0.3);
            }

            .review-bubble {
                padding: 15px;
            }
        }
    </style>
</head>

<body>
    <header>
        <div class="header-container">
            <img src="https://dimensionpowerwash.com/DP-MEDIA/logo.png" 
                 alt="Dimension Powerwash Logo" 
                 loading="lazy"
                 width="300"
                 height="300">
            <h1>Dimension Powerwash</h1>
            <p>Exterior Cleaning Specialists - Sheffield</p>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="#driveway-patio" aria-label="Learn about our drive and patio cleaning services">Drive & Patio Cleaning</a></li>
            <li><a href="#gutter-cleaning" aria-label="Learn about our gutter cleaning services">Gutter Cleaning</a></li>
            <li><a href="#customer-reviews" aria-label="See what our customers say">Reviews</a></li>
            <li><a href="#contact" aria-label="Contact us for a quote">Contact</a></li>
        </ul>
    </nav>

    <!-- Driveway & Patio Cleaning Section -->
    <section id="driveway-patio" class="section">
        <h2>Driveway & Patio Cleaning</h2>
        <div class="slider-container">
            <div class="slides">
                <img src="https://dimensionpowerwash.com/DP-MEDIA/Drive%20Cleaning.png" alt="Driveway Cleaning">
                <img src="https://dimensionpowerwash.com/DP-MEDIA/Patio%20Cleaning.png" alt="Patio Cleaning">
            </div>
            <div class="slider-controls">
                <button class="slider-button" onclick="sliders['driveway-patio'].prev()">Prev</button>
                <button class="slider-button" onclick="sliders['driveway-patio'].next()">Next</button>
            </div>
        </div>
    </section>

    <!-- Gutter Cleaning Section -->
    <section id="gutter-cleaning" class="section">
        <h2>Gutter Cleaning</h2>
        <div class="slider-container">
            <div class="slides">
                <img src="https://dimensionpowerwash.com/DP-MEDIA/Fascia%20Cleaning.png" alt="Fascia Cleaning">
                <img src="https://dimensionpowerwash.com/DP-MEDIA/Free%20Gutter%20CHECK.png" alt="Gutter Cleaning">
            </div>
            <div class="slider-controls">
                <button class="slider-button" onclick="sliders['gutter-cleaning'].prev()">Prev</button>
                <button class="slider-button" onclick="sliders['gutter-cleaning'].next()">Next</button>
            </div>
        </div>
    </section>

    <!-- Customer Reviews Section -->
    <section id="customer-reviews" class="section">
        <h2>What Our Customers Say About Us</h2>
        <div class="slider-container">
            <div class="slides">
                <div class="review-bubble">
                    <p>"Joe did a fantastic job cleaning my gutters. They look brand new!"</p>
                    <div class="stars">★★★★★ - Clare</div>
                </div>
                <div class="review-bubble">
                    <p>"The driveway looks amazing after the pressure washing. Highly recommend!"</p>
                    <div class="stars">★★★★★ - Peter</div>
                </div>
                <div class="review-bubble">
                    <p>"Very professional service, and my patio has never looked better!"</p>
                    <div class="stars">★★★★★ - M</div>
                </div>
                <div class="review-bubble">
                    <p>"Excellent work on both the gutters and the patio. Will definitely book again."</p>
                    <div class="stars">★★★★★ - Sam</div>
                </div>
            </div>
            <div class="slider-controls">
                <button class="slider-button" onclick="sliders['customer-reviews'].prev()">Prev</button>
                <button class="slider-button" onclick="sliders['customer-reviews'].next()">Next</button>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="section">
        <h2>Contact Us</h2>
        <p>Call us at 0114 457 3009 / 07494503865</p>
        <p><a href="https://calendly.com/dimensionpowerwash/free-quote" style="color: #FFD700;">Book a Free Quote</a></p>
        <p><a href="https://facebook.com/dimensionpowerwash" style="color: #FFD700;">Follow us on Facebook</a></p>
    </section>

    <!-- Script for Sliders -->
    <script>
        let sliders = {};

        function Slider(id) {
            this.container = document.querySelector(`#${id} .slides`);
            this.currentSlide = 0;
            this.slides = this.container.children;

            this.showSlide = (index) => {
                if (index >= this.slides.length) index = 0;
                if (index < 0) index = this.slides.length - 1;
                this.currentSlide = index;
                this.container.style.transform = `translateX(-${index * 100}%)`;
            };

            this.next = () => this.showSlide(this.currentSlide + 1);
            this.prev = () => this.showSlide(this.currentSlide - 1);
        }

        document.addEventListener('DOMContentLoaded', () => {
            try {
                sliders['driveway-patio'] = new Slider('driveway-patio');
                sliders['gutter-cleaning'] = new Slider('gutter-cleaning');
                sliders['customer-reviews'] = new Slider('customer-reviews');
            } catch (error) {
                console.error('Error initializing sliders:', error);
            }
        });
    </script>
</body>
</html>