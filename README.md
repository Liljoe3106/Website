<html lang="en">

    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dimension Powerwash</title>
    <style>
        /* Global styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #fff;
            color: #333;
            box-sizing: border-box;
        }

        /* er styles */
        er {
            background-color: #000;
            color: #FFD700;
            padding: 20px 0;
            text-align: center;
        }

        .header-container h1 {
            margin: 0;
            font-size: 2.5em; /* Increased size */
        }

        .header-container p {
            margin: 5px 0 0;
            font-size: 1.2em;
            color: #fff;
        }

        /* Navigation styles */
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
        }

        /* Slider styles */
        .slider {
            max-width: 100%;
            width: 100%;
            height: 1080px; /* Set height to 1080 for square */
            margin: 20px auto;
            position: relative;
            overflow: hidden;
            background-color: #000;
            border: 5px solid #FFD700;
        }

        .slides {
            display: flex;
            transition: transform 0.6s ease-in-out;
            height: 100%;
        }

        .slides img {
            width: 100%;
            height: 100%;
            object-fit: contain; /* Changed to 'contain' for better fitting */
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
            background-color: rgba(0, 0, 0, 0.8);
        }

        /* Section styles */
        section {
            padding: 20px;
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
        }

        section h2 {
            color: #FFD700;
            margin-bottom: 15px;
            font-size: 2em; /* Increased size */
        }

        section p {
            color: #333;
            font-size: 1.1em;
            line-height: 1.5; /* Added line-height for readability */
        }

        /* Footer styles */
        footer {
            background-color: #000;
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
        }

        /* Responsive styles */
        @media (max-width: 800px) {
            section {
                padding: 15px;
            }

            footer {
                padding: 15px;
            }
        }

        @media (max-width: 600px) {
            nav ul li {
                display: block;
                margin: 5px 0;
            }
        }
    </style>

<body>
    <header>
        <div class="header-container">
            <img src="DP MEDIA/logo.png" alt="Dimension Powerwash Logo" style="height: 300px; width: auto;">
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

    <section id="driveway-patio">
        <h2>Driveway & Patio Cleaning</h2>
        <p>Remove ingrained dirt, moss, algae, lichen, and black spots with our professional cleaning services.
            <br><br>
            We use softwashing and low-pressure cleaning techniques to ensure your surfaces are thoroughly cleaned without damage.
        </p>

        <div class="slider">
            <div class="slides">
                <img src="DP MEDIA/Drive Cleaning.png" alt="Drive Cleaning">
                <img src="DP MEDIA/Patio Cleaning.png" alt="Patio Cleaning">
            </div>
            <a class="prev" onclick="plusSlides(-1, '.slider')">&#10094;</a>
            <a class="next" onclick="plusSlides(1, '.slider')">&#10095;</a>
        </div>
    </section>

    <section id="gutter-cleaning">
        <h2>Gutter Cleaning</h2>
        <p>Prevent expensive repairs caused by blockages, leaks, and debris.
            <br><br>
            Our gutter cleaning services ensure that your gutters are free from obstructions, allowing rainwater to flow freely.
            <br><br>
            We also offer a full gutter wash, including soffits and facias.
        </p>

        <div class="slider gutter-slider">
            <div class="slides">
                <img src="DP MEDIA/Free Gutter CHECK.png" alt="Free Gutter Check">
                <img src="DP MEDIA/Facia Cleaning.png" alt="Facia Cleaning">
            </div>
            <a class="prev" onclick="plusSlides(-1, '.gutter-slider')">&#10094;</a>
            <a class="next" onclick="plusSlides(1, '.gutter-slider')">&#10095;</a>
        </div>
    </section>

    <footer id="contact">
        <h3>Contact Us</h3>
        <p>For a free quote, call Joe at:</p>
        <p>Phone: 0114 457 3009 / 07494 503 865</p>
        <br>
        <p>Or reach us on Facebook and WhatsApp.</p>
        <br>
        <a href="https://www.facebook.com/dimensionpowerwash" target="_blank">
            Follow us on Facebook!
        </a>
    </footer>

    <script>
        function showSlides(slidesClass, initialIndex = 0) {
            let slideIndex = initialIndex;
            const slidesContainer = document.querySelector(slidesClass);
            const slides = slidesContainer.querySelectorAll('img');
            const totalSlides = slides.length;

            function displaySlides() {
                slidesContainer.style.transform = `translateX(-${slideIndex * 100}%)`;

                slideIndex = (slideIndex + 1) % totalSlides;

                setTimeout(displaySlides, 5000); // Change image every 5 seconds
            }

            displaySlides();
        }

        function plusSlides(n, slidesClass) {
            const slidesContainer = document.querySelector(slidesClass + ' .slides');
            const slides = slidesContainer.querySelectorAll('img');
            const totalSlides = slides.length;
            let slideIndex = [...slides].findIndex(slide => slide.style.transform === 'translateX(0%)');

            slideIndex += n;

            if (slideIndex >= totalSlides) {
                slideIndex = 0;
            } else if (slideIndex < 0) {
                slideIndex = totalSlides - 1;
            }

            slidesContainer.style.transform = `translateX(-${slideIndex * 100}%)`;
        }

        showSlides('.slider .slides'); // For the Driveway/Patio Cleaning slider
        showSlides('.gutter-slider .slides'); // For the new Gutter Cleaning slider
    </script>
</body>

</html>
