<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        /* Global styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #000; /* Main background black */
            color: #FFF; /* Body text white */
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
            flex-direction: column; /* Aligns items in a column */
            align-items: center;    /* Centers items horizontally */
        }

        .header-container img {
            height: 300px;
            width: auto;
            display: block; /* Center the logo */
            margin: 0 auto; /* Center the logo */
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
            padding: 10px 15px; /* Add padding */
            border-radius: 5px; /* Rounded corners */
            background-color: rgba(255, 215, 0, 0.2); /* Light background for contrast */
            transition: background-color 0.3s ease; /* Smooth transition */
        }

        nav ul li a:hover {
            background-color: rgba(255, 215, 0, 0.5); /* Darker on hover */
        }

        /* Slider styles */
        .slider {
            width: 100%; 
            height: 0; /* Set height to zero */
            padding-top: 100%; /* Maintain a square aspect ratio */
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
            bottom: 0; /* Fill the parent */
            display: flex;
            transition: transform 0.6s ease-in-out;
        }

        .slides img {
            width: 100%; 
            height: 100%; /* Set height to fill the slider */
            object-fit: contain; /* Change to 'contain' to fit the entire image */
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
            background-color: rgba(255, 215, 0, 0.8); /* Yellow background on hover */
        }

        section {
            padding: 40px 20px; /* Increased padding */
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
            color: #FFF; /* Change paragraph text to white */
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
        }

        footer a {
            color: #FFD700; /* Link color */
            text-decoration: none; /* Remove underline */
        }

        footer a:hover {
            text-decoration: underline; /* Underline on hover */
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
                font-size: 1.5em; /* Slightly smaller headings */
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

    <section id="driveway-patio">
        <h2>Driveway & Patio Cleaning</h2>
        <p>Remove ingrained dirt, moss, algae, lichen, and black spots with our professional cleaning services.
            <br /><br />
            We use softwashing and low-pressure cleaning techniques to ensure your surfaces are thoroughly
            cleaned without damage.
            <br /><br />
        </p>

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
        <p>Prevent expensive repairs caused by blockages, leaks, and debris.
            <br /><br />
            Our gutter cleaning services ensure that your gutters are free from obstructions, allowing rainwater
            to flow freely.
            <br /><br />
            We also offer a full gutter wash, including soffits and fascias.
            <br /><br />
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
        <br />
        <p>Or reach us on Facebook and WhatsApp.</p>
        <br />
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
            let slideIndex = Math.abs(parseInt(slidesContainer.style.transform.replace(/[^0-9]/g, '')) / 100) || 0;

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
