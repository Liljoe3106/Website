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
            border: none;
        }

        .slides, .gutter-slides, .review-slides {
            display: flex;
            transition: transform 0.6s ease-in-out;
            width: 300%;
        }

        .slides img, .gutter-slides img {
            width: 100%; 
            flex-shrink: 0;
            object-fit: contain; /* Use contain to make images fit without cropping */
        }

        .review-slides .review-bubble {
            max-width: 100%;
            flex-shrink: 0;
            padding: 20px;
            margin: 10px;
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

        /* Review bubble styles */
        .review-bubble {
            background: rgba(255, 215, 0, 0.2);
            border-radius: 15px;
            padding: 20px;
            margin: 10px auto;
            position: relative;
            max-width: 90%; /* Increased max-width to give more space */
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
            height: auto; 
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
        }

        .review-bubble p {
            margin: 0;
        }

        .review-bubble strong {
            display: block;
            margin-top: 10px;
        }

        .review-bubble strong::after {
            content: " ★★★★★";
            color: #FFD700; 
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
        <h2>What Our Customers Say About Us</h2>
        <div class="review-slider">
            <div class="review-slides">
                <div class="review-bubble">
                    <p>"Had gutters cleaned out. 3 story house and high gutters but Joe did a great job with the sky vac and was really nice to deal with - highly recommend!"</p>
                    <p><strong>Clare</strong></p>
                </div>
                <div class="review-bubble">
                    <p>"Great communication and great job done. Gutters now clear of gunk - thanks Joe!"</p>
                    <p><strong>Peter</strong></p>
                </div>
                <div class="review-bubble">
                    <p>"Excellent service with a fair price! Joe cleaned our gutters, driveway, and patio. I highly recommend and I will be booking in the near future!"</p>
                    <p><strong>M</strong></p>
                </div>
                <div class="review-bubble">
                    <p>"Great service from Joe, getting my driveway clean, looks amazing thank you!"</p>
                    <p><strong>Sam</strong></p>
                </div>
                <div class="review-bubble">
                    <p>"Joe checked our gutters, Very friendly, professional service, procedure clearly explained and camera footage provided.would definitely use again and highly recommend."</p>
                    <p><strong>Morag</strong></p>
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
                <img src="DP MEDIA/Patio Cleaning.png" alt="Patio Cleaning">
            </div>
        </div>
    </section>

    <section id="gutter-cleaning">
        <h2>Gutter Cleaning</h2>
        <p>Prevent expensive repairs caused by blockages, leaks, and debris.</p>

        <div class="gutter-slider">
            <div class="gutter-slides">
                <img src="DP MEDIA/Free Gutter CHECK.png" alt="Free Gutter Check">
                <img src="DP MEDIA/Fascia Cleaning.png" alt="Fascia Cleaning">
            </div>
        </div>
    </section>

    <footer id="contact">
        <h3>Contact Us</h3>
        <br />
        <a href="https://calendly.com/dimensionpowerwash/free-quote" target="_blank">Book your free, no obligation quote here!</a>
        <br />
        <br />
        <p>Or Call/WhatsApp us at: <br /> 0114 457 3009 / 07494503865</p>
        <a href="https://www.facebook.com/dimensionpowerwash" target="_blank">Follow us on Facebook</a>
    </footer>

    <script>
        let slideIndex = 0;

        function showSlides(sliderClass) {
            const slides = document.querySelector(sliderClass + ' .slides');
            const totalSlides = slides.children.length;
            slideIndex = (slideIndex + 1) % totalSlides;
            slides.style.transform = `translateX(-${slideIndex * 100}%)`;
        }

        function showGutterSlides() {
            const slides = document.querySelector('.gutter-slider .gutter-slides');
            const totalSlides = slides.children.length;
            slideIndex = (slideIndex + 1) % totalSlides;
            slides.style.transform = `translateX(-${slideIndex * 100}%)`;
        }

        function showReviewSlides() {
            const slides = document.querySelector('.review-slider .review-slides');
            const totalSlides = slides.children.length;
            slideIndex = (slideIndex + 1) % totalSlides;
            slides.style.transform = `translateX(-${slideIndex * 100}%)`;
        }

        // Set intervals for each slider
        setInterval(() => showSlides('.slider'), 3000);  // For Driveway & Patio Cleaning slider
        setInterval(() => showGutterSlides(), 3000);    // For Gutter Cleaning slider
        setInterval(() => showReviewSlides(), 3000);    // For Review slider
    </script>
</body>
</html>
