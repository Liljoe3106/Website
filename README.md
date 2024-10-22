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
    <meta property="og:image" content="DP MEDIA/logo.png">
    <meta property="og:url" content="https://yourwebsite.com">
    
    <!-- Favicon -->
    <link rel="icon" type="image/x-icon" href="DP MEDIA/favicon.ico">
    
    <style>
        /* Your existing styles remain the same, but add: */
        .slide-container {
            position: relative;
            max-width: 1000px;
            margin: 0 auto;
        }

        .slide-dots {
            text-align: center;
            margin-top: 10px;
        }

        .dot {
            height: 10px;
            width: 10px;
            margin: 0 5px;
            background-color: #bbb;
            border-radius: 50%;
            display: inline-block;
            cursor: pointer;
        }

        .dot.active {
            background-color: #FFD700;
        }

        /* Add animation for slide transitions */
        .slides img, .review-bubble {
            opacity: 0;
            transition: opacity 0.5s ease-in-out;
        }

        .slides img.active, .review-bubble.active {
            opacity: 1;
        }

        /* Add schema markup styles */
        .schema-hidden {
            display: none;
        }
    </style>
</head>

<body>
    <!-- Schema.org markup for local business -->
    <script type="application/ld+json" class="schema-hidden">
    {
      "@context": "https://schema.org",
      "@type": "LocalBusiness",
      "name": "Dimension Powerwash",
      "image": "DP MEDIA/logo.png",
      "description": "Professional exterior cleaning services in Sheffield",
      "address": {
        "@type": "PostalAddress",
        "addressLocality": "Sheffield",
        "addressRegion": "South Yorkshire",
        "addressCountry": "UK"
      },
      "geo": {
        "@type": "GeoCoordinates",
        "latitude": "YOUR_LATITUDE",
        "longitude": "YOUR_LONGITUDE"
      },
      "url": "https://yourwebsite.com",
      "telephone": "0114 457 3009",
      "areaServed": ["Sheffield", "Rotherham", "Worksop"]
    }
    </script>

    <!-- Your existing header and nav sections remain the same -->

    <!-- Modified sliders with dots navigation -->
    <section id="driveway-patio">
        <h2>Drive & Patio Cleaning</h2>
        <p>Remove ingrained dirt, moss, algae, lichen, and black spots with our professional cleaning services.</p>

        <div class="slide-container">
            <div class="slider">
                <div class="slides">
                    <img src="DP MEDIA/Block paving before after.png" alt="Before and after comparison of block paving cleaning" loading="lazy">
                    <img src="DP MEDIA/Patio before after.png" alt="Before and after comparison of patio cleaning" loading="lazy">
                </div>
            </div>
            <div class="slide-dots" id="driveway-dots"></div>
        </div>
    </section>

    <!-- Modified JavaScript with improved functionality -->
    <script>
        let slideIndex = 0;
        let reviewIndex = 0;

        function createDots(containerID, count) {
            const container = document.getElementById(containerID);
            for (let i = 0; i < count; i++) {
                const dot = document.createElement('span');
                dot.className = 'dot';
                dot.onclick = () => currentSlide(i, containerID);
                container.appendChild(dot);
            }
            updateDots(containerID, 0);
        }

        function updateDots(containerID, index) {
            const dots = document.querySelectorAll(`#${containerID} .dot`);
            dots.forEach((dot, i) => {
                dot.classList.toggle('active', i === index);
            });
        }

        function currentSlide(n, containerID) {
            const slides = document.querySelectorAll(`#${containerID.split('-')[0]} .slides img`);
            slideIndex = n;
            showSlides(containerID.split('-')[0]);
        }

        function showSlides(containerId) {
            const slides = document.querySelectorAll(`#${containerId} .slides img`);
            slides.forEach(slide => {
                slide.classList.remove('active');
                slide.classList.add('hidden');
            });
            slides[slideIndex].classList.remove('hidden');
            setTimeout(() => slides[slideIndex].classList.add('active'), 50);
            updateDots(`${containerId}-dots`, slideIndex);
            slideIndex = (slideIndex + 1) % slides.length;
        }

        // Initialize dots for each slider
        document.addEventListener('DOMContentLoaded', () => {
            const sliderSections = ['driveway-patio', 'gutter-cleaning'];
            sliderSections.forEach(section => {
                const slides = document.querySelectorAll(`#${section} .slides img`);
                createDots(`${section}-dots`, slides.length);
            });

            // Start the automatic slideshow
            ['driveway-patio', 'gutter-cleaning'].forEach(section => {
                setInterval(() => showSlides(section), 3000);
            });
        });

        // Add touch support for mobile devices
        let touchStartX = 0;
        let touchEndX = 0;

        document.addEventListener('touchstart', e => {
            touchStartX = e.changedTouches[0].screenX;
        }, false);

        document.addEventListener('touchend', e => {
            touchEndX = e.changedTouches[0].screenX;
            handleSwipe();
        }, false);

        function handleSwipe() {
            const swipeThreshold = 50;
            if (touchEndX < touchStartX - swipeThreshold) {
                // Swipe left
                slideIndex = (slideIndex + 1) % document.querySelectorAll('.slides img').length;
                showSlides('driveway-patio');
            } else if (touchEndX > touchStartX + swipeThreshold) {
                // Swipe right
                slideIndex = (slideIndex - 1 + document.querySelectorAll('.slides img').length) % document.querySelectorAll('.slides img').length;
                showSlides('driveway-patio');
            }
        }
    </script>
</body>
</html>