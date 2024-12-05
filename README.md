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
            color: #FFD700; /* Yellow color for all section headings */
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

        /* New About Us Section */
        #about-us {
            padding: 40px 20px;
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
        }

        #about-us h2 {
            color: #FFD700; /* Yellow color for the title */
            margin-bottom: 15px;
            font-size: 1.8em;
        }

        #about-us p {
            color: #fff;
            font-size: 1.1em;
        }

        #about-us p strong {
            color: #FFD700; /* Yellow color for keywords */
        }

        /* Slider styles */
        .slider, .gutter-slider, .review-slider, .roof-slider {
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
            max-width: 90%;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
            height: 275px;
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

    <!-- New About Us Section -->
    <section id="about-us">
        <h2>About Us</h2>
        <p>Welcome to <strong>Dimension Powerwash</strong>! We are dedicated to providing high-quality exterior cleaning services, specializing in <strong>pressure washing</strong>, <strong>drive cleaning</strong>, <strong>patio cleaning</strong>, <strong>roof cleaning</strong> and <strong>gutter clearing/cleaning</strong>. Based in <strong>Sheffield</strong>, we proudly serve both residential and commercial clients across the city and surrounding areas, including <strong>Rotherham</strong> and <strong>Worksop</strong>. We are more than just a small jet wash company, with years of experience, our focus is on delivering outstanding results and ensuring customer satisfaction, helping to transform and maintain your outdoor spaces. Let us restore the beauty of your property with our professional cleaning services.</p>
    </section>

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
                    <p>"Great service from Joe getting our driveway clean, looks amazing thank you!"</p>
                    <p><strong>Sam</strong> <span class="stars">★★★★★</span></p>
                </div>
                <div class="review-bubble hidden">
                    <p>"Excellent service with a fair price! Joe cleaned our gutters, driveway and patio, I highly recommend and I will be booking in the near future!"</p>
                    <p><strong>M</strong> <span class="stars">★★★★★</span></p>
                </div>
            </div>
        </div>
    </section>

    <section id="driveway-patio">
        <h2>Drive & Patio Cleaning</h2>
        <u>
            <li>Remove <strong style="color: #FFD700;">ingrained dirt, moss, algae, and black spots</strong>.</li>
            <li>Bring up surfaces <strong style="color: #FFD700;">like new</strong>. </li>
            <li> Including <strong style="color: #FFD700;">Block Paving, Patio Stone, Walls, Paths, Tarmac, Resin & more</strong>.        
            </u>

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
        <p>Prevent expensive repairs caused by blockages, leaks, and debris with our gutter vacuum service. We will clear your gutters so that rain water can flow freely. We also offer a full washdown of the gutters and fascias should you want them looking like new!</p>

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
        <p>Your roof is the main reason your gutters get blocked, the growth of moss on your roof tiles can cause a handful of issues down the road, if left untreated. Wind, rainfall and the attraction of birds can cause this moss to block up your gutters and create enough organic growth for weeds to take root and cause further damage to your proprty. We offer a moss removal and anti-fungal wash treatment that not only prevents the growth of moss for years to come but acts as a self cleaning agent that will allow your roof to look cleaner and cleaner as the months go by. It's a much less invasive way of cleaning your roof compared to pressure washing.
        </p>

        <div class="roof-slider">
            <div class="slides">
                <img src="DP MEDIA/Roof Treatment.png" alt="Roof Treatment" loading="lazy">
            </div>
        </div>
    </section>

    <footer id="contact">
        <h3>Contact Us</h3>
        <br />
        <a href="https://calendly.com/dimensionpowerwash/free-quote" target="_blank">Get your free gutter check here, or book your free quote today!</a>
        <br /><br />
        <p>Call us today for a quote:</p>
        <p>0114 457 3009</p>
        <p>07494503865</p>
        <br />
        <p>Follow us on <a href="https://facebook.com/dimensionpowerwash" target="_blank">Facebook</a></p>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function () {
            document.querySelectorAll('.slider .slides img').forEach((slide, index) => {
                if (index === 0) slide.classList.remove('hidden');
                else slide.classList.add('hidden');
            });

            document.querySelectorAll('.gutter-slider .slides img').forEach((slide, index) => {
                if (index === 0) slide.classList.remove('hidden');
                else slide.classList.add('hidden');
            });

            document.querySelectorAll('.roof-slider .slides img').forEach((slide, index) => {
                if (index === 0) slide.classList.remove('hidden');
                else slide.classList.add('hidden');
            });

            document.querySelectorAll('.review-bubble').forEach((review, index) => {
                if (index === 0) review.classList.remove('hidden');
                else review.classList.add('hidden');
            });

            setInterval(showDrivewaySlides, 3000);
            setInterval(showGutterSlides, 3000);
            setInterval(showRoofSlides, 3000);
            setInterval(showReviewSlides, 5000);
        });

        let drivewaySlideIndex = 0;
        let gutterSlideIndex = 0;
        let roofSlideIndex = 0;
        let reviewIndex = 0;

        function showDrivewaySlides() {
            const slides = document.querySelectorAll('.slider .slides img');
            slides.forEach(slide => slide.classList.add('hidden'));
            drivewaySlideIndex = (drivewaySlideIndex + 1) % slides.length;
            slides[drivewaySlideIndex].classList.remove('hidden');
        }

        function showGutterSlides() {
            const slides = document.querySelectorAll('.gutter-slider .slides img');
            if (slides.length <= 1) return;
            slides.forEach(slide => slide.classList.add('hidden'));
            gutterSlideIndex = (gutterSlideIndex + 1) % slides.length;
            slides[gutterSlideIndex].classList.remove('hidden');
        }

        function showRoofSlides() {
            const slides = document.querySelectorAll('.roof-slider .slides img');
            if (slides.length <= 1) return;
            slides.forEach(slide => slide.classList.add('hidden'));
            roofSlideIndex = (roofSlideIndex + 1) % slides.length;
            slides[roofSlideIndex].classList.remove('hidden');
        }

        function showReviewSlides() {
            const reviews = document.querySelectorAll('.review-bubble');
            reviews.forEach(review => review.classList.add('hidden'));
            reviewIndex = (reviewIndex + 1) % reviews.length;
            reviews[reviewIndex].classList.remove('hidden');
        }
    </script>
</body>
</html>
