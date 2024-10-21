<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dimension Powerwash - Expert Exterior Cleaning in Sheffield</title>
    <meta name="description" content="Professional pressure washing, gutter cleaning, and patio cleaning services in Sheffield. Call us for a free quote!">
    <meta name="keywords" content="Pressure washing, gutter cleaning, patio cleaning, Sheffield, exterior cleaning">
    <style>
        /* General styles for sliders */
        .slider,
        .gutter-slider,
        .review-slider {
            position: relative;
            max-width: 100%;
            margin: auto;
            overflow: hidden;
        }

        .slides img,
        .review-bubble {
            width: 100%;
            display: block;
            opacity: 0;
            transition: opacity 0.5s ease-in-out;
        }

        .slides img.active,
        .review-bubble.active {
            opacity: 1;
        }

        /* Additional styles for the layout */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            background-color: black;
            color: white;
            padding: 10px 20px;
            text-align: center;
        }

        nav {
            margin-top: 10px;
        }

        main {
            padding: 20px;
            background-color: white;
        }

        section {
            margin-bottom: 20px;
        }

        footer {
            text-align: center;
            padding: 10px 0;
            background-color: black;
            color: white;
        }

        a {
            color: yellow;
            text-decoration: none;
        }

        a:hover {
            text-decoration: underline;
        }
    </style>
</head>

<body>

    <header>
        <img src="DP MEDIA/logo.png" alt="Dimension Powerwash Logo">
        <nav>
            <!-- Navigation links -->
        </nav>
    </header>

    <main>
        <section class="slider">
            <div class="slides">
                <img src="DP MEDIA/Drive Cleaning.png" alt="Driveway Cleaning">
                <img src="DP MEDIA/Patio Cleaning.png" alt="Patio Cleaning">
                <!-- Add other images here -->
            </div>
        </section>

        <section class="gutter-slider">
            <div class="slides">
                <img src="DP MEDIA/Fascia Cleaning.png" alt="Fascia Cleaning">
                <img src="DP MEDIA/Free Gutter CHECK.png" alt="Free Gutter Check">
                <!-- Add other images here -->
            </div>
        </section>

        <section class="review-slider">
            <div class="review-bubble active">Clare: Amazing job on my gutters! ★★★★★</div>
            <div class="review-bubble">Peter: My driveway looks brand new! ★★★★★</div>
            <div class="review-bubble">M: Excellent service and very professional! ★★★★★</div>
            <div class="review-bubble">Sam: Highly recommend for patio cleaning! ★★★★★</div>
        </section>

        <section>
            <h2>Contact Us</h2>
            <p>Call us at <a href="tel:01144573009">0114 457 3009</a> / <a href="tel:07494503865">07494503865</a></p>
            <p><a href="https://calendly.com/dimensionpowerwash/free-quote">Book a free quote</a></p>
        </section>

        <footer>
            <p>Follow us on <a href="https://facebook.com/dimensionpowerwash">Facebook</a></p>
        </footer>
    </main>

    <script>
        let sliderIndex = {
            'slider': 0,
            'gutter-slider': 0,
            'review-slider': 0
        };

        function showSlides(sliderClass) {
            const slides = document.querySelectorAll(`${sliderClass} .slides img, ${sliderClass} .review-bubble`);
            slides.forEach(slide => slide.classList.remove('active'));
            sliderIndex[sliderClass] = (sliderIndex[sliderClass] + 1) % slides.length;
            slides[sliderIndex[sliderClass]].classList.add('active');
        }

        // Initial setup
        document.querySelectorAll('.slides img, .review-bubble').forEach(item => item.classList.remove('active'));
        document.querySelector('.slider .slides img').classList.add('active');
        document.querySelector('.gutter-slider .slides img').classList.add('active');
        document.querySelector('.review-bubble').classList.add('active');

        // Unified slider intervals
        setInterval(() => showSlides('.slider'), 3000);
        setInterval(() => showSlides('.gutter-slider'), 3000);
        setInterval(() => showSlides('.review-slider'), 5000);
    </script>

    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "LocalBusiness",
      "name": "Dimension Powerwash",
      "image": "https://yourwebsite.com/DP MEDIA/logo.png",
      "address": {
        "@type": "PostalAddress",
        "addressLocality": "Sheffield",
        "addressRegion": "South Yorkshire",
        "postalCode": "S1",
        "addressCountry": "UK"
      },
      "url": "https://yourwebsite.com",
      "telephone": "0114 457 3009",
      "priceRange": "$$",
      "servesCuisine": "Cleaning Services",
      "geo": {
        "@type": "GeoCoordinates",
        "latitude": "53.3811",
        "longitude": "-1.4701"
      }
    }
    </script>

</body>

</html>
