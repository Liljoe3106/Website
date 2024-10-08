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

        /* Slider styles */
        .slider, .gutter-slider, .review-slider {
            width: 100%;
            max-width: 800px;
            margin: 0 auto;
            overflow: hidden;
            position: relative;
            background-color: #000;
            border: 5px solid #FFD700;
        }

        .slides, .review-slides {
            display: flex;
            transition: transform 0.6s ease-in-out;
        }

        .slides img {
            width: 100%;
            flex-shrink: 0;
        }

        .review-slides div {
            min-width: 100%;
            flex-shrink: 0;
            padding: 20px;
            box-sizing: border-box;
            height: 250px; /* Increased box height to fit reviews */
        }

        .review-slides div p {
            font-size: 1.1em;
            line-height: 1.5;
            color: #fff;
        }

        .review-slides p strong {
            font-size: 1.2em;
        }

        .review-slides p.stars {
            color: #FFD700; /* Yellow stars */
            font-size: 1.2em;
            margin-top: 5px;
        }

        .prev, .next {
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

        .prev:hover, .next:hover {
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

        /* Responsive styles */
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

    <section id="customer-reviews">
        <h2>What our customers say about us</h2>
        <div class="review-slider">
            <div class="review-slides">
                <div>
                    <p>"Had gutters cleaned out. 3 story house and high gutters but Joe did a great job with the sky vac and was really nice to deal with - highly recommend!"</p>
                    <p><strong>Clare</strong></p>
                    <p class="stars">★★★★★</p>
                </div>
                <div>
                    <p>"Great communication and great job done. Gutters now clear of gunk - thanks Joe!"</p>
                    <p><strong>Peter</strong></p>
                    <p class="stars">★★★★★</p>
                </div>
                <div>
                    <p>"Excellent service with a fair price! Joe cleaned our gutters, driveway, and patio. I highly recommend and I will be booking in the near future!"</p>
                    <p><strong>M</strong></p>
                    <p class="stars">★★★★★</p>
                </div>
                <div>
                    <p>"Great service from Joe, getting my driveway clean, looks amazing thank you!"</p>
                    <p><strong>Sam</strong></p>
                    <p class="stars">★★★★★</p>
                </div>
                <div>
                    <p>"I had Joe round yesterday for a gutter check, very friendly professional service, procedure clearly explained and camera footage provided. Reliable, arrived as expected, price clearly explained, excellent service, would definitely use again and highly recommend."</p>
                    <p><strong>Morag</strong></p>
                    <p class="stars">★★★★★</p>
                </div>
            </div>
        </div>
    </section>

    <section id="driveway-patio">
        <h2>Driveway & Patio Cleaning</h2>
        <p>Remove ingrained dirt, moss, algae, lichen, and black spots with our professional cleaning services.</p>

        <div class="slider">
            <div class="slides">
                <img src="DP MEDIA/Drive Cleaning.png" alt="Driveway Cleaning">
                <img src="DP MEDIA/Patio Cleaning.png" alt="Patio Cleaning"> <!-- Fixed image path -->
                <img src="DP MEDIA/Driveway After Clean.png" alt="Driveway After Clean">
                <img src="DP MEDIA/Driveway Clean Before After.png" alt="Driveway Clean Before and After">
            </div>
        </div>
    </section>

    <section id="gutter-cleaning">
        <h2>Gutter Cleaning</h2>
        <p>Prevent expensive repairs caused by blockages, leaks, and debris.</p>

        <div class="gutter-slider">
            <div class="slides">
                <img src="DP MEDIA/Free Gutter CHECK.png" alt="Free Gutter Check">
                <img src="DP MEDIA/Fascia Cleaning.png" alt="Fascia Cleaning"> <!-- Fixed image path -->
                <img src="DP MEDIA/Gutter Vacuum.png" alt="Gutter Vacuum Cleaning">
                <img src="DP MEDIA/Gutter Cleaning Before and After.png" alt="Gutter Cleaning Before and After">
            </div>
        </div>
    </section>

    <footer id="contact">
        <h3>Contact Us</h3>
        <p>Phone: <a href="tel:07934728960">07934 728 960</a></p>
        <p>Email: <a href="mailto:info@dimensionpowerwash.com">info@dimensionpowerwash.com</a></p>
    </footer>

    <script>
        let slideIndex = 0;
        let reviewIndex = 0;

        function showSlides(className) {
            const slides = document.querySelectorAll(className);
            slideIndex++;
            if (slideIndex >= slides[0].children.length) {
                slideIndex = 0;
            }
            slides.forEach(slide => {
                slide.style.transform = `translateX(${-100 * slideIndex}%)`;
            });
        }

        function showReviewSlides() {
            const reviewSlides = document.querySelector('.review-slides');
            reviewIndex++;
            if (reviewIndex >= reviewSlides.children.length) {
                reviewIndex = 0;
            }
            reviewSlides.style.transform = `translateX(${-100 * reviewIndex}%)`;
        }

        setInterval(() => {
            showSlides('.slider');
            showSlides('.gutter-slider');
            showReviewSlides();
        }, 5000);
    </script>
</body>
</html>