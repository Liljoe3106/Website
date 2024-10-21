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
        .stars {
            color: #FFD700; /* Yellow color */
            font-size: 1.2em; /* Adjust the size if needed */
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
            max-width: 1000px;
            margin: 0 auto;
            overflow: hidden;
            position: relative;
            background-color: #000;
            border: none;
        }

        .slides, .review-slides {
            display: flex;
            transition: transform 0.6s ease-in-out;
        }

        .slides img, .review-slides div {
            width: 100%;
            flex-shrink: 0;
        }

        .hidden {
            display: none;
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
            transition: background-color 0.3s ease;
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
            max-width: 90%;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
            height: 275px;
        }

        /* About section styles */
        .about-section {
            background-color: #111;
            padding: 40px 20px;
            text-align: center;
            margin: 0 auto;
            max-width: 800px;
        }

        .about-section h2 {
            color: #FFD700;
            margin-bottom: 15px;
            font-size: 1.8em;
        }

        .about-section p {
            color: #fff;
            font-size: 1.1em;
            line-height: 1.5;
        }

        /* Hidden class for slides */
        .hidden {
            display: none;
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
            <li><a href="#driveway-patio">Driveway & Patio Cleaning</a></li>
            <li><a href="#gutter-cleaning">Gutter Cleaning</a></li>
            <li><a href="#about">About Us</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <section id="customer-reviews">
        <h2>What Our Customers Say About Us</h2>
        <div class="review-slider">
            <div class="review-slides">
                <div class="review-bubble">
                    <p>"Had gutters cleaned out. 3 story house and high gutters but Joe did a great job with the sky vac and was really nice to deal with - highly recommend!"</p>
                    <p><strong>Clare</strong> <span class="stars">★★★★★</span></p>
                </div>
                <div class="review-bubble hidden">
                    <p>"Great communication and great job done. Gutters now clear of gunk - thanks Joe!"</p>
                    <p><strong>Peter</strong> <span class="stars">★★★★★</span></p>
                </div>
                <div class="review-bubble hidden">
                    <p>"Excellent service with a fair price! Joe cleaned our gutters, driveway, and patio. I highly recommend and I will be booking in the near future!"</p>
                    <p><strong>M</strong> <span class="stars">★★★★★</span></p>
                </div>
                <div class="review-bubble hidden">
                    <p>"Great service from Joe, getting my driveway clean, looks amazing thank you!"</p>
                    <p><strong>Sam</strong> <span class="stars">★★★★★</span></p>
                </div>
                <div class="review-bubble hidden">
                    <p>"I had Joe round yesterday to do a gutter check, very friendly professional service, procedure clearly explained and camera footage provided. Would definitely use again and highly recommend."</p>
                    <p><strong>Morag</strong> <span class="stars">★★★★★</span></p>
                </div>
                <div class="review-bubble hidden">
                    <p>"Gave a great service cleaning our blocked gutters, the price was good and also very friendly. Would highly Recommend!"</p>
                    <p><strong>Kenneth</strong> <span class="stars">★★★★★</span></p>
                </div>
            </div>
        </div>
    </section>

    <section id="driveway-patio">
        <h2>Driveway & Patio Cleaning</h2>
        <p>Remove ingrained dirt, moss, algae, lichen, and black spots with our professional cleaning services.</p>

        <div class="slider">
            <div class="slides">
                <img src="DP MEDIA/Block paving before after.png" alt="Block paving before after" loading="lazy">
                <img src="DP MEDIA/Patio before after.png" alt="Patio before after" loading="lazy">
                <img src="DP MEDIA/Path before after.png" alt="Path before after" loading="lazy">
            </div>
            <button class="prev" onclick="moveSlide(-1)">&#10094;</button>
            <button class="next" onclick="moveSlide(1)">&#10095;</button>
        </div>
    </section>

    <section id="gutter-cleaning">
        <h2>Gutter Cleaning</h2>
        <p>Keep your gutters clean and prevent damage to your property with our comprehensive gutter cleaning services.</p>
        
        <div class="gutter-slider">
            <div class="slides">
                <img src="DP MEDIA/Gutters before after.png" alt="Gutters before after" loading="lazy">
                <img src="DP MEDIA/Gutter vacuuming.png" alt="Gutter vacuuming" loading="lazy">
            </div>
            <button class="prev" onclick="moveSlide(-1)">&#10094;</button>
            <button class="next" onclick="moveSlide(1)">&#10095;</button>
        </div>
    </section>

    <section id="about">
        <div class="about-section">
            <h2>About Dimension Powerwash</h2>
            <p>At Dimension Powerwash, we are dedicated to providing top-quality exterior cleaning services to homeowners in Sheffield / Worksop and surrounding areas. We use the latest equipment and techniques to ensure your property looks its best. Whether it’s driveway and patio cleaning or gutter cleaning / clearing, we take pride in delivering exceptional results that enhance the appearance and longevity of your property.</p>
            <p>Our commitment to customer satisfaction and our attention to detail set us apart in the industry. With Dimension Powerwash, you can trust that your property is in good hands.</p>
        </div>
    </section>

    <footer id="contact">
        <h3>Contact Us</h3>
        <p>For a free quote, call us at:</p>
        <p><strong>0114 457 3009</strong> or <strong>07494503865</strong></p>
        <p><a href="https://calendly.com/dimensionpowerwash/free-quote" target="_blank">Book a Free Quote</a></p>
        <p>Follow us on <a href="https://facebook.com/dimensionpowerwash" target="_blank">Facebook</a></p>
    </footer>

    <script>
        let slideIndex = 0;

        function showSlides(slideClass) {
            const slides = document.querySelectorAll(`.${slideClass} .slides > div`);
            slides.forEach((slide, index) => {
                slide.style.display = (index === slideIndex) ? 'block' : 'none';
            });
        }

        function moveSlide(n) {
            slideIndex += n;
            const slider = document.querySelector('.slider') || document.querySelector('.gutter-slider');
            const slides = slider.querySelectorAll('.slides > div');
            if (slideIndex >= slides.length) slideIndex = 0;
            if (slideIndex < 0) slideIndex = slides.length - 1;
            showSlides(slider.classList[0]);
        }

        showSlides('review-slider');
        showSlides('slider');
        showSlides('gutter-slider');

        // Set automatic transitions for the review slider
        setInterval(() => {
            slideIndex++;
            const slider = document.querySelector('.review-slider');
            const slides = slider.querySelectorAll('.review-slides > div');
            if (slideIndex >= slides.length) slideIndex = 0;
            if (slideIndex < 0) slideIndex = slides.length - 1;
            showSlides('review-slider');
        }, 5000); // Change slide every 5 seconds
    </script>
</body>
</html>
