<html lang="en">
<head>
    <style>
        /* Global styles - the same as your original code */
    </style>
</head>
<body>
    <header>
        <div class="header-container">
            <img src="DP MEDIA/logo.png" alt="Dimension Powerwash Logo">
            <h1>Dimension Powerwash</h1>
            <p>Exterior Cleaning Specialists - Sheffield</p>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="driveway-patio.html">Driveway & Patio Cleaning</a></li>
            <li><a href="gutter-cleaning.html">Gutter Cleaning</a></li>
            <li><a href="contact.html">Contact</a></li>
        </ul>
    </nav>

    <section id="customer-reviews">
        <h2>What Our Customers Say About Us</h2>
        <div class="review-slider">
            <div class="review-slides">
                <div class="review-bubble">
                    <p>"Had gutters cleaned out. 3 story house and high gutters but Joe did a great job with the sky vac and was really nice to deal with - highly recommend!"</p>
                    <p><strong>Clare</strong> ★★★★★</p>
                </div>
                <div class="review-bubble">
                    <p>"Great communication and great job done. Gutters now clear of gunk - thanks Joe!"</p>
                    <p><strong>Peter</strong> ★★★★★</p>
                </div>
                <!-- Additional reviews here -->
            </div>
        </div>
    </section>

    <!-- Contact section, same across all pages -->
    <footer id="contact">
        <h3>Contact Us</h3>
        <a href="https://calendly.com/dimensionpowerwash/free-quote" target="_blank">Get your free gutter check here, or book your free quote today!</a>
        <p>Phone: 0114 457 3009</p>
        <p>Follow us on <a href="https://facebook.com/dimensionpowerwash" target="_blank">Facebook</a>!</p>
    </footer>

    <script>
        let reviewIndex = 0;

        function showReviewSlides() {
            const reviewSlides = document.querySelectorAll('.review-slides .review-bubble');
            const totalReviews = reviewSlides.length;
            reviewIndex = (reviewIndex + 1) % totalReviews;
            for (let i = 0; i < totalReviews; i++) {
                reviewSlides[i].style.display = (i === reviewIndex) ? "block" : "none";
            }
        }

        setInterval(showReviewSlides, 5000);
    </script>
</body>
</html>



<html lang="en">
<head>
    <style>
        /* Global styles - the same as your original code */
    </style>
</head>
<body>
    <header>
        <div class="header-container">
            <img src="DP MEDIA/logo.png" alt="Dimension Powerwash Logo">
            <h1>Dimension Powerwash</h1>
            <p>Exterior Cleaning Specialists - Sheffield</p>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="gutter-cleaning.html">Gutter Cleaning</a></li>
            <li><a href="contact.html">Contact</a></li>
        </ul>
    </nav>

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

    <!-- Contact section, same across all pages -->
    <footer id="contact">
        <h3>Contact Us</h3>
        <a href="https://calendly.com/dimensionpowerwash/free-quote" target="_blank">Get your free gutter check here, or book your free quote today!</a>
        <p>Phone: 0114 457 3009</p>
        <p>Follow us on <a href="https://facebook.com/dimensionpowerwash" target="_blank">Facebook</a>!</p>
    </footer>

    <script>
        let slideIndex = 0;

        function showSlides() {
            const slides = document.querySelectorAll('.slider .slides img');
            const totalSlides = slides.length;
            slideIndex = (slideIndex + 1) % totalSlides;
            for (let i = 0; i < totalSlides; i++) {
                slides[i].style.display = (i === slideIndex) ? "block" : "none";
            }
        }

        setInterval(showSlides, 3000);
    </script>
</body>
</html>



<html lang="en">
<head>
    <style>
        /* Global styles - the same as your original code */
    </style>
</head>
<body>
    <header>
        <div class="header-container">
            <img src="DP MEDIA/logo.png" alt="Dimension Powerwash Logo">
            <h1>Dimension Powerwash</h1>
            <p>Exterior Cleaning Specialists - Sheffield</p>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="driveway-patio.html">Driveway & Patio Cleaning</a></li>
            <li><a href="contact.html">Contact</a></li>
        </ul>
    </nav>

    <section id="gutter-cleaning">
        <h2>Gutter Cleaning</h2>
        <p>Prevent expensive repairs caused by blockages, leaks, and debris.</p>

        <div class="gutter-slider">
            <div class="slides">
                <img src="DP MEDIA/Free Gutter CHECK.png" alt="Free Gutter Check">
                <img src="DP MEDIA/Fascia Cleaning.png" alt="Fascia Cleaning">
            </div>
        </div>
    </section>

    <!-- Contact section, same across all pages -->
    <footer id="contact">
        <h3>Contact Us</h3>
        <a href="https://calendly.com/dimensionpowerwash/free-quote" target="_blank">Get your free gutter check here, or book your free quote today!</a>
        <p>Phone: 0114 457 3009</p>
        <p>Follow us on <a href="https://facebook.com/dimensionpowerwash" target="_blank">Facebook</a>!</p>
    </footer>

    <script>
        let slideIndex = 0;

        function showSlides() {
            const slides = document.querySelectorAll('.gutter-slider .slides img');
            const totalSlides = slides.length;
            slideIndex = (slideIndex + 1) % totalSlides;
            for (let i = 0; i < totalSlides; i++) {
                slides[i].style.display = (i === slideIndex) ? "block" : "none";
            }
        }

        setInterval(showSlides, 3000);
    </script>
</body>
</html>




<html lang="en">
<head>
    <style>
        /* Global styles - the same as your original code */
    </style>
</head>
<body>
    <header>
        <div class="header-container">
            <img src="DP MEDIA/logo.png" alt="Dimension Powerwash Logo">
            <h1>Dimension Powerwash</h1>
            <p>Exterior Cleaning Specialists - Sheffield</p>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="driveway-patio.html">Driveway & Patio Cleaning</a></li>
            <li><a href="gutter-cleaning.html">Gutter Cleaning</a></li>
        </ul>
    </nav>

    <section id="contact-info">
        <h2>Contact Us</h2>
        <p>We’re here to help with any exterior cleaning services!</p>
        <p>Phone: 0114 457 3009</p>
        <a href="https://calendly.com/dimensionpowerwash/free-quote" target="_blank">Book your free quote here!</a>
    </section>

    <!-- Contact section, same across all pages -->
    <footer id="contact">
        <h3>Contact Us</h3>
        <a href="https://calendly.com/dimensionpowerwash/free-quote" target="_blank">Get your free gutter check here, or book your free quote today!</a>
        <p>Phone: 0114 457 3009</p>
        <p>Follow us on <a href="https://facebook.com/dimensionpowerwash" target="_blank">Facebook</a>!</p>
    </footer>
</body>
</html>