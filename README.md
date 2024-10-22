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
    <meta property="og:image" content="https://dimensionpowerwash.com/DP-MEDIA/logo.png">
    <meta property="og:url" content="https://dimensionpowerwash.com">
    
    <style>
        /* Global styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #000;
            color: #fff;
            box-sizing: border-box;
            line-height: 1.6;
        }

        /* Global heading styles */
        h2, h3 {
            color: #FFD700;
        }

        /* Focus styles for accessibility */
        a:focus, button:focus {
            outline: 3px solid #FFD700;
            outline-offset: 2px;
        }

        .stars {
            color: #FFD700;
            font-size: 1.2em;
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
            display: inline-block;
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

        nav ul li a:hover,
        nav ul li a:focus {
            background-color: rgba(255, 215, 0, 0.5);
        }

        .review-bubble {
            background: rgba(255, 215, 0, 0.2);
            border-radius: 15px;
            padding: 20px;
            margin: 10px auto;
            position: relative;
            max-width: 90%;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
            min-height: 275px;
            height: auto;
        }

        /* Slider improvements */
        .slider-container {
            position: relative;
        }

        .slider-controls {
            position: absolute;
            bottom: 20px;
            left: 0;
            right: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 10px;
        }

        .slider-button {
            background: rgba(255, 215, 0, 0.2);
            border: none;
            color: #fff;
            padding: 8px 16px;
            cursor: pointer;
            border-radius: 4px;
        }

        .slider-button:hover,
        .slider-button:focus {
            background: rgba(255, 215, 0, 0.5);
        }

        /* Media query improvements */
        @media (max-width: 600px) {
            nav ul li {
                display: block;
                margin: 5px 0;
            }

            nav ul li a {
                display: block;
                background-color: rgba(255, 215, 0, 0.3);
            }

            .review-bubble {
                padding: 15px;
            }
        }
    </style>
</head>

<body>
    <!-- Schema.org markup with absolute URLs -->
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "LocalBusiness",
      "name": "Dimension Powerwash",
      "image": "https://dimensionpowerwash.com/DP-MEDIA/logo.png",
      "description": "Professional exterior cleaning services in Sheffield",
      "address": {
        "@type": "PostalAddress",
        "addressLocality": "Sheffield",
        "addressRegion": "South Yorkshire",
        "addressCountry": "UK"
      },
      "url": "https://dimensionpowerwash.com",
      "telephone": "0114 457 3009",
      "areaServed": ["Sheffield", "Rotherham", "Worksop"]
    }
    </script>

    <!-- Rest of the HTML structure remains similar but with improved accessibility -->
    <header>
        <div class="header-container">
            <img src="https://dimensionpowerwash.com/DP-MEDIA/logo.png" 
                 alt="Dimension Powerwash Logo" 
                 loading="lazy"
                 width="300"
                 height="300">
            <h1>Dimension Powerwash</h1>
            <p>Exterior Cleaning Specialists - Sheffield</p>
        </div>
    </header>

    <!-- Navigation with improved accessibility -->
    <nav>
        <ul>
            <li><a href="#driveway-patio" aria-label="Learn about our drive and patio cleaning services">Drive & Patio Cleaning</a></li>
            <li><a href="#gutter-cleaning" aria-label="Learn about our gutter cleaning services">Gutter Cleaning</a></li>
            <li><a href="#contact" aria-label="Contact us for a quote">Contact</a></li>
        </ul>
    </nav>

    <!-- Improved slider JavaScript -->
    <script>
        class Slider {
            constructor(containerId, interval = 3000) {
                this.container = document.getElementById(containerId);
                this.slides = this.container.querySelectorAll('.slides > *');
                this.index = 0;
                this.interval = interval;
                this.intervalId = null;
                this.isPaused = false;

                this.init();
            }

            init() {
                // Add pause on hover
                this.container.addEventListener('mouseenter', () => this.pause());
                this.container.addEventListener('mouseleave', () => this.resume());
                
                // Add keyboard navigation
                this.container.addEventListener('keydown', (e) => {
                    if (e.key === 'ArrowLeft') this.prev();
                    if (e.key === 'ArrowRight') this.next();
                });

                this.start();
            }

            show(index) {
                this.slides.forEach(slide => {
                    slide.classList.remove('active');
                    slide.classList.add('hidden');
                });

                this.slides[index].classList.remove('hidden');
                requestAnimationFrame(() => {
                    this.slides[index].classList.add('active');
                });
            }

            next() {
                this.index = (this.index + 1) % this.slides.length;
                this.show(this.index);
            }

            prev() {
                this.index = (this.index - 1 + this.slides.length) % this.slides.length;
                this.show(this.index);
            }

            pause() {
                this.isPaused = true;
                clearInterval(this.intervalId);
            }

            resume() {
                if (this.isPaused) {
                    this.isPaused = false;
                    this.start();
                }
            }

            start() {
                this.show(this.index);
                this.intervalId = setInterval(() => this.next(), this.interval);
            }
        }

        // Initialize sliders when DOM is loaded
        document.addEventListener('DOMContentLoaded', () => {
            try {
                const sliders = {
                    'driveway-patio': new Slider('driveway-patio', 3000),
                    'gutter-cleaning': new Slider('gutter-cleaning', 3000),
                    'customer-reviews': new Slider('customer-reviews', 5000)
                };

                // Initialize touch events for all sliders
                Object.values(sliders).forEach(slider => {
                    let touchStartX = 0;
                    
                    slider.container.addEventListener('touchstart', e => {
                        touchStartX = e.touches[0].clientX;
                    }, { passive: true });

                    slider.container.addEventListener('touchend', e => {
                        const touchEndX = e.changedTouches[0].clientX;
                        const diff = touchStartX - touchEndX;

                        if (Math.abs(diff) > 50) {
                            if (diff > 0) {
                                slider.next();
                            } else {
                                slider.prev();
                            }
                        }
                    }, { passive: true });
                });
            } catch (error) {
                console.error('Error initializing sliders:', error);
            }
        });
    </script>
</body>
</html>