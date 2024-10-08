<html lang="en">
<head>
    <style>
        /* Global styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #000; /* Black background */
            color: #fff; /* White text */
            box-sizing: border-box;
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

        .header-container p {
            color: #fff;
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

        .slider {
            width: 100%;
            height: 0;
            padding-top: 100%;
            position: relative;
            overflow: hidden;
            background-color: #000;
            border: 5px solid #FFD700;
        }

        .slides {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            display: flex;
            transition: transform 0.6s ease-in-out;
        }

        .slides img {
            width: 100%;
            height: 100%;
            object-fit: contain;
            flex-shrink: 0;
            display: block;
        }

        .prev,
        .next {
            cursor: pointer;
            position: absolute;
            top: 50%;
            width: auto;
            margin-top: -22px;
            padding: 16px;
            color: white;
            font-weight: bold;
            font-size: 18px;
            transition: 0.6s ease;
            border-radius: 0 3px 3px 0;
            user-select: none;
        }

        .next {
            right: 0;
            border-radius: 3px 0 0 3px;
        }

        .prev:hover,
        .next:hover {
            background-color: rgba(255, 215, 0, 0.8);
        }

        section {
            padding: 40px 20px;
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
        }

        section h2 {
            color: #FFD700;
            margin-bottom: 15px;
            font-size: 1.8em;
        }

        section p {
            color: #fff;
            font-size: 1.1em;
        }

        footer {
            background: linear-gradient(90deg, #000, #333);
            color: #FFD700;
            padding: 20px 0;
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
        }

        footer h3 {
            margin-bottom: 10px;
            font-size: 1.5em;
        }

        footer p {
            margin: 5px 0;
            font-size: 1.1em;
            color: #fff;
        }

        footer a {
            color: #FFD700;
            text-decoration: underline;
        }

        footer a:hover {
            text-decoration: underline;
        }

        @media (max-width: 800px) {
            section {
                padding: 15px;
            }

            footer {
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
            <img src="DP MEDIA/logo.png" alt="Dimension Powerwash Logo">
            <h1>Dimension Powerwash</h1>
            <p>Remove the grime, and bring back the shine!</p>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="#driveway-patio">Driveway & Patio Cleaning</a></li>
            <li><a href="#gutter-cleaning">Gutter Cleaning</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Customer Reviews Slider -->
    <section id="customer-reviews">
        <h2>What our customers say about us</h2>
        <div class="review-slider">
            <div class="review-slides">
                <div class="review">
                    <p>Clare - ★★★★★</p>
                    <p>Had gutters cleaned out. 3 story house and high gutters but Joe did a great job with the sky vac and was really nice to deal with - highly recommend!</p>
                </div>
                <div class="review">
                    <p>Peter - ★★★★★</p>
                    <p>Great communication and great job done. Gutters now clear of gunk - thanks Joe!</p>
                </div>
                <div class="review">
                    <p>M - ★★★★★</p>
                    <p>Excellent service with a fair price! Joe cleaned our gutters, driveway and patio. I highly recommend and I will be booking in the near future!</p>
                </div>
                <div class="review">
                    <p>Sam - ★★★★★</p>
                    <p>Great service from Joe, getting my driveway clean, looks amazing thank you!</p>
                </div>
            </div>
            <a class="prev" onclick="plusReviewSlides(-1)">&#10094;</a>
            <a class="next" onclick="plusReviewSlides(1)">&#10095;</a>
        </div>
    </section>

    <section id="driveway-patio">
        <h2>Driveway & Patio Cleaning</h2>
        <p>Remove ingrained dirt, moss, algae, lichen, and black spots with our professional cleaning services.</p>
        <div class="slider">
            <div class="slides">
                <img src="DP MEDIA/Drive Cleaning.png" alt="Driveway Cleaning">
                <img src="DP MEDIA/Patio Cleaning.png" alt="Patio Cleaning">
            </div>
            <a class="prev" onclick="plusSlides(-1, '.slider')">&#10094;</a>
            <a class="next" onclick="plusSlides(1, '.slider')">&#10095;</a>
        </div>
    </section>

    <section id="gutter-cleaning">
        <h2>Gutter Cleaning</h2>
        <p>Prevent expensive repairs caused by blockages, leaks, and debris. Our gutter cleaning services ensure that your gutters are free from obstructions, allowing rainwater to flow freely.</p>
        <div class="slider gutter-slider">
            <div class="slides">
                <img src="DP MEDIA/Free Gutter CHECK.png" alt="Free Gutter Check">
                <img src="DP MEDIA/Fascia Cleaning.png" alt="Fascia Cleaning">
            </div>
            <a class="prev" onclick="plusSlides(-1, '.gutter-slider')">&#10094;</a>
            <a class="next" onclick="plusSlides(1, '.gutter-slider')">&#10095;</a>
        </div>
    </section>

    <!-- Contact Section -->
    <footer id="contact">
        <h3>Contact Us</h3>
        <p>For a free quote, call Joe at:</p>
        <p>Phone: 0114 457 3009 / 07494 503 865</p>
        <br />
        <p>Or reach us on Facebook and WhatsApp.</p>
        <br />
        <a href="https://www.facebook.com/dimensionpowerwash" target="_blank">Follow us on Facebook!</a>
    </footer>

    <script>
        let reviewIndex = 0;

        function showReviewSlides() {
            const reviewSlides = document.querySelector('.review-slides');
            const reviews = document.querySelectorAll('.review');
            const totalReviews = reviews.length;

            reviewSlides.style.transform = `translateX(-${reviewIndex * 100}%)`;

            reviewIndex = (reviewIndex + 1) % totalReviews;

            setTimeout(showReviewSlides, 7000); // Change review every 7 seconds
        }

        function plusReviewSlides(n) {
            const reviews = document.querySelectorAll('.review');
            const
            totalReviews = reviews.length;

            reviewIndex += n;
            if (reviewIndex >= totalReviews) {
                reviewIndex = 0;
            } else if (reviewIndex < 0) {
                reviewIndex = totalReviews - 1;
            }

            const reviewSlides = document.querySelector('.review-slides');
            reviewSlides.style.transform = `translateX(-${reviewIndex * 100}%)`;
        }

        let slideIndex = 0;

        function showSlides(sliderSelector) {
            const slides = document.querySelectorAll(`${sliderSelector} .slides img`);
            const totalSlides = slides.length;

            slides.forEach((slide, i) => {
                slide.style.display = i === slideIndex ? 'block' : 'none';
            });

            slideIndex = (slideIndex + 1) % totalSlides;

            setTimeout(() => showSlides(sliderSelector), 5000); // Change image every 5 seconds
        }

        function plusSlides(n, sliderSelector) {
            const slides = document.querySelectorAll(`${sliderSelector} .slides img`);
            const totalSlides = slides.length;

            slideIndex += n;
            if (slideIndex >= totalSlides) {
                slideIndex = 0;
            } else if (slideIndex < 0) {
                slideIndex = totalSlides - 1;
            }

            slides.forEach((slide, i) => {
                slide.style.display = i === slideIndex ? 'block' : 'none';
            });
        }

        document.addEventListener('DOMContentLoaded', () => {
            showSlides('.slider');
            showSlides('.gutter-slider');
            showReviewSlides();
        });
    </script>
</body>
</html>
